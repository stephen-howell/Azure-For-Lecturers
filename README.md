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

This will give us the connection details we need, the ssh connection string such as username@ip address. Unfortunately this won't work yet because we haven't opened the ssh port to connect from outside. Copy the code to connect by selecting the Copy to Clipboard icon.

![image](https://user-images.githubusercontent.com/38020233/55687509-77eb7780-5965-11e9-9e89-a469ab1d80a9.png)

You can use any ssh client you like to connect to the VM of course, but if you have Windows 10 version 1803 (April 2018) or later, it's built in to Windows now. Alternatively, download and use putty.exe or whatever client you have in the college image.
To use Windows 10 ssh:
1. Windows key + R => cmd => enter
1. paste the ssh connection code from your own VM (it will be something like username@ip) => enter
1. Not surprisingly, it doesn't connect because we haven't enabled external public connections
1. Go back to Azure portal, select *Networking* from the *Settings* in the VM

![image](https://user-images.githubusercontent.com/38020233/55687537-ddd7ff00-5965-11e9-9195-f2258311ebd7.png)

Find the **Add inbound port rule** button and:
1. Add a *Destination port* of 22 for ssh
1. Click Add

![image](https://user-images.githubusercontent.com/38020233/55687570-44f5b380-5966-11e9-94b5-f0b1bb4a618e.png)

Now try ssh again and you should be prompted for a password. Enter it and you are logged into your Linux VM!

If you know Python, try this:
Create and edit a new Python file: nano test.py
```
nums = range(-10, 10, 2)
for i in nums:
        print(i)
```
Save with CTRL+O and exit with CTRL+X

Run the file with: python test.py

Remember to stop the VM when finished using it.

### Creating a Windows VM
This is very similar process, but slightly different ways to connect to the VM.
1. Create the VM, select same options (though a different name) and **Image** as *Windows 10 Pro 1809* (it is possible that depending on your subscription, some images from third party companies are not available to you)
1. I selected Standard D2s v3 as it costs 0.09 EUR/Hr and has 8 gigs of RAM, but you can select anything as long as you remember to switch it off
1. Allow **Public inbound ports** this time, select RDP

Took 6 minutes 38 seconds to deploy for me. Go to the resource when it is finished for you.
1. Connect
1. Download RDP file
1. Open downloaded file with Remote Desktop (unless that is blocked in college network, which is possible)
1. Put in the username and password you configured earlier
1. Use Windows as normal

*Remember to switch off all VMs when you are finished*

## Databases (*SQL Database*)
SQL Database is a hosted enterprise database that is much cheaper than buying a CPU license and server yourself.
Let's create a database and connect to it with Java (or your choice of programming language).
The design is as follows:
1. You need a **Server**
1. Each server can have multiple **Databases**
1. Each database can have multiple **Tables**

Luckily, you can create the server with *Create new* when creating your first database.

![image](https://user-images.githubusercontent.com/38020233/55689322-05859200-597b-11e9-90f7-ed2be660ff80.png)

Note the Server name must be unique, so if the one you want is taken, add something to the name until it is unique. 

Because this is just for teaching, I selected a **Basic 100 MB** configuation (costs $5 a month, or €4.21)

Review and Create -> Create. Deployment for me took 2 minutes exactly.
Go to the resource and select *Query editor (preview)* and log in.
I used [Mockaroo.com](https://mockaroo.com/) to generate the following fake data:
```
create table Students (
	id INT,
	first_name VARCHAR(50),
	last_name VARCHAR(50),
	email VARCHAR(50),
	gender VARCHAR(50)
);
insert into Students (id, first_name, last_name, email, gender) values (1, 'Danyette', 'De Paoli', 'Danyette.De Paoli@athlone.edu', 'Female');
insert into Students (id, first_name, last_name, email, gender) values (2, 'Gilbertina', 'Pond', 'Gilbertina.Pond@athlone.edu', 'Female');
insert into Students (id, first_name, last_name, email, gender) values (3, 'Othella', 'Hendrickson', 'Othella.Hendrickson@athlone.edu', 'Female');
insert into Students (id, first_name, last_name, email, gender) values (4, 'Mikkel', 'Selburn', 'Mikkel.Selburn@athlone.edu', 'Male');
insert into Students (id, first_name, last_name, email, gender) values (5, 'Renae', 'MacNish', 'Renae.MacNish@athlone.edu', 'Female');
insert into Students (id, first_name, last_name, email, gender) values (6, 'Archibaldo', 'Ousby', 'Archibaldo.Ousby@athlone.edu', 'Male');
insert into Students (id, first_name, last_name, email, gender) values (7, 'Gottfried', 'Scrooby', 'Gottfried.Scrooby@athlone.edu', 'Male');
insert into Students (id, first_name, last_name, email, gender) values (8, 'Mattie', 'McGinley', 'Mattie.McGinley@athlone.edu', 'Female');
insert into Students (id, first_name, last_name, email, gender) values (9, 'Whitney', 'Berntsson', 'Whitney.Berntsson@athlone.edu', 'Male');
insert into Students (id, first_name, last_name, email, gender) values (10, 'Lonee', 'Bilbery', 'Lonee.Bilbery@athlone.edu', 'Female');
```
for the Students table.
Also, the marks table, I generated the marks using Excel (as it's quick and easy).
```
create table Marks (
	id INT,
	moduleTitle VARCHAR(40),
	mark INT
);

insert into Marks (id, moduleTitle, mark) values (	1, 'Digital Media', 6);
insert into Marks (id, moduleTitle, mark) values (	2, 'Digital Media', 84);
insert into Marks (id, moduleTitle, mark) values (	3, 'Digital Media', 93);
insert into Marks (id, moduleTitle, mark) values (	4, 'Digital Media', 83);
insert into Marks (id, moduleTitle, mark) values (	5, 'Digital Media', 76);
insert into Marks (id, moduleTitle, mark) values (	6, 'Digital Media', 76);
insert into Marks (id, moduleTitle, mark) values (	7, 'Digital Media', 49);
insert into Marks (id, moduleTitle, mark) values (	8, 'Digital Media', 69);
insert into Marks (id, moduleTitle, mark) values (	9, 'Digital Media', 75);
insert into Marks (id, moduleTitle, mark) values (	10, 'Digital Media', 76);
insert into Marks (id, moduleTitle, mark) values (	1, 'Mathematics', 85);
insert into Marks (id, moduleTitle, mark) values (	2, 'Mathematics', 8);
insert into Marks (id, moduleTitle, mark) values (	3, 'Mathematics', 88);
insert into Marks (id, moduleTitle, mark) values (	4, 'Mathematics', 92);
insert into Marks (id, moduleTitle, mark) values (	5, 'Mathematics', 76);
insert into Marks (id, moduleTitle, mark) values (	6, 'Mathematics', 67);
insert into Marks (id, moduleTitle, mark) values (	7, 'Mathematics', 91);
insert into Marks (id, moduleTitle, mark) values (	8, 'Mathematics', 11);
insert into Marks (id, moduleTitle, mark) values (	9, 'Mathematics', 85);
insert into Marks (id, moduleTitle, mark) values (	10, 'Mathematics', 5);
insert into Marks (id, moduleTitle, mark) values (	1, 'Web Development', 74);
insert into Marks (id, moduleTitle, mark) values (	2, 'Web Development', 3);
insert into Marks (id, moduleTitle, mark) values (	3, 'Web Development', 85);
insert into Marks (id, moduleTitle, mark) values (	4, 'Web Development', 80);
insert into Marks (id, moduleTitle, mark) values (	5, 'Web Development', 95);
insert into Marks (id, moduleTitle, mark) values (	6, 'Web Development', 82);
insert into Marks (id, moduleTitle, mark) values (	7, 'Web Development', 14);
insert into Marks (id, moduleTitle, mark) values (	8, 'Web Development', 60);
insert into Marks (id, moduleTitle, mark) values (	9, 'Web Development', 67);
insert into Marks (id, moduleTitle, mark) values (	10, 'Web Development', 64);
insert into Marks (id, moduleTitle, mark) values (	1, 'Computer Applications', 14);
insert into Marks (id, moduleTitle, mark) values (	2, 'Computer Applications', 52);
insert into Marks (id, moduleTitle, mark) values (	3, 'Computer Applications', 78);
insert into Marks (id, moduleTitle, mark) values (	4, 'Computer Applications', 100);
insert into Marks (id, moduleTitle, mark) values (	5, 'Computer Applications', 70);
insert into Marks (id, moduleTitle, mark) values (	6, 'Computer Applications', 30);
insert into Marks (id, moduleTitle, mark) values (	7, 'Computer Applications', 38);
insert into Marks (id, moduleTitle, mark) values (	8, 'Computer Applications', 72);
insert into Marks (id, moduleTitle, mark) values (	9, 'Computer Applications', 66);
insert into Marks (id, moduleTitle, mark) values (	10, 'Computer Applications', 78);
insert into Marks (id, moduleTitle, mark) values (	1, 'Software Development', 91);
insert into Marks (id, moduleTitle, mark) values (	2, 'Software Development', 64);
insert into Marks (id, moduleTitle, mark) values (	3, 'Software Development', 58);
insert into Marks (id, moduleTitle, mark) values (	4, 'Software Development', 63);
insert into Marks (id, moduleTitle, mark) values (	5, 'Software Development', 7);
insert into Marks (id, moduleTitle, mark) values (	6, 'Software Development', 95);
insert into Marks (id, moduleTitle, mark) values (	7, 'Software Development', 27);
insert into Marks (id, moduleTitle, mark) values (	8, 'Software Development', 38);
insert into Marks (id, moduleTitle, mark) values (	9, 'Software Development', 47);
insert into Marks (id, moduleTitle, mark) values (	10, 'Software Development', 49);
insert into Marks (id, moduleTitle, mark) values (	1, 'Networks', 56);
insert into Marks (id, moduleTitle, mark) values (	2, 'Networks', 30);
insert into Marks (id, moduleTitle, mark) values (	3, 'Networks', 98);
insert into Marks (id, moduleTitle, mark) values (	4, 'Networks', 5);
insert into Marks (id, moduleTitle, mark) values (	5, 'Networks', 67);
insert into Marks (id, moduleTitle, mark) values (	6, 'Networks', 73);
insert into Marks (id, moduleTitle, mark) values (	7, 'Networks', 14);
insert into Marks (id, moduleTitle, mark) values (	8, 'Networks', 100);
insert into Marks (id, moduleTitle, mark) values (	9, 'Networks', 64);
insert into Marks (id, moduleTitle, mark) values (	10, 'Networks', 21);
insert into Marks (id, moduleTitle, mark) values (	1, 'Mobile Apps and Connected Devices', 98);
insert into Marks (id, moduleTitle, mark) values (	2, 'Mobile Apps and Connected Devices', 71);
insert into Marks (id, moduleTitle, mark) values (	3, 'Mobile Apps and Connected Devices', 68);
insert into Marks (id, moduleTitle, mark) values (	4, 'Mobile Apps and Connected Devices', 48);
insert into Marks (id, moduleTitle, mark) values (	5, 'Mobile Apps and Connected Devices', 87);
insert into Marks (id, moduleTitle, mark) values (	6, 'Mobile Apps and Connected Devices', 30);
insert into Marks (id, moduleTitle, mark) values (	7, 'Mobile Apps and Connected Devices', 57);
insert into Marks (id, moduleTitle, mark) values (	8, 'Mobile Apps and Connected Devices', 10);
insert into Marks (id, moduleTitle, mark) values (	9, 'Mobile Apps and Connected Devices', 61);
insert into Marks (id, moduleTitle, mark) values (	10, 'Mobile Apps and Connected Devices', 89);
insert into Marks (id, moduleTitle, mark) values (	1, 'Communications (Mobile Devices and Apps)', 77);
insert into Marks (id, moduleTitle, mark) values (	2, 'Communications (Mobile Devices and Apps)', 10);
insert into Marks (id, moduleTitle, mark) values (	3, 'Communications (Mobile Devices and Apps)', 62);
insert into Marks (id, moduleTitle, mark) values (	4, 'Communications (Mobile Devices and Apps)', 84);
insert into Marks (id, moduleTitle, mark) values (	5, 'Communications (Mobile Devices and Apps)', 34);
insert into Marks (id, moduleTitle, mark) values (	6, 'Communications (Mobile Devices and Apps)', 37);
insert into Marks (id, moduleTitle, mark) values (	7, 'Communications (Mobile Devices and Apps)', 24);
insert into Marks (id, moduleTitle, mark) values (	8, 'Communications (Mobile Devices and Apps)', 55);
insert into Marks (id, moduleTitle, mark) values (	9, 'Communications (Mobile Devices and Apps)', 2);
insert into Marks (id, moduleTitle, mark) values (	10, 'Communications (Mobile Devices and Apps)', 13);

```

Now, to add all the SQL above to the database, we'll use that query editor. Paste each query in (including the Create Table statement) and click Run. You should see 10 rows affected to create the students and 80 for the marks.

Now let's run some queries.
What is the average mark in Mathematics?
```
SELECT AVG(mark) as MathsAvg FROM Marks WHERE moduleTitle = 'Mathematics'
```

Show the names and marks in descending order for Networks:  
```
SELECT Marks.mark, Students.first_name, Students.last_name FROM Marks INNER JOIN Students ON Marks.id=Students.id WHERE Marks.moduleTitle = 'Networks' ORDER BY Marks.Mark DESC;
```

The best student in each subject

## Compute (*App Service* & *Web App Service*) 


## Containers (*Azure Functions*)


## AI + Machine Learning


