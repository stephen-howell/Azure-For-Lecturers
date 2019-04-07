# Azure for Lecturers

## Introduction 
Azure for Lecturers is a short (two-hours-ish) tutorial for lecturers on getting started using and teaching Azure.  
Assumes no particular cloud experience but does assume familiarity with coding and that you probably have a CS degree somewhere in your educational history.

## Table of Contents
1. Introduction to Microsoft Azure
1. What is Cloud Computing 
1. IaaS, PaaS, serverless, and SaaS
1. Activating your academic account on Azure
   1. Creating a Resource Group
1. Compute (*Virtual Machines*)
1. Databases (*SQL Database*)
1. Compute (*App Service* & *Web App Service*) 
1. Containers (*Azure Functions*)
1. AI + Machine Learning

## Introduction to Microsoft Azure

Microsoft Azure [https://azure.microsoft.com/](https://azure.microsoft.com/) is a suite of services and technologies that share the fact they are hosted in Microsoft data centres. The closest Microsoft to Ireland is in Dublin and this DC is classified as 'North Europe'.
There is a wide range of services, and we will only cover a few today. 

Here is the list of *categories* of services (each can have a dozen services):
1. AI + Machine Learning
1. Analytics
1. Compute
1. Containers
1. Databases
1. Developer Tools
1. DevOps
1. Identity
1. Integration
1. Internet of Things
1. Management and Governance
1. Media
1. Microsoft Azure Stack
1. Migration
1. Mixed Reality
1. Mobile
1. Networking
1. Security
1. Storage
1. Web

Some of these are only used by certain specialised roles, but often a complex will mix and match services that it needs from many different sections, for instance, a common and simple pattern would be:
1. Web App from Compute
1. SQL Database from Databases
1. Azure Active Directory authentication from Security
1. Notification Hubs from Web

It's really hard to know all categories and services in depth. To make it harder, they are often updated, so there is a bit of constant learning needed when using cloud services. Luckily there are rarely huge changes that break existing systems, and if there are, they are highlighted in advance.

## What is Cloud Computing?
A good [beginner's guide](https://azure.microsoft.com/en-us/overview/what-is-cloud-computing/) is available and the short, non-techie answer to *What is Cloud Computing* is:
> Simply put, cloud computing is the delivery of computing services—servers, storage, databases, networking, software, analytics, intelligence and more—over the Internet (“the cloud”) to offer faster innovation, flexible resources, and economies of scale. You typically pay only for cloud services you use, helping lower your operating costs, run your infrastructure more efficiently, and scale as your business needs change.

Looking at the change in the graduate role requirements and the transition of most software developing companies (from startups to enterprises) to *Cloud First* being the increasingly  defacto way of developing software, your graduates need to be comfortable with it.

For us, Cloud Computing makes it easier to teach certain modules on a typical CS degree:
1. Cloud reduces the setup and configuration headaches for IT Services staff and lecturing staff
1. Easier for students to deploy (and lecturers examine) student assignments

What's the catch? Well, cloud services cost money. Students and lecturers can get $100 free Azure a year, which will suffice for a lot of modules, though lectures who require heavy use may need to request IT services purchase a set amount for them to teach a course. We recommend students are taught how to monitor and manage their costs in the first lecture of any cloud module. Share this with students to avoid the *'I've used up all my Azure, can you give me more'* conversations: [Pricing Calculator](https://azure.microsoft.com/pricing/calculator/).

### Benefits of Cloud Computing
From [https://azure.microsoft.com/en-us/overview/what-is-cloud-computing/](https://azure.microsoft.com/en-us/overview/what-is-cloud-computing/)

**Cost**: Cloud computing eliminates the capital expense of buying hardware and software and setting up and running on-site datacenters—the racks of servers, the round-the-clock electricity for power and cooling, the IT experts for managing the infrastructure. It adds up fast.

**Speed**: Most cloud computing services are provided self service and on demand, so even vast amounts of computing resources can be provisioned in minutes, typically with just a few mouse clicks, giving businesses a lot of flexibility and taking the pressure off capacity planning.

**Global scale**: The benefits of cloud computing services include the ability to scale elastically. In cloud speak, that means delivering the right amount of IT resources—for example, more or less computing power, storage, bandwidth—right when it’s needed, and from the right geographic location.

**Productivity**: On-site datacenters typically require a lot of “racking and stacking”—hardware set up, software patching, and other time-consuming IT management chores. Cloud computing removes the need for many of these tasks, so IT teams can spend time on achieving more important business goals.

**Performance**: The biggest cloud computing services run on a worldwide network of secure datacenters, which are regularly upgraded to the latest generation of fast and efficient computing hardware. This offers several benefits over a single corporate datacenter, including reduced network latency for applications and greater economies of scale.

**Security**: Many cloud providers offer a broad set of policies, technologies, and controls that strengthen your security posture overall, helping protect your data, apps, and infrastructure from potential threats.

### Types of cloud computing
Not all clouds are the same and not one type of cloud computing is right for everyone. Several different models, types, and services have evolved to help offer the right solution for your needs.

Types of cloud deployments: **public**, **private**, and **hybrid**

First, you need to determine the type of cloud deployment, or cloud computing architecture, that your cloud services will be implemented on. There are three different ways to deploy cloud services: on a public cloud, private cloud, or hybrid cloud.

**Public cloud**: Public clouds are owned and operated by a third-party cloud service providers, which deliver their computing resources like servers and storage over the Internet. Microsoft Azure is an example of a public cloud. With a public cloud, all hardware, software, and other supporting infrastructure is owned and managed by the cloud provider. You access these services and manage your account using a web browser.

**Private cloud**: A private cloud refers to cloud computing resources used exclusively by a single business or organization. A private cloud can be physically located on the company’s on-site datacenter. Some companies also pay third-party service providers to host their private cloud. A private cloud is one in which the services and infrastructure are maintained on a private network.

**Hybrid cloud**: Hybrid clouds combine public and private clouds, bound together by technology that allows data and applications to be shared between them. By allowing data and applications to move between private and public clouds, a hybrid cloud gives your business greater flexibility, more deployment options, and helps optimize your existing infrastructure, security, and compliance.

## IaaS, PaaS, serverless, and SaaS
Most cloud computing services fall into four broad categories: infrastructure as a service (IaaS), platform as a service (PaaS), serverless, and software as a service (SaaS). These are sometimes called the cloud computing stack because they build on top of one another. Knowing what they are and how they’re different makes it easier to accomplish your business goals.

**Infrastructure as a service (IaaS)**: The most basic category of cloud computing services. With IaaS, you rent IT infrastructure—servers and virtual machines (VMs), storage, networks, operating systems—from a cloud provider on a pay-as-you-go basis. 

**Platform as a service (PaaS)**: Platform as a service refers to cloud computing services that supply an on-demand environment for developing, testing, delivering, and managing software applications. PaaS is designed to make it easier for developers to quickly create web or mobile apps, without worrying about setting up or managing the underlying infrastructure of servers, storage, network, and databases needed for development. 

**Serverless computing**: Overlapping with PaaS, serverless computing focuses on building app functionality without spending time continually managing the servers and infrastructure required to do so. The cloud provider handles the setup, capacity planning, and server management for you. Serverless architectures are highly scalable and event-driven, only using resources when a specific function or trigger occurs.

**Software as a service (SaaS)**: Software as a service is a method for delivering software applications over the Internet, on demand and typically on a subscription basis. With SaaS, cloud providers host and manage the software application and underlying infrastructure, and handle any maintenance, like software upgrades and security patching. Users connect to the application over the Internet, usually with a web browser on their phone, tablet, or PC.

## Activating your academic account on Azure
Get an academic subscription here [https://azure.microsoft.com/en-us/free/free-account-students-faq/](https://azure.microsoft.com/en-us/free/free-account-students-faq/), you need to click the green **Activate** button and use your college email. Staff email should work. This is the only way to get free Azure without using a credit/debit card. 

Once that is complete, log into the Portal and check your subscription is active: 
1. Go to [https://portal.azure.com/](https://portal.azure.com/)
1. Click on Subscriptions on the left side-panel: [Subscriptions](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)
1. It should show the Subscriptions blade with your academic subscription

### Creating a Resource Group
Before we create anything, we need to create a *Resource Group*. Everything we create today will be part of the resource group, and this makes it easier to manage (e.g. if we had multiple separate projects, or modules to lecture, we can compartmentalise them). It will also make it easier to delete everything when we are finished.

To create a resource group, select the Resource groups icon in the Favorites on the left.

![Resource groups icon](https://user-images.githubusercontent.com/38020233/55686730-c6e0df00-595c-11e9-80a9-08c532d8ac71.png)

this will open the Resource groups blade. Now select the **+ Add** icon on the top.  
![+ Add icon](https://user-images.githubusercontent.com/38020233/55686755-132c1f00-595d-11e9-82da-b0fd92bb1368.png)

Now make sure the correct subscription is selected (in case you have two) and give a good meaningful name to your Resource group, for instance here I used AthloneIT because I was creating a Resource group for a demo in AthloneIT. You might use SecondYearDatabases or ThirdYearAppDevelopment if you teach a few modules. Finally, **ensure** you use *North Europe* as the Region. Otherwise you'll be adding an unnecessary delay to 

![image](https://user-images.githubusercontent.com/38020233/55686779-4c648f00-595d-11e9-90b6-50177e55df0e.png)

Hit Review and Create and the Create if you are happy with your choices. It will create the Resource group and when it's ready a popup will let you know:

![image](https://user-images.githubusercontent.com/38020233/55686857-46bb7900-595e-11e9-8c40-dd38c8a666e1.png)

I recommend you *Pin to Dashboard* but it's not essential, just handy.

## Compute (*Virtual Machines*)
Scenario: You want to teach students about virtual machines, containers, virtual networking and other infrastructure topics. Typically, a lot of VMs are created locally, and the local PCs have to be powerful enough (and have permissions) to host and execute the VM. Let's create two different VMs and connect to them.

### Creating a Linux VM
Select the Virtual machines favorite (not the classic) and open the VMs blade

![image](https://user-images.githubusercontent.com/38020233/55686899-c77a7500-595e-11e9-9688-b2bbc053fe06.png)

Fill in the settings - the main ones to ensure are:
1. Resource group is the one you created earlier (or the correct one if you have many)
1. Ensure region is North Europe
1. Pick any Linux image you like, I'm using Ubuntu
1. Remember the username and password!
1. The image size is only important if you **forget** to switch off the VM. If you use the cheapest one, Stndard B1s, as I have here, and leave it on all month, it will cost 7 euro or so. I'll be leaving it on for a few minutes, so it will only cost a few cents (0.0095 EUR/hr).

![image](https://user-images.githubusercontent.com/38020233/55686950-54bdc980-595f-11e9-8a03-897f60006006.png)

I also changed the Disks setting for OS Disk Type to Standard HDD. It's slow but I don't need fast for this VM.

![image](https://user-images.githubusercontent.com/38020233/55687093-d530fa00-5960-11e9-9138-be5243159b29.png)

Other useful things to do - Enable auto-shotdown on the VM in *Management*

![image](https://user-images.githubusercontent.com/38020233/55687111-19bc9580-5961-11e9-9755-47f859622e40.png)

Notice we haven't set any networking rules allowing us to connect to the VM once it is created, we could do that here but we'll add them later.

Select Review and Create, it took 2 minutes 9 seconds to complete when I did this.

### Connecting to the Linux VM
Go to your dashboard, if you pinned the LinuxVM like I did it should say *Running* on the tile.  
Select it, and it opens the a blade showing several menus on the left and details on the right. We won't go through all of theseas  there's a fair few lectures here alone, but let's **Connect** to the VM (top left).

This will give us the connection details we need, the ssh connection string such as username@ip address. Unfortunately this won't work yet because we haven't opened the ssh port to connect from outside.



## Databases (*SQL Database*)


## Compute (*App Service* & *Web App Service*) 


## Containers (*Azure Functions*)


## AI + Machine Learning


