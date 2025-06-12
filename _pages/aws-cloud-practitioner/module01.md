In this track of the CLF-C02: AWS Certified Cloud Practitioner journey, the focus will be on the following:

- Define the benefits of the AWS Cloud• Identify design principles of the AWS Cloud
- Understand the benefits of and strategies for migration to the AWS Cloud
- Understand concepts of cloud economics

## Skill Benchmark

The Cloud Concepts and Cloud Economics Literacy (Beginner Level) benchmark measures your knowledge of the fundamentals of AWS networking and compute services and cloud architecture design principles. You will be evaluated on your ability to define aspects of the AWS Cloud, its value proposition, and the characteristics of AWS Cloud Economics.

Learners who score high on this benchmark demonstrate that they have the skills to recognize cloud architecture design principles and Cloud Economics.

### Topics covered:

- Recall key service offerings of Amazon Web Services (AWS)
- Describe the shared responsibility model and the AWS security triad
- Define compute as a service in AWS
- Describe the Amazon Elastic Compute Cloud (EC2) service
- Compare server-based instances and containers to serverless Lambda functions and Fargate containers
- Describe the Amazon Virtual Private Cloud (VPC) components

## Why take a Skill Benchmark?

- Determine your skill level in a particular area – you can’t fail
- Help your company gauge where to target its resources
- Challenge yourself to learn new skills and improve your score

## What to expect:

- Mostly multiple choice, but some matching and ranking questions
- Immediate results
- Your scores not visible to other learners


## AWS Cloud Practitioner: Benefits & Design of the AWS Cloud

### Course Overview

In this video, we will discover the key concepts covered in this course.

- discover the key concepts covered in this course[Video description begins] *Topic title: Course Overview. Your host for this session is Michael Shannon.* [Video description ends]

Benefits and design principles of the AWS Cloud. It has always been a top priority for Amazon Web Services to provide all potential and 
existing customers with the knowledge and tools necessary to conduct proper due diligence. In this course, we will: 

- outline the value proposition of the AWS Cloud and understand the economies of scale.
- We'll describe the AWS global infrastructure and list the advantages of high availability, elasticity, and agility.
- And wrap it up by defining the AWS Well-Architected Framework and the six pillars of design principles of the Well-Architected Framework.

### The Value Proposition of the AWS Cloud

- Let's go ahead and define cloud computing right from the source. Let's see what Amazon Web Services has to say about it. Cloud computing is the **on-demand delivery of compute power**. In other words, virtual CPU and virtual RAM, database, storage, applications, and other IT resources through a cloud services platform via the Internet with pay-as-you-go pricing.
- Whether you're running applications that share photos to millions of mobile users or you're supporting the critical operations of your business, a cloud services platform provides rapid access to flexible and low-cost IT resources.
- With cloud computing, you don't need to make large upfront investments in hardware and spend a lot of time on the heavy lifting of managing that hardware.
- Instead, you can provision exactly the right type and size of computing resources you need to power your newest bright idea or operate your IT department.
- You can access as many resources as you need, almost instantly, and only pay for what you use.

One of the biggest value propositions of cloud computing is the ability **to trade fixed expenses** for **variable expenses**. But what does that mean exactly? 

- Well, you only pay for what is needed and used.
- Customers can pay only when they consume computing resources like a utility, for example, your water bill, your electric bill, or your mobile phone bill.
- The default model is to only pay for what is consumed.
- You can reduce upfront capital expenditures or CapEx by avoiding heavy investments in server farms, data centers, and blade server stacks before you know how you're going to use them.

Another characteristic is to **benefit from massive economies** of scale. 

- By using cloud computing, customers can obtain a much lower adaptable cost than they can get on their own.
- New customers can leverage the utilization and experience of hundreds of thousands of other customers aggregated in the cloud.
- Cloud service providers like AWS can realize higher economies of scale which leads to lower pay-as-you-go pricing.

Stop guessing capacity. 

- Remove the need to guess about infrastructure and service capacity needs.
- Customers typically find themselves either sitting on costly idle resources or struggling with inadequate capacity.
- Proper capacity decisions can be made prior to application deployment, and a cloud consumer can access as much or as little capacity as needed, and scale up and down as required, with only a few minutes' notice. And you may think that scaling up or adding capacity is the true value add. But sometimes in some situations, for example, a global pandemic, the ability to scale down or de-provision can be even more valuable.

With cloud computing, you can increase speed and agility. 

- Cutting-edge IT resources are only a click away in a cloud computing environment.
- Customers decrease the time to make resources available to 
administrators and developers from weeks to merely minutes in many circumstances.
- The outcome of cloud computing is a substantial increase in agility for the enterprise.
    - The resources, for example, cost and time necessary to experiment and develop can be considerably lower.

Stop spending money running and maintaining data centers. 

- Cloud customers can prioritize projects and propositions that set the business apart from competitors rather than the infrastructure.
- AWS cloud computing lets organizations focus on their own customers instead of the overhead and heavy lifting of racking, stacking, and powering racks of server blades.
- Large and unsustainable data centers will become a thing of the past due to global cloud consuming.

And finally, go global in minutes. 

- Organizations can effortlessly deploy data and applications in several regions around the world, pretty much all the continents, with just a few simple clicks.
    - This results in lower latency and a better experience for customers at a minimal cost.
- AWS customers are leveraging edge locations and availability zone data centers in over 30 geographic regions throughout the world.
- And new availability zones and regions are added every year.

### Economics of Scale

### outline the economies of scale

In the previous lesson, we mentioned that one of the value 
propositions of cloud computing is **economies of scale**. In this lesson, I want to elaborate more on this concept. 

- It refers to the ability to **lower costs** and **raise the efficiency** when operating at a larger scale in comparison to operating at a smaller scale.
- Since cloud customers are becoming more motivated and willing to drive growth through technology, they often look to strategies such as cost-reducing while enabling innovation.
- Cloud economics transcends simply cutting cloud costs. It's about addressing business goals through greater speed, agility, and flexibility.
- Considering the larger perspective in this way helps IT groups to select the best cloud solution for their projects, programs, and initiatives.
    
    For example, in a traditional infrastructure, you have capital expenditures on equipment or infrastructure components, you have resources and administrative overhead, contracts and agreements, and general costs. 
    
    But in the AWS Cloud, you have no upfront expense, you only pay for what you use. You can improve time to market and agility and that could mean using an Agile Software Development Lifecycle or Agile Project Management. You can quickly scale up and scale down and you can leverage a self-service infrastructure.
    

What are some traditional examples of economies of scale? 


- Well, technical. Large capital equipment with high fixed costs.
- Specialization. The division of labor and specialization within  production. In other words, a more efficient way to deliver with high output or
- bulk buying, lowering the average costs by buying large quantity. In the cloud, for example, at AWS, the more data storage you use, the cheaper it is by gigabyte.
- Marketing; national ad campaigns may be more efficient for high sales.
- Risk bearing. You can transfer risk. Bigger firms are more able to survive downturns when using the cloud, especially because of auto-scaling.
- Container principle. Increase in the surface area leads to double the increase in volume.
- Financial economy of scale. A large firm gets better rates of interest from the bank or
- external economy of scale when a firm benefits from the whole industry increasing in size or becoming more popular.

One of the primary aspects of Amazon Web Services economy of scale is their global infrastructure. In the next lesson, we'll take a web Safari up to Amazon Web Services and learn about their global infrastructure of Availability Zones, data centers, and edge locations all over the world.

### Exploring AWS Global Infrastructure

### recognize the benefits of the AWS global infrastructure including regions, availability zones, and edge locations

[Global Infrastructure -  AWS](https://aws.amazon.com/about-aws/global-infrastructure/)

All right, in this first demo, we're going to do a web Safari up to AWS and we're going to look at the global infrastructure and realize that AWS has regions all over the world.

We can see North America, South America, Europe, Middle East, Africa, Asia Pacific, and Australia and New Zealand.

If we look at Europe here, these little circles represent regions. 
Now, one thing about AWS is that every region in the world has at least three Availability Zones. OK. So, if we go here, let's say to Frankfurt, we can see there's 3 **Availability Zones**.

[Video description begins] *A pop up appears on the dot on the map of Europe. It shows: Frankfurt. Launched 2014. Availability Zones: 3 | Local Zones: 2.* [Video description ends] 

Now on the exam, don't confuse **Availability Zones**, which we will discuss in more detail throughout this training with **Local Zones**.

Local Zones are really for hybrid cloud or edge computing. So, we'll talk about Local Zones later on in this training. 

But in this lesson, we want to focus on Availability Zones Now, an Availability Zone is at least two data centers and those two data centers can be relatively close like on a Metro Ethernet or a fiber ring. So, they're relatively close. 

But the Availability Zones, because of the technology that's being used, specifically VXLAN, Virtual Extensible LAN, the Availability Zone data centers can be theoretically up to 600 miles apart or about 800 kilometers. 

So, in this region, let's say Spain, those 3 Availability Zones are many miles apart, dozens or hundreds of miles apart and that's for durability, high availability, and resiliency. 

[Video description begins] *A new pop up appears on a dot on the map. It displays: Spain. Launched 2022. Availability Zones: 3.* [Video description ends] 

And if we were to look at all these different areas, for example, South America just has one region here in Sao Paulo, Brazil. But if you were to look at these, for example, North America, the Northern Virginia region, which is right here, has 6 Availability Zones. 

[Video description begins] *A pop up appears on a dot on the map of North America. It shows: Northern Virginia. Launched 2006. Availability Zones: 6 | Local Zones: 12 | Wavelength Zones: 8.* [Video description ends] 

So, this is the largest region in AWS's global infrastructure. And so those are many miles apart, and of course, we're servicing not just Washington D.C., but Northern Virginia and other cities like Philadelphia and Baltimore, and don't forget North Carolina has a lot of IT and universities.

Now right next to that, we see what's called GovCloud. So, this is a separate community cloud just for the US government.

[Video description begins] *A pop up appears on a dot on the map of North America. It displays: AWS GovCloud (US-East). Launched 2018. Availability Zones: 3.* [Video description ends] 

The GovCloud in Northern Virginia region are really isolated from each other and separate. If you see one that's red here, it means it's coming soon. OK, now, when Canada West rolls out, and by the time you're doing this training, it may be rolled out, there will be at least 3 Availability Zones. 

Something else about these zones. Let's go back to Europe. If we scroll down, we'll see the different regions, at least 3 Availability Zones in each region. What we're also going to have is edge locations.

[Video description begins] *The Europe option is active now. Below the map, there are three sections: Europe, AWS Edge Locations, and Regional Edge Caches. The Europe section contains information about different regions such as name, launch year, and Availability Zones. The AWS Edge Locations sections contains names 
of different cities.* [Video description ends] 

So, edge locations have several functions, but the primary function is for something we're going to learn later called Content Distribution Networking or Content Delivery Networking. Maybe you've heard of something like Akamai or Cloudflare? Well, AWS has CloudFront, and this is just a way for you to get your content a wide variety of different things close to your customers.

So, if they want to stream your audio or stream video, or watch your documentary or get your content or maybe access data, you can get copies of it close to them. So, for example, if you have customers in Prague or if you have customers in London or Manchester, or Frankfurt, you can just distribute copies of this content to these edge locations and then your customers in those areas can then get the content from there. OK, so, these edge locations are very important and they're also part of the AWS global infrastructure. 

And so, this is how we get all of those wonderful global benefits of high availability and resiliency and durability of data because we have regions all over the world and you want to be aware of this on the exam.

You can also check out Middle East, we have several there. Asia 
Pacific has a couple coming soon, for example, in Thailand and Malaysia. Japan has a pretty big region. The Tokyo region has 4 Availability Zones. 

[Video description begins] *A pop up appears on a dot on the map of Asia Pacific. It displays: Tokyo. Launched 2011. Availability Zones: 4 | Local Zones: 1| Wavelength Zones: 2.* [Video description ends] 

You'll also notice on this pop-up here something called Wavelength Zones. That is for 5G. 

OK, so Wavelength Zones or for what we call 5G gateways. And we can see Seoul, South Korea has 4 Availability Zones as well. So, 
that's the global infrastructure of Amazon Web Services. 

[Video description begins] *A new pop up appears on a dot on the map of Asia Pacific. It shows: Seoul. Launched 2016. Availability Zones: 4 | Wavelength Zones: 1.* [Video description ends] 

Be familiar with it on your Cloud Practitioner exam.

### Advantages of High Availability, Elasticity and Agility

### *Topic title: Advantages of High Availability, Elasticity, and Agility.*

*Your host for this session is Michael Shannon.* [Video description ends]

In the previous lesson, as we looked at the AWS global infrastructure, we saw an example of massive global **high availability**. 

- High availability protects against data center, Availability Zone (AZ), server, network, and storage subsystem failures.
    - You can keep your organization or your business running with little or no downtime.
- All Availability Zones in an AWS region are interconnected with 
high-bandwidth, low-latency networking over fully redundant, dedicated metro fiber.
- Data centers located in different AWS Availability Zones have a discreet, uninterruptible power supply and onsite backup generation facilities.
- Most providers of real-time communications align with service levels that provide availability from 99.9% to 99.999%, otherwise known as five nines, which means your planned and unplanned downtime is literally only minutes per year.
- Depending upon the degree of High Availability needed at AWS, 
customers can take progressively sophisticated steps along the full life cycle of the service or the application.
- AWS recommends following these guidelines to achieve a robust degree of high availability.
    - Design the system or application to have no single point of failure by using automated monitoring, detection, and failover mechanisms for both stateless and stateful components. Remember, a stateful component has data or metadata stored about that state, in some type of construct or table, or buffer.
    - Correctly instrument and test system availability.
    - Prepare operating procedures for manual mechanisms to respond to, mitigate, and recover from the failure.

Let's talk more about **elasticity**. 

- Elasticity provides the ability to almost instantly provision and de-provision assorted cloud resources.
    - This could be virtual instances, for example at AWS, Windows Server 2019, 2022, various Linux builds including their own machine images, and even MacOS. They could be containers, appliances, virtual appliances from many different partners, database tables, and more.
- Elasticity involves leveraging dynamic auto-scaling technologies, 
typically referring to scaling out the virtual instances or the 
containers or appliances.
- Another advantage of elasticity is that there's many challenges with predicting demand in the enterprise, which leads to higher costs.
- Recent circumstances, for example, starting in 2020, have revealed how de-provisioning may be the more vital aspect of elasticity. In other words, a company can run at 70% for months after months if they're running most of their business in the cloud.

**Advantages of Elasticity:**

Let's see what Yury Izrailevsky, the vice president of cloud and platform engineering at Netflix says, "Elasticity of the cloud allows us to add thousands of virtual servers and petabytes of storage within minutes, making such an expansion possible. Leveraging multiple AWS cloud regions, spread all over the world, enables us to dynamically shift around and expand our global infrastructure capacity, creating a better and more enjoyable streaming experience for Netflix members wherever they are."

![image.png](attachment:ac8cfe00-ecb8-4553-bbd3-bbd632448f85:image.png)

- By using cloud elasticity at Amazon Web Services, we can reduce waste and we can reduce customer satisfaction. When the predicted demand is less than actual demand, we have waste, when the actual demand is greater than predicted demand, we have customer satisfaction, and this is more common with rigid on-premises resources.
- However, in the cloud, our predicted demand will be much more closely aligned with actual demand because we're relying on elastic cloud-based resources.

Cloud computing also offers **agility**. 

- Agility leverages features for rapid deployment, testing, experimentation, and innovation.
- Customers can quickly overcome geographical limitations.
- And content creators can get customer content as close to the customer as possible.
- Agility means reducing time and costs for testing, innovation, and experimentation.

**Advantages of agility:**

- With AWS as the producer, consumers can co-create value and deliver 
data, applications, services, and solutions.
- Agility also includes the concept of flexibility in terms of many 
different options, but the two terms aren't exactly the same. For 
example, growing up, I may have been very fast and agile and quick, but not very flexible.
- The decision to "build or buy", otherwise known as acquire or construct, can be more adaptable for your DevOps programs. Remember, DevOps is a clipped compound of development and operations.
- The value proposition of agility integrates with the Agile development and Agile project management as well.

How can you make sure that you take advantage of all of the value 
propositions at Amazon Web Services? Well, in the next lesson, we'll 
look at their Well-Architected Framework, which will put you on the path to taking advantage of all of the propositions and features and 
characteristics that the AWS cloud has to offer.

### Exploring the Well-Architected Framework Design Principles

### identify the six pillars of the AWS well-architected initiative

In this lesson, we're going to do a web Safari up to Amazon.com and 
get a basic understanding of the AWS Well-Architected or architectural 
best practices. 

[AWS Well-Architected - Build secure, efficient cloud applications](https://aws.amazon.com/architecture/well-architected/?wa-lens-whitepapers.sort-by=item.additionalFields.sortDate&wa-lens-whitepapers.sort-order=desc&wa-guidance-whitepapers.sort-by=item.additionalFields.sortDate&wa-guidance-whitepapers.sort-order=desc)

[Video description begins] *A web page appears with the heading: AWS Well-Architected. It contains a menu with various options: Products, Solutions, Pricing, Documentation, Learn, Partner Network, and More. Below, the banner contains a button: Get started with the AWS Well-Architected Tool. Further, it contains various options: AWS Well-Architected Tool, AWS Well-Architected Pillars, AWS Well-Architected Lenses, AWS Well-Architected Guidance, AWS Architecture Center, and Partners.* [Video description ends] 

So, on the exam, you want to be able to define simply what **Well-Architected** is, and it says right here. 

> *It helps cloud practitioners, engineers, and architects build secure, high-performing, resilient, and efficient infrastructure for a variety of applications and workloads.*
> 

That's the definition. Now, we have a tool that can help us as well called the Well-Architected Tool. So, learning best practices and applying important design considerations. 

Also in Well-Architected, if we go back, we'll notice that there are six pillars. Also on the exam, you'll want to be able to memorize these six pillars.

[Video description begins] *The main pane displays: AWS Well-Architected and the Six Pillars. Below, it displays: Framework Overview. Further, it contains the six headings with descriptions: Operational Excellence Pillar, Security Pillar, Reliability Pillar, Performance Efficiency Pillar, Cost Optimization Pillar, and Sustainability Pillar. Beneath each heading, there are two buttons: HTML and Labs.* [Video description ends] 

Remember, on the CLF-C02 exam, you're going to have a number of questions, there are going to be, let's say, five possible answers and two out of the five will be correct.

- The Operational Excellence Pillar: The operational excellence pillar focuses on running and monitoring systems, and continually improving processes and procedures. Key topics include automating changes, responding to events, and defining standards to manage daily operations.
- the Security Pillar, The security pillar focuses on protecting information and systems. Key topics include confidentiality and integrity of data, managing user permissions, and establishing controls to detect security events.
- the Reliability Pillar,  The reliability pillar focuses on workloads performing their intended functions and how to recover quickly from failure to meet demands. Key topics include distributed system design, recovery planning, and adapting to changing requirements.
- the Performance Efficiency Pillar, The performance efficiency pillar focuses on structured and streamlined allocation of IT and computing resources. Key topics include selecting resource types and sizes optimized for workload requirements, monitoring performance, and maintaining efficiency as business needs evolve.
- Cost Optimization, The cost optimization pillar focuses on avoiding unnecessary costs. Key topics include understanding spending over time and controlling fund allocation, selecting resources of the right type and quantity, and scaling to meet business needs without overspending.
- and Sustainability. The sustainability pillar focuses on minimizing the environmental impacts of running cloud workloads. Key topics include a shared responsibility model for sustainability, understanding impact, and maximizing utilization to minimize required resources and reduce downstream impacts.

So, you would have two of these correct answers. You would have five options, one would be Performance Efficiency, the other Reliability. The other three would be distractors. In fact, they may be actually trusted advisor categories. So, on the exam, you want to be aware of these different pillars and these basic descriptions here. 

OK, the operational excellence pillar focuses on this. The security 
pillar focuses on protecting information and systems, reliability pillar on workloads, performing their intended functions, also how to recover. Performance efficiency, that goes without saying, streamlining the allocation of your computing resources. Cost optimization and of course, sustainability, minimizing the environmental impact of running cloud workloads. 

So, you need to be aware of the six pillars and a kind of brief understanding of these pillars. I also want you to know that within each one of these pillars you have Labs and, in these Labs, it's kind of like going to college, right? You've got Foundational level, 100 level is like your freshman year, 200 level is sophomore, 300 is your junior year, and the senior year would be Quests.

[Video description begins] *A new web page appears with the heading: Security :: AWS Well-Architected Labs. The left navigation menu contains various options: Operational Excellence, Reliability, Performance Efficiency, Cost Optimization, and so on. The Operational Excellence option contains a sub-option: Security. The Security sub-option contains four collapsible options: 100 Level Foundational Labs, 200 Level Intermediate Labs. 300 Level Advanced Labs, and Quests. The main pane displays: SECURITY. Below, it contains the Introduction.* [Video description ends]

So, these are all walkthroughs that you can go through. 100, 200, and 300 or walkthroughs. They're going to provide you often with an infrastructure as code environment. 

So, they'll give you a YAML, Yet Another Markup Language, YAML or JSON, JavaScript object notation, template, and that kind of create your lab environment. You go through the walkthrough and then you tear it down.

[Video description begins] *The 100 Level Foundational Labs collapsible option is open. It contains various options: Account Setup and Root User, Identity and Access Management User, Group, Role, CloudFront with S3 Bucket Origin, Enable Security Hub, and Create a Data Bunker Account.* [Video description ends] 

So, they provide those for you. 

The Quests aren't walkthroughs. They're going to give you tasks to go through and you basically leverage what you learned in these walkthroughs at the 100, 200, and 300 level to accomplish the Quests. 

And as you can see, you've got Labs for each one of these Well-Architected pillars. And obviously, it depends on what your specialty is. Mine happens to be Security. So, I've spent quite a bit of time going through the Security Labs and they're very helpful. 

In the next lesson, we're going to dig a little bit deeper and we're going to look at the design principles of each one of these six pillars.

### compare the design principles of the six well-architected pillars

### compare the design principles of the six well-architected pillars

In this lesson, we're going to dig deeper into the six pillars of the AWS Well-Architected framework because on the exam, they may ask you questions about the actual design principles in each one of those 
pillars. 

[Video description begins] *A web page appears with the heading: The 6 Pillars of the AWS Well-Architected Framework. It contains various tabs such as: Products, Solutions, Pricing, Documentation, Learn, Partner Network, and More. Below, it contains three options in a bar: AWS Blog Home, Blogs, and Editions. The main pane displays: AWS Partner Network (APN) Blog.* [Video description ends]

Now it's odd, but this is really difficult to find at the AWS Well-Architected site. 

[The 6 Pillars of the AWS Well-Architected Framework | Amazon Web Services](https://aws.amazon.com/blogs/apn/the-6-pillars-of-the-aws-well-architected-framework/)

So, I'm going to use this blog article that was written by Seth Eliott and Lara Valverde. It's been updated in 2022. If we scroll down here, we'll see Operational Excellence and then some design principles for Operational Excellence. 

[Video description begins] *The main pane now displays the heading with description: Operational Excellence. Below, it contains two sub-headings with points: Design Principles and Best Practices.* [Video description ends]

**Operational Excellence**: 

- Perform operations as code,
- make frequent, small, reversible changes,
- refine operation procedures frequently,
- anticipate failure,
- and learn from all of your operational failures.

And so, you may have a question on the exam, and they'll give you a multiple-choice question, you'll have to know that performing operations as code is a design principle of Operational Excellence.

If we come down to **Security**, there are seven design principles for 
Security. 

- Implement a strong identity foundation,
- enable traceability, that may be on the exam,
- apply security at all layers. For example, layer three of the OSI model all the way up to layer five,
- automate security best practices,
- protect data in transit and data at rest.
- Keep people away from data. In other words, it should only be acting on a abstraction view or a copy of that data
- and prepare for security events.

The **Reliability** pillar has five design principles. 

- Automatically recover from failure,
- test recovery procedures,
- scale horizontally to increase aggregate workload availability,
- stop guessing capacity,
- and manage change in automation.

Number 4 is **Performance Efficiency**. Performance Efficiency has five design principles. 

- Democratize advanced technologies. In other words, don't just let your DevOps team or your data analyst use the advanced technologies of Amazon Web Services. Consider how all your different departments and business units and organizational units can benefit from the cloud.
- Go global in minutes,
- use serverless architectures, we'll talk more about that later in this training.
- Experiment more often
- and consider mechanical sympathy. In other words, not everything's right for virtualization and the cloud.

**Cost Optimization**. 

- Implement cloud financial management,
- adopt a consumption model,
- measure overall efficiency,
- stop spending money on undifferentiated heavy lifting,
- and analyze and attribute your expenditure.

And finally, we have the **Sustainability** pillar with six design principles. 

- Understand your impact,
- establish sustainability goals,
- maximize utilization,
- anticipate and adopt new, more efficient hardware and software offerings,
- use managed services,
- and reduce the downstream impact of your cloud workloads.

Make sure you're familiar with these design principles and that you can map them to the actual pillar on the exam.

[Video description begins] *Various points like Security, Reliability, Performance Efficiency, Cost Optimization, and Sustainability are displayed one after the other.* [Video description ends]Course Summary

### Course Summary

In this course, 

- you learned about the AWS value proposition and economy of scale.
- High availability, elasticity, and agility,
- and the AWS Well-Architected Framework.

Coming up in the next course, we'll look at migration to the AWS Cloud and cloud economics.


## AWS Cloud Practitioner: Migration to the AWS Cloud and Cloud Economics

### Course Overview

There is a profound saying in The Art of War by the renowned Chinese General Sun Tzu. Tactics without strategy is the noise before defeat.

It is critical that all potential customers of AWS understand migration options, strategies, and all aspects of AWS cloud economics 
before placing a single file, data, or app into the cloud.

In this course: 

- we will discover the benefits of the AWS Cloud Adoption Framework (AWS CAF),
- identify proper migration strategies,
- understand cost models and licensing strategies,
- and define the concept of right sizing.

### Cloud Adoption Strategies and Resources

In this first lesson, we're going to look at the six strategies for migrating applications to the cloud: **rehosting**, **replatforming**, **repurchasing**, **refactoring**, **retiring**, and **retaining**.

### Cloud Adoption Strategies: Rehosting

- **Rehosting** is also known as the "lift-and-shift" method.
- Most applications are rehosted since the organization is looking to scale its migration quickly to meet a certain business case. A common example is Microsoft SharePoint.
- Most rehosting can be automated with tools provided by Amazon Web Services.
    - Some customers still prefer to do this manually as they learn how to apply their legacy systems to the new cloud platform.
        
        For example, a legacy call center to a new cloud call center or legacy service desk to a new cloud service desk. 
        
- Many applications are easier to optimize and rearchitect once they are already running in the cloud.

### Cloud Adoption Strategies: Replatforming

The second strategy is replatforming. 

- This is sometimes called "lift-tinker-and-shift."
- The customer might make a few cloud (or other) optimizations to achieve some tangible benefits with replatforming.
- Otherwise, they are not changing the core architecture of the application.
    - Examples to be explored later in this training will be migrating to a Database as a Service (DBaaS) platform like Amazon Relational Database Service (Amazon RDS) or migrating an application to a fully managed platform like Amazon Elastic Beanstalk for software development.

### Cloud Adoption Strategies: Repurchasing

- This strategy involves moving to a different product or vendor solution.
- A common example is moving to a Software as a Service solution for enterprise resource planning (ERP) or customer relationship management (CRM).

### Cloud Adoption Strategies: Refactoring

Next, we have refactoring, otherwise known as rearchitecting. 

- Refactoring would involve reimagining how the application is architected and developed, often using cloud-native solutions.
- A common use case is when a business must add features, scalability, or performance that would otherwise be challenging to achieve in the application's current server farm or data center environment on-premises.
- Refactoring is a more expensive option for organizations looking to migrate from a monolithic architecture to a service-oriented or serverless cloud environment to boost agility or improve continuity of operations.

### Cloud Adoption Strategies: Retiring

- The retiring option is when an application or service has reached the disposition phase because of
    - supply chain challenges,
    - end of life or end of support,
    - deprecated technology,
    - regulations or compliance,
    - or no more utility or usefulness.

### Cloud Adoption Strategies: Retaining

Cloud adoption strategy number six is retaining. 

- This typically means to "revisit" or do nothing for the foreseeable future.
- In other words, the company may be still "riding out" some of the depreciation.
- Another reason to retain is there is not a present inclination to migrate some applications until there are changes to the business cycle, socio-political factors, or additional resources in the budgets.
- Remember, the organization should only migrate what makes sense for the delivery of their value proposition.

### Cloud Adoption Resources

Let's look at some cloud adoption resources. 

- You can use AWS Professional Services — this is a global team of experts that can help customers realize their desired business outcomes.
- AWS Solutions Architects — these are certified cloud architects.
- AWS Activate for Startups — here AWS offers free templates, tools, resources, content, and expert support to accelerate your startup.
- AWS Knowledge Center — this helps answer the questions most frequently asked by AWS Support customers.
- AWS Compliance
- AWS Cloud Adoption Framework.

In the upcoming lesson, we'll do a cloud safari to Amazon Web Services and explore the Cloud Adoption Framework (CAF).

### Outlining the AWS Cloud Adoption Framework

[AWS Cloud Adoption Framework](https://aws.amazon.com/es/cloud-adoption-framework/)

All right, let's do a web safari up to Amazon Web Services and look at something that you’ll very likely get a question on the exam. [Video description begins] *AWS Cloud Adoption Framework page is displayed with a top menu, an introduction about AWS CAF, and several CTA buttons.* [Video description ends]

The AWS Cloud Adoption Framework or AWS CAF standing on the shoulders of giants, really using the experience and best practices of other people at Amazon Web Services to basically help you enhance and accelerate and transform your business by using Amazon Web Services. You will want to know on the exam that it breaks up its elements what are called six perspectives. And so, each one of these perspectives is a set of capabilities that basically allow you to focus on your cloud 
transformation process. So, if we go down here, we'll see. We have 
business, people, and governance. [Video description begins] *Under a section called Capabilities and Perspectives, there are six options, out of which three are titled: Business, People, and Governance.* [Video description ends]

- So, the business perspective helps you make sure that your cloud 
investments are being accelerated, your ambitions, your business  outcomes, you know, used by the C team or the C-suite.
- And then you see the people perspective, which is a kind of a synergy with technology and business accelerating your journey.
- And then governance. The governance perspective so you can automate and orchestrate your initiatives and maximize all of the capabilities.

So, we see the business, the people, and the governance is like the **strategic aspect**. So you have those three, which are the strategy [Video description begins] *The host scrolls down displaying the other three options labelled: Platform, Security, and Operations.* [Video description ends]

And if we come down here, we have three would be **the tactical**, right,

- platform perspective to build the enterprise-grade, scalable, hybrid cloud platform, modernization, leveraging new cloud-native solutions that would be used by your CTO, your chief technology officer.
- The security aspect, achieving confidentiality, integrity, availability, identity management, including non-repudiation.
- And then operations ensuring that your cloud services are delivered at an appropriate and efficient level.

So remember, we have six of these to remember for the exam. Business, people, and governance being the ***strategic***. Platform, security, and operations being the ***tactical***.

And then you can go, and you can assess your cloud readiness by going through this. Forty-seven different capabilities across all six perspectives. [Video description begins] *He scrolls down and points to a button labelled Assess your cloud readiness.* [Video description ends]

And then of course, we see the benefits:

- reducing your business risk,
- improving environmental, social, and governance performance (ESG)
- growing your revenue,
- and increasing operational efficiency. [Video description begins] *He scrolls down further showcasing the Benefits section.* [Video description ends]

So that is the AWS Cloud Adoption Framework (AWS CAF) with its six perspectives.

### Appropriate Cloud Migration Strategies

Realize on the cloud practitioner exam. When you look at appropriate migration strategies, it’s really a couple of fundamental concepts, it’s not a deep architectural view.

So, for many customers, a common strategy is to perform **database replication**. 

- This refers to the process of copying data from a primary database to one or more replica databases to improve data availability and system fault-tolerance and reliability.
- Database replication is usually a continual process happening in real-time as data is created, modified, used, shared, or deleted in the primary database.
    - It can also occur as a one-time event or through scheduled batch projects.

Some use cases for **data replication** at AWS would be when:

- customers can create tasks for ongoing replication using the AWS Database Migration Service (DMS).
- Data can be migrated to S3 object storage to match the organizational data life cycle.
- A newer solution would be to use Amazon Elastic File System (EFS) replication to create a replica of their EFS file system in the AWS Region of their choosing.
- AWS customers may decide to innovate and build new database applications with Amazon Relational Database Service (RDS).
    - For example, for their Oracle database or their Microsoft SQL 
    database.

Another migration strategy we refer to is **OOB or out-of-band**. 

- The **AWS Snowball** service offers secure, rugged devices that allow customers to transfer data into and out of AWS and bring AWS computing and storage capabilities to edge environments.
- These rugged devices are commonly referred to as AWS Snowball or AWS Snowball Edge.
- Previously, Snowball referred explicitly to an early hardware version of these devices, however that model has been replaced by updated hardware. Keep that in mind for this newer exam.
- The AWS Snowball service now operates with Snowball Edge devices, which include on-board computing capabilities as well as storage. [Video description begins] *A process loop diagram of AWS Snowball depicting the steps is displayed.* [Video description ends]

![image.png](attachment:3da9b364-052f-40a8-85ea-b01e3fff34a6:image.png)

Here’s how it works: 

1. If you want to use AWS Snowball, in the AWS Snow family management console, create a job and then choose your device.
2. AWS prepares and ships the device to you for arrival in approximately 4-6 business days. 
3. Then when the device arrives or devices, power it on, unlock it, and connect it to your local network.For example, your data center or your storage area network. 
4. Read or write the data to the device with the AWS OpsHub, NFS, or the built-in Amazon S3 adapter. 
5. When you’re ready, ship the device back to AWS; the e-link shipping label auto-updates for easy return.
6. Once it arrives at AWS, your data is transferred to your Amazon S3 bucket, verified, and then securely erased on the device. 
7. You can use the graphical interface the Snow family management console to track the progress of data migration plans. Or you can create a large data migration plan if necessary.

### Cost of On-premises Environments

A major value proposition and why AWS is so popular or cloud computing, in general, is the ongoing increasing costs of on-premises environments.

- On-premises costs can quickly be burdensome and prohibitive, especially in challenging economic environments such as inflation.
- These costs can range from upfront capital, for example, higher interest rates and borrowing costs to regular operational expenditures to keep that data center running.
- Customers are discovering the massive savings in labor costs and  other overhead by moving to the AWS cloud.
- Although capital expenditures like hardware, racks, and network equipment are a one-time purchase, they typically have a refresh cycle of about five years.
- Companies will amortize this for an accurate comparison.

Here we see three categories of on-premises costs: server costs, storage costs, and network costs. 

![image.png](attachment:591a6fdf-86c1-4bc2-ad11-9f9d4673fb33:image.png)

- With servers, we have server hardware, server blades, rack chassis PDUs, and ToR switches, plus the ongoing maintenance. On the server, we’re running software: operating system, and virtualization licenses (+ maintenance).
- Storage costs: we have storage disks, storage area networking switches and fiber channel switches possibly upgrading from a 10 gigabit to 100 gigabit network. And of course, storage software costs (+ maintenance).
- On the  network, we may have local area network switches, layer two and  multilayer switches and load balancers and the recurring costs of  Internet service providers and the bandwidth. And of course, in the facility, we have space, power, and cooling for servers including hypervisors, the storage area network, and the network infrastructure.

### Cost Savings to the Cloud

In this brief lesson, we'll look at the cost savings of moving to the cloud. 

- The value of the cloud or cloud proposition extends beyond total cost of ownership reduction.
- AWS customers also see substantial enhancements in other areas, including better productivity for their personnel, operational resilience, and corporate agility. The ability to respond quickly to new customers, new technologies, and the pressure from competitors.
- Amazon Web Services customers get an average cost savings of 31 
percent by migrating to the cloud.
- By moving to the cloud, organizations are achieving more IT competencies at a fraction of the cost.
- When commercial organizations increase their efficiency and savings, they free up profits to expand, modernize, and grow in new areas.
- And since the customer only pays for the cloud services they use, they can easily adapt to changing business demand.
    - For example, International Data Corporation (IDC) interviewed 41 organizations globally and reported that AWS helped customers accelerate growth, drive efficiencies, and realize vital long-term cost reductions.

It's important as a candidate for the AWS cloud practitioner that you understand from AWS’ standpoint, they are the leader offering: 

- an average 10 months to pay back,
- nearly 2.3x more new features are delivered,
- $66.3M additional revenue per year per organization in US dollars,
- 47% more efficient IT infrastructure staff, and 50% lower 5-year cost of operations.

### Fixed Costs vs. Variable Costs

Let's compare fixed costs vs. variable costs. 

- The cloud allows customers to trade fixed expenses or capital expenditures for variable expenses and only pay for IT (Information Technology) as they consume it.
- Due to the economies of scale, the variable expenses are much lower than what organizations would pay to do it themselves.
- Whether it is a startup in the cloud, for example, a group of programmers who just graduated from university and want to develop mobile apps or do blockchain smart contracts, or you’re just starting the migration journey to the cloud, AWS has a set of solutions to help manage and optimize your expenditures.

Here's some examples of fixed cost vs. variable cost. 

| Fixed cost | Variable cost |
| --- | --- |
| data centers and server farms.  For example, an on-premise SharePoint server farm. | virtual instances of Windows and Linux. And don’t forget macOS.  |
| Physical blade servers and racks | serverless solutions like Functions as a Service, specifically AWS Lambda |
| storage area networks (SAN) | relational database services in the cloud |
| buildings, HVAC, and environmental controls | elastic file services |

By using the AWS cloud and variable costs, we can create a superior environment as opposed to the cost of on-premises environments. 

- For example, we can **plan & evaluate** with the migration evaluator, AWS pricing calculator, and AWS budgets.
- We can **manage and control** our identity and access management with AWS IAM or the Identity Center.
    
    We can use the billing console, AWS purchase order management, AWS budget actions, and AWS cost anomaly detection. 
    
- We can **see** by **organizing and reporting** through the AWS Cost Explorer, the AWS cost & usage reports, cost categories, and the AWS application cost profiler.
- And we can **optimize and save** with savings plans, reserved instances, rightsizing which we’ll define later on in this course, and recommendations.

### Examining AWS Licensing Strategies

In this lesson, we're going to talk about licensing options in the cloud, and we're going to focus on two things. 

First, Microsoft licensing on AWS. Because Linux and macOS are open 
source, we don't have the same considerations. We'll also talk about the licensing manager.

[Microsoft Licensing](https://aws.amazon.com/windows/resources/licensing/)

You have a lot of choices here with Microsoft. When you instantiate an Elastic Compute Cloud (EC2) instance or a relational database license-included instance, you're going to get a fully compliant Windows Server. And in the case of RDS with Microsoft SQL, you get a SQL Server license directly from AWS. 

And you can manage all of this through the AWS License Manager, which makes it easy to change license types between AWS provided licenses, where they’re included and what’s called BYOL, which you must know on the exam stands for **bring-your-own-license**. 

So you can buy licenses from AWS using the included instances when you spin it up based on the Amazon Machine Image that also includes the platform that’s running on it, for example, Microsoft SQL Server.

Whether doing Infrastructure as a Service through EC2 or using Amazon RDS for SQL Server, AWS manages the licensing compliance, they support 
current and other legacy versions as well. And remember, Windows Server Client Access Licenses (CALs) are not required. Keep that in mind on the exam. 

- You can bring your license to AWS. This is called BYOL. Remember, it is subject to the Microsoft licensing terms, however, here you can leverage
    - the efficiencies of the AWS Cloud using your own existing perpetual license,
    - you can extend the lifecycle of your software without additional costs,
    - and you can expedite the migration to the cloud using existing virtual machine images.

You have two options with BYOL. 

- You can do BYOL without software assurance, or
- you can do BYOL with software assurance, and that would be Microsoft License Mobility through Software Assurance, which allows 
many software licenses to be transferred into the AWS Cloud for use with Amazon EC2.

Remember, when you purchase an Amazon EC2 instance with a Windows Server-Based AMI, or an Amazon RDS for SQL Server license included instance, Amazon will take care of all the cost and compliance for you.

Also, Microsoft includes two Microsoft RDP or Remote Desktop Services licenses for administrative purposes. 

Here, we see a list of eligible products covered by the Microsoft 
Product Terms as of September of 2023. This list may change, but you may want to look at it for your reference. This will not be on the exam. 

Let’s look at the AWS License Manager. Here, you can manage your 
software licenses and fine-tune your licensing costs. 

[Software de administración de licencias - Amazon License Manager – AWS](https://aws.amazon.com/es/license-manager/)

![image.png](attachment:8e9c4e93-d2c2-46ca-93e3-9f530cd3528f:image.png)

Here's how it works: Basically, the AWS License Manager, you:

- define the rules for your license software,
- you attach licensing rules during launch and proactively control the usage,
- you can search the inventory and track licenses brought in post launch,
- and you can use alerts to control and centrally manage licenses across all AWS accounts including on premises.

License manager makes it easy and smooth for you to manage your 
software licenses from vendors like Microsoft, SAP, Oracle, IBM and 
others in your AWS environment or your hybrid cloud environment.

### The Right Sizing Concept

Let's go ahead and define the right sizing concept. 

- Right sizing is the practice of mapping instance types, for example, Amazon Linux running on T2 micro and different sizes to workload performance and capacity requirements at the lowest feasible cost.
- Right sizing is also the process of observing deployed instances and recognizing openings to eradicate or downsize without compromising capacity or other requirements, which results in lower costs. We would call this due care or ongoing operational excellence.

Rightsizing for optimization:

- Right sizing is a key mechanism for optimizing AWS costs. It is often overlooked by organizations when they first transfer to the AWS Cloud. After all, they have so many other priorities and operational responsibilities, and they fail to emphasize the importance of right sizing.
- Often companies will lift and shift their environments and expect to right size later and then they never get around to it.
- Another reason is that speed and performance are frequently prioritized over cost, which results in oversized instances and a lot of squandered spending on idle resources. And remember, it’s not an Amazon Web Services’ best interest for their customers to overspend or oversize. They want to keep you for the long run.

Right sizing is an Ongoing Task:

- Right sizing is the most effective way to manage costs in the cloud, and it's an ongoing task.
- It involves persistently analyzing instance performance and usage needs and patterns. And you can use tools from AWS or from the third party AWS marketplace.
    - For example, turning off idle instances and right sizing instances that are either overprovisioned or below par when matched to workloads.
- And since resource needs are constantly changing, right sizing must be a constant task to continually optimize costs.
- Right sizing can be a tight process by establishing a schedule for 
each team, placing tags on all instances, and taking advantage of the aforementioned tools that AWS and partners offer to streamline resource monitoring and analysis.

### Course Summary

![image.png](attachment:02b59af9-8bde-4fb9-93a7-5f0fdf6a4c05:image.png)

![image.png](attachment:1426ddda-141b-465a-9cfb-761532a7cde9:image.png)

![image.png](attachment:b21fc85e-f21a-4e18-91a3-b8d3c23eb5fe:image.png)

![image.png](attachment:7ebfc4ad-03a6-4714-9be9-f6708f8a87e6:image.png)

## AWS Cloud Practitioner: Automation & Managed Services

### Course Overview

Automation and managed services.It is an established fact that when an organization can remove human error from its infrastructure configuration, the environment will be more consistent, secure, and optimized. Automation and orchestration are vital services in the cloud.

Learning objectives for this course will be:

- To outline the benefits of automation in the AWS cloud.
- To describe
    - Amazon Relational Database Service (RDS),
    - Amazon Elastic Container Service (Amazon ECS),
    - Amazon Elastic Kubernetes Service (Amazon EKS),
    - Amazon DynamoDB,
    - AWS Lambda,
    - and Amazon Simple Storage (S3).

### Benefits of Automation

Let's begin this course looking at the benefits of automation.

- A beneficial mental image for automation through Infras**tructure as Code** or IAC, is to imagine an architect’s drawing actually coming to life in two dimensions or even three dimensions.
- Just as a blueprint with walls, doors, and windows can be converted into a real  brick-and-mortar building, so too can load balancers, databases, or network infrastructure be written in source code and then instantiated (or terraformed).
- Contemporary monolithic or container based architectures benefit greatly from infrastructure-level automation.
- With virtual machines, IT teams can easily replicate environments, and create stacks and templates of operating system states, to use as they need.
- The host operating system became immutable and disposable, and with cloud computing the idea exploded and scale was added to the solution.
- There's no need to predict the future when you can simply provision on demand for what you need, and pay for what you use.

Organizations can also automate compliance in the cloud. 

- By introducing compliance requirements early in the product or service life cycle, customers can ensure that they address policy and regulation objectives while improving their value proposition, whether it be a product or a service.
- Automating compliance in the cloud has three benefits.
    - There's an immediate cost savings.
    - Shifting workloads to the cloud, logically encourages greater automation,
    - and when the automated process identifies a problem, the remediation can be much easier to deploy.

Automation in AWS:

- Automation in AWS emphasizes the setup, configuration, deployment,  and support of infrastructure and the applications that run on it.
- By leveraging automation tools, customers of AWS can roll out environments more quickly in a standardized, consistent, and repeatable way.
- The removal of manual processes is a critical success factor (CSF) in an effective DevOps strategy.
- And the main service for automation and Infrastructure as Code in AWS, is AWS CloudFormation.

Here’s eight reasons to use AWS’ Infrastructure as Code CloudFormation service:

- It's a free and managed service.
- Human errors and configuration errors can be avoided.
- The architecture code is kept in your repository.
- You can create environments with re-usable templates.
- Costs are reduced by deleting unused stacks and re-creating them later.
- It’s easy to learn with YAML, Yet Another Markup Language, or JSON, JavaScript Object Notation Language.
- The templates are self-explanatory.
- And finally, it's integrated with practically all AWS services.

### Amazon Relational Database Services (RDS)

Alright. Let’s do a quick survey of the AWS Relational Database Service. 

We could go to the Splash page, but I’m going to go ahead and go into the Amazon RDS Dashboard.

Remember, on the exam there is no configuration. So by no means will 
you have to memorize anything here. But notice that we’re using the 
following RDS resources, so far none. But we’re in the US East (N. Virginia) region.

Let's come down here where it says create a database. 

You have a couple of options. 

- You can go with a Standard create where we can set all the configuration options, we can do our availability settings, security, backups, and maintenance,
- or they have an Easy create option. This is the recommended best practice configurations.

But you can always change them, of course, after the fact. 

On the exam, it's important to realize that the RDS service is going to support **five different platforms**. 

- So on the CLF-C02 exam, they have two types of questions. Several questions that have five possibilities, and you have to choose two of the five possibilities.
    
    ![image.png](attachment:1e1a5608-8c56-4fdd-b1ef-46f337f71bec:image.png)
    
    So looking at this right here, this looks pretty prototypical of what you might see on the exam. For example, we’re going to talk more about Amazon Aurora.
    
    But if they ask you which two of these five platforms are supported by Amazon Aurora, the two correct answers would be **MySQL** and **PostgreSQL**. You can also see that they support MariaDB, Oracle, and Microsoft SQL Server. 
    

So for most of you early practitioners, you’d want to do the **Easy create** option, and then go down and choose one of these options.

Remember, this is still a managed platform as a service offering if you choose MariaDB, or Oracle, or Microsoft SQL Server. But Aurora offers what we call fully-managed.

Then you can go down and you can choose your DB instance size.

![image.png](attachment:ff905ee7-b6d1-4184-a024-c2f7cf7804cd:image.png)

- Probably beginning with the Dev/Test option as opposed to the Production option.

Create a name for your DB cluster and then a Master username, which 
would be the ID of the master user of your database instance. 

And you can have them Auto generate a password for you right there.

If you want to, you can set up an EC2 connection after creating the 
database and of course finally viewing the default settings for easy 
create would be right here.

As I mentioned, there's no configuration on this exam, but you 
definitely want to know the five different platforms that are supported by Amazon RDS.

### Amazon Elastic Container Service (ECS)

Containers are a very popular way to develop applications at Amazon Web Services. Whether you use Agile or CI/CD as your development life cycle, it's very likely you're developing with containers.

But before we look at the different services offered at AWS, let's define what containers are.

- It’s a standard unit of software that packages code and all of its 
dependencies.
- And the application can run rapidly and reliably from one computing environment or platform to another.
    - For example, from Windows to macOS to Linux.
- A container image is a lightweight, standalone, executable bundle of software that comprises everything necessary to run an application, including the code, the runtime environment, system tools, libraries, dependencies, and settings.
- Container images become containers at runtime and often when they run on an engine.

Containers at AWS:

- As mentioned, containers are a key component of modern app 
development.
- They have become the standard way to organize, compute resources, and manage the content of your application deployments.
- Containers provide a discrete reproducible compute environment.
- They also provide a way to simplify packaging and dependency management.

Amazon Elastic Container Service (ECS):

- Amazon ECS is a fully managed container orchestration service that 
streamlines the customer’s deployment, management, and scaling of 
containerized applications.
- The developer simply describes their application and the resource required in the ECS service.
- Amazon ECS will launch, watch, and scale the application along with 
the elastic compute options.
- ECS also provides automatic integration with other supporting AWS services that the application needs.
    - For example, AWS Fargate.
- Customers can
    - conduct system operations in ECS.
    - generate custom scaling and capacity rules.
    - monitor and query data from application logs and telemetry.

Here, we can see how ECS works from either the developer or the 
operations standpoint. In other words, DevOps. 

![image.png](attachment:fd670652-e666-4e32-93b7-993ba6e4716f:image.png)

- From the developer standpoint, you describe your application and the resources it needs and then let Amazon ECS take over from there.
- Operators can create custom scaling and capacity rules and observe and query telemetry and logs from running applications.

Both developers and operators are inputs into the ECS service. 

Services that are used for deployments and scaling would be AWS Fargate or serverless containers. 

Amazon EC2, for example running on Graviton or Intel processors.  There’s also Amazon ECS Anywhere for hybrid computing. With AWS Outposts, you can deploy to AWS Local Zones in metropolitan areas or for 5G leverage AWS Wavelength.

All of these services can send application telemetry back to ECS and then back to the operators.

Another important tool with ECS is the Amazon Elastic Container  Registry or ECR. Here you can build and store container images using  Amazon ECR or another container registry. For example, GitHub.

And notice that ECS has automated integration with Elastic Load Balancing, Amazon Elastic File System, and the AWS Secrets Manager for configuration purposes.

### Amazon Elastic Kubernetes Service (Amazon EKS)

Amazon Elastic Kubernetes Service (Amazon EKS)

- AWS customers can choose between two fully managed container services: Amazon’s ECS or the Amazon EKS for Kubernetes.
- Both services support a wide-ranging assortment of compute options. They have strong integration with other AWS services and they offer the global scale and reliability that customers have come to expect from Amazon Web Services.
- Amazon EKS is a managed Kubernetes service to operate Kubernetes container orchestration in the AWS cloud and on-premises data centers.
- In the cloud, EKS automatically controls and manages the availability and scalability of the Kubernetes control plane nodes that:
    - schedule containers such as Docker and Podman.
    - Manage application availability,
    - store cluster data
    - and conduct other key tasks for cloud developers.
- With Amazon EKS, customers can utilize all of the performance, scaling, availability, reliability, and durability of the AWS infrastructure.
- They can interoperate with AWS networking and security services.
- On-premises, EKS provides a dependable, fully-supported K8 or Kubernetes solution with integrated tooling and fundamental deployment to hybrid cloud sites, virtual machines, or bare metal servers.

![image.png](attachment:83daf2a1-670b-4bd6-afbd-d7ea27c6e8e5:image.png)

First you would create your Kubernetes clusters. This is powered by Amazon EKS Distro.

Then you can transport those to AWS Fargate to deploy serverless containers or to EC2 to deploy worker nodes for your EKS cluster. 

For example, on Windows Server 22 or Red Hat enterprise.

Then run your Kubernetes apps and then view and explore running Kubernetes apps in the AWS EKS dashboard in the AWS console.

### Surveying Amazon DynamoDB

### Surveying AWS Lambda

### Examining Amazon Simple Storaga Servie (S3)

### Course Summary