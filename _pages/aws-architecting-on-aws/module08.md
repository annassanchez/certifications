---
layout: page
title: "Module 8: Automation"
permalink: /aws-architecting-on-aws/module08/  # Optional
parent: AWS Architecting on AWS # For breadcrumbs (if supported)
---

## Overview

This module provides an overview of automating the process of launching AWS Cloud infrastructure for your cloud applications. You will learn about AWS services that you can use to automate launching the cloud infrastructure.

In this module, you learn how to:

- Use AWS CloudFormation to automate infrastructure deployment
- Identify tools that automate the deployment of infrastructure and help manage resources once deployed.

## AWS CloudFormation

Building cloud infrastructure manually might lead to human errors and the deployment, so it's a good idea to automate cloud infrastructure deployment. AWS CloudFormation automates building your cloud infrastructure.

Let's talk about AWS CloudFormation.

How can we simplify our cloud infrastructure build? 

We start with the concept, infrastructure as code. Can we treat our infrastructure like code? Can I check it into a source control repository? Can I see the history of commits that were made that define our infrastructure? And the answer is yes. 

When we apply this concept, we start with an architecture template, so let's look over here. I have an architecture template here that defines how I want my infrastructure to look. That's declarative, and then we pass that on to a infrastructure as code solution, which is the product that understands that template, understands the current state of the infrastructure, and makes the changes necessary to build the architecture that I've defined in the template.

Now that comes with some advantages. I can replicate, redeploy, and repurpose because I've defined that as a simple template file. I can hand that on to someone else, and we can build exactly that same architecture in another count in another Region, in our developer environment. We can control versioning on infrastructure and applications. I check that into a source control repository, and we see the full history of commits that were used to modify the architecture. I might want to ask a question of why exactly do we have this security group in our architecture? I can look at source control and see when that was created. It was created as part of a project last week and I can see who created that commit as well. So documenting things as we're treating our infrastructure as code, we can detect drift. 

Maybe some changes have gone in and someone's just changed something manually. I just need to quickly go in and diagnose something. I'm just going to open up this access, and I'm gonna go and diagnose it. And I'm sure I'll change it back on Monday. What happens if we don't change it back on Monday? We can use our IaC solution to detect where we differ from our desired state that's written into that template, and like any piece of code, we can roll back. We've made some modifications to our architecture. Maybe things aren't quite working out. We've run some tests on it and we're seeing some latency. Before we diagnose, let's just roll back that commit, hand it on to our IaC solution, and revert back to the state that we were before the changes. 

Some benefits of reusability at the bottom of the screen there. I'm defining a template. Inside of that template is a definition for resources. I'm defining some Auto Scaling groups, a load balancer, and I want that in development, and I want exactly the same architecture in production. If you were to contrast that with doing it manually, I'm going into the console, building all these things for my development environment, and I need to remember exactly how I built it to hand that over into my production environment. The more human hands that are involved with building infrastructure, the more likely things are going to get forgotten. Mistakes are going to be made. Let's hand all that work onto our IaC service to build the infrastructure for us.

I want to make a modification to my infrastructure. We need some new security groups. That's a change to the template. We see the difference in desired state. The template now has a resource that is not in our observed state. We can see that difference and the product will go and make the changes for me.

Now, we talk about AWS CloudFormation and as you might have guessed it, this is the service that we use to treat infrastructure as code. Very similar concepts to what we've just gone over. I define my infrastructure as a template. I have an application. The application needs EC2 instances. It needs roles, it needs security groups. It needs a load balancer. I define that in a template. I'm defining it declaratively. I'm just saying this is what I desire, not the steps to create it, just the finished product. 

I hand that on to CloudFormation, and CloudFormation makes the API calls to go and make the infrastructure on this side. Not only are we creating infrastructure, we're modifying infrastructure. That template is not going to remain static. Some changes happen to my application, some changes happen to my infrastructure. I get told, okay, we need to install this monitoring software on all of the instances. I need to make changes to the template. I need to add additional roles to my EC2 instances I make the change over here. CloudFormation knows the difference between our observed state and our desired state, and makes the changes to my infrastructure via some API requests on this side. What CloudFormation creates is called a stack. A stack is a set of resources that will now travel together. If I want to delete the resources that were created by a template, I delete the stack. That's much more convenient than doing things manually where I have to remember what exactly was that I created. I need to go back through all of that and delete everything. No, let's treat all of that as a single stack, and I can delete that in one operation.

What does a CloudFormation template look like? 

We can write CloudFormation templates in JSON or YAML. It describes the resources that we want to create. If I look over here in my JSON, I have a resources key. Exactly the same in the YAML is the resources. That is defining AWS infrastructure, and we say treat it as source code. I can check it into a source code repository. I can have someone else look at my commits. We can do a code review. Are we not happy with the code review? We can roll back a commit. When we're happy with it, let's hand that code on to CloudFormation. That will build the resources for us.

The stack is the collection of resources that are created from a template. We deploy and delete resources as a unit. This has big advantages over trying to do things manually. We can update resources and settings on a running stack. The example that I gave earlier, we just need to change a security group. Let's make the modification to the template. Check that into source control. We'll see the commit, we'll see who made that commit, and then hand that on to CloudFormation so that we can modify the stack. We can certainly nest stacks. A stack is an AWS resource like any other resource.

CloudFormation can create AWS resources, so a template can contain a stack. You can also do cross-stack references. A template can have an output. When I run a template in the same Region, I can refer to the outputs of another stack. That's another nice way that we can cross reference between stacks.

We say it's a good practice to work with a layered architecture like we have on the diagram here. I'm imagining I'm building a new application and there's quite a few things that I need to build. There is a library within my organization and I'm ready to build my application. I need to build some identity resources. I need IAM users, groups, and roles. Someone has already written a template for me to do that. That's the bottom layer of my stack. My application needs some network resources, VPCs, internet gateways, VPNs.

That's another template that someone who's already designed for me, that might also speed up some approval process. You're building the application. Are we compliant? Just use this template. It's already been approved. You are going to be compliant. As I move up the stack, I also want to create some databases, monitoring alarms, subnets, security groups. 

This is another stack. How does that stack know where to create these resources?

CloudFormation templates can be parameterized, so I run this shared resources template. One of the parameters that it will request is the VPC. Where exactly do you want to create these things? And this is how we can build layers on top of previous layers, by taking that as a parameter in the template. And I move up, there's more that I need to create on the backend. There's more that I need to create on the frontend. And again, I can take a preexisting template. We have a library of templates. Pass in parameters to tell it where to build my resources. And now, I'm getting my application done much quicker than if I had to go and build that manually, and go through some forms of approval process.

### Infrastructure as Code (IaC)

You can simplify the deployment of your AWS resources using infrastructure as code (IaC). With IaC, you use code to define, deploy, configure, update, and remove infrastructure through a template. A template is a text file that describes and defines the resources to be deployed in your environment.

A template can be used to:

- Define an entire application stack (all resources required for your application) in a JSON or YAML template file. Treat the template as code and manage it using a version control system.

- Define runtime parameters for a template, such as the Amazon Elastic Compute Cloud (Amazon EC2) instance size and Amazon EC2 key pair.

![/assets/images/](/assets/images/module08-01.png)

Benefits of IaC:

- Speed and safety – Your infrastructure is built programmatically, which makes it faster than manual deployment and makes errors less likely.

- Reusability – You can organize your infrastructure into reusable modules.

- Documentation and version control – Your templates document your deployed resources, and version control provides a history of your infrastructure over time. You can also roll back to a previous working version of your infrastructure in the event of error.

- Validation – You perform code reviews of your templates, which decreases the chances of errors.

### AWS CloudFormation

With AWS CloudFormation, you can create and manage AWS infrastructure deployments predictably and repeatedly. You can use CloudFormation to use AWS products—such as Amazon Elastic Compute Cloud (Amazon EC2), Amazon Elastic Block Store (Amazon EBS), and so on—to build highly reliable, highly scalable, cost-effective applications without creating or configuring the underlying AWS infrastructure.

With CloudFormation, you declare all your resources and dependencies in a template file. The template defines a collection of resources as a single unit called a stack. CloudFormation creates and deletes all member resources of the stack together and manages all dependencies between the resources for you.

To learn more about each step in the process, choose each hotspot.

![Building cloud infrastructure using AWS CloudFormation](/assets/images/module08-02.png)

### Stacks

All resources in a stack are defined by the stack’s CloudFormation template. You can manage a collection of resources by creating, updating, or deleting stacks. For example, a stack can include all resources required to run a web application, including a web server, database, and networking rules. If you no longer require that web application, you can delete the stack, which deletes all of its related resources.

CloudFormation treats the stack resources as a single unit. They must all be created or deleted successfully for the stack to be created or deleted. If a resource can't be created, CloudFormation rolls the stack back and deletes any resources that were created.

Next, you will learn how to manage the cloud infrastructure you created.

## Infrastructure Management

Once you build cloud infrastructure using AWS CloudFormation, you should deploy, maintain, and scale applications in the cloud. In this lesson, you learn how to manage cloud infrastructure.

Up next, let's talk about some infrastructure management. 

What can help us deploy, maintain, and scale our applications in the cloud?

And we have some services and some options laid out here on a spectrum of convenience to control. Elastic Beanstalk, we'll talk more about these services on the following slides.

Beanstalk is a service that I can hand on some code, and it will build the infrastructure to host that code and deploy it for me.

AWS Solutions Library, aws.amazon.com/solutions, is a place where you can find solutions that have been approved by AWS architects.


AWS Cloud Development Kit builds on what we just spoke about in CloudFormation. It is a software library for you to be able to use the programming languages you're familiar with, to build the defined infrastructure that we hand on to CloudFormation, and we can get a lot of the benefits of code reuse there.

CloudFormation, we've spoken about, is the service that I can hand a template and it will build and update infrastructure for me. On the management side, we will talk about AWS Systems Manager, which is a service that can automate a lot of operational type tasks in your infrastructure.

So, we start with AWS Elastic Beanstalk. This is a service that I can zip up some code, hand it on to Beanstalk, and it will build the infrastructure to host my application. If it is a load-balanced application, you have the choice of single host or load balanced. It will create the EC2 instance, it will create the load balancer, it will create Auto Scaling groups, and it actually uses CloudFormation to do this.

When you create an application in Beanstalk, you'll see a stack appear in CloudFormation for it. It supports Docker, Go, Java, .NET, Node, PHP, Python, Ruby, a lot of popular application programming languages. And because it supports Docker, you can hand on a container for it to deploy as well. It provisions your infrastructure, it manages the application stack, it is deploying the application for you. It will also update applications. My applications are not static. I supply a new addition of the code and Beanstalk will automate, deploying that code to all of my hosts. Automatically scales up and down. As it is creating the infrastructure, it is also creating Auto Scaling groups for me. And I have a lot of control over that. There's a lot of settings and parameters that I can go in there and tell it when I wish to scale. 


AWS Solutions Library is at aws.amazon.com/solutions. You'll find some reference architectures, deployment accelerators. These are solutions approved by the AWS architects. You'll find CloudFormation templates, you'll find scripts, you'll find sample applications. A lot of it is inside of a GitHub repository. If you look at the AWS Solutions GitHub repository, you'll find all the code that goes with these solutions.

AWS CDK, Cloud Development Kit, is a software development kit for different languages. I've used it with Node, I've used it with Python, and it allows me to write code that defines infrastructure. The output of a CDK build is an actual CloudFormation template. It will create a CloudFormation template. We can hand that on to CloudFormation and build my stack. The advantage here is mostly code reuse. If there's a certain way that you like your applications to be deployed, you can build that as a construct, it's called in CDK. There are existing constructs. For example, there is an Application Load Balanced Fargate Service. That single construct will create a 400-line CloudFormation template for you, which gives you a lot of benefit of reuse.

We can define things in code, write code exactly how you like it. The output from that will be a declarative template and I can hand that on to CloudFormation to build my environments. 

AWS Systems Manager is a service that can automate a lot of operational tasks on your infrastructure. It is made possible by the SSM Agent running on your instance. If you turn on an Amazon AMI, the SSM Agent is already there. If you have the correct roles configured on your instance, it's able to receive messages from the Systems Manager service. And using that, we can automate a lot of things, like updating, managing, and configuring servers. There are automation documents that can automate a lot of the processes that you do in AWS. There are examples, like I need to diagnose a Windows instance. The automation document will go through the multiple steps to clone the drive in there, attach it to a new instance, and run some system checks on it. Those are the sort of things that we're doing with the automation documents. We can check compliance, we can run scripts, you can do a run script by tag. So I need to go and find out what version of a Java logging library is installed on all of my servers. I can run that as a script, and I can say run that script against all instances tagged with Java, for example. We can do remote administration with Session Manager and install patches using the Patch Manager.

### Infrastructure tools

When choosing infrastructure deployment tools, you need to find a balance between convenience and control. Some tools give you complete control and have you choose every component and configuration. Though you can customize your deployment to fit your business needs, this requires greater expertise and more resources to manage and maintain. Other tools are designed for convenience and include preconfigured infrastructure templates for common solutions. Though these tools are easier to use and require less maintenance, you do not always have the ability to customize your infrastructure components.

![Infrastructure Tools](/assets/images/module08-03.jpg)

#### AWS Elastic Beanstalk

Elastic Beanstalk configures each EC2 instance in your environment with the components necessary to run applications for the selected application type. You don’t have to worry about logging in to instances to install and configure your application stack. With Elastic Beanstalk, you can provision infrastructure to support common application designs, such as web applications and worker services.

![AWS Elastic Beanstalk](/assets/images/module08-04.png)

#### AWS Solutions Library

The AWS Solutions Library helps you solve common problems and build faster. Solutions are vetted by AWS architects and are designed to be operationally effective, reliable, secure, and cost efficient. Many AWS solutions come with prebuilt CloudFormation templates. They may also include a detailed architecture, a deployment guide, and instructions for automated and manual deployment. 

#### AWS Cloud Development Kit (AWS CDK)

![(AWS CDK)](/assets/images/module08-05.jpg)

AWS Cloud Development Kit (AWS CDK) is a software development framework that defines your cloud application resources by using a declarative model and familiar programming languages. AWS CDK includes a library of customizable constructs, which are building blocks consisting of one or more resources and include common configurations. You can use AWS CDK to generate CloudFormation templates and deploy your infrastructure along with your application runtime assets.  

You can use AWS CDK with common programming languages such as Python, JavaScript, TypeScript, Java, or C#.

#### AWS Systems Manager

AWS Systems Manager is a collection of capabilities to help you manage your applications and infrastructure running in the AWS Cloud. Systems Manager simplifies application and resource management, shortens the time to detect and resolve operational problems, and helps you manage your AWS resources securely at scale.

AWS Systems Manager provides a central place to view and manage your AWS resources, so you can have visibility and control over your operations.

With Systems Manager, you can:

- Create logical groups of resources, such as applications, different layers of an application stack, or development and production environments.
- Select a resource group and view its recent API activity, resource configuration changes, related notifications, operational alerts, software inventory, and patch compliance status.
- Take action on each resource group, depending on your operational needs.
- Centralize operational data from multiple AWS services and automate tasks across your AWS resources.

![AWS Systems Manager](/assets/images/module08-06.jpg)