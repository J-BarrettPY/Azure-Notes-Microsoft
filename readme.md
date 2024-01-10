# Manage resources in Azure

## Azure solutions for public, private, and hybrid cloud

Imagine that you work at a healthcare company. You have legacy systems, line-of-business systems, and future plans for new systems. You've heard there are advantages to using cloud computing. How do you choose between public, private, or hybrid cloud environments to support your needs?

## What's cloud computing?
Cloud computing provides services and applications on demand over the internet. Servers, applications, data, and other resources are provided as a service.

To the user, the details of the services are abstracted. You can quickly provision computing resources and use the service with minimal management. You shouldn't think of cloud computing as a datacenter available through the internet. Cloud computing uses virtualization, commodity hardware, and automated processes to provide a self-service user experience to customers, similar to a public utility.

## Public cloud
Public clouds are the most common way to deploy cloud computing. Services are offered over the public internet and available to anyone who wants to purchase them. The cloud resources, such as servers and storage, are owned and operated by a third-party cloud service provider and delivered over the internet. Services might be free or sold on demand, allowing customers to pay only per usage for the CPU cycles, storage, or bandwidth they consume. Microsoft Azure is an example of a public cloud.

Let's imagine your healthcare company needs an enrollment website. The site needs to scale and be responsive during peak enrollment at various times during the year. Your customers access the site from global locations. You can use the public cloud to automatically scale up to meet demand at peak enrollment. When site traffic is low, your site can scale down to save costs. Your site is responsive at peak demand, and you only pay for more resources when needed. You can also deploy your website in multiple geographic regions to increase reliability and responsiveness.

During your website's development, developers want to create multiple development environments to speed their development process. Developers can use the public cloud to quickly provision virtual machines for sandboxed environments to develop a solution. When the developers no longer need an environment, they can delete it.

## Why public cloud?
Public clouds can be deployed faster than on-premises infrastructures and with an almost infinitely scalable platform. Every employee of a company can use the same application from any office or branch, using their device of choice, as long as they can access the internet.

Examples of why you'd use public cloud:

- Service consumption through on-demand or subscription model: The on-demand or subscription model allows you to pay for the amount of CPU, storage, and other resources that you use or reserve.
- No up-front investment in hardware: No requirement to purchase, manage, and maintain on-premises hardware and application infrastructure. The cloud service provider is held responsible for all management and maintenance of the system.
- Automation: Quickly provision infrastructure resources using a web portal, scripts, or automation.
- Geographic dispersion: Store data near your users or in desired locations without having to maintain your own datacenters.
- Reduced hardware maintenance: The service provider is responsible for hardware maintenance.

## Private cloud
A private cloud consists of computing resources used exclusively by users from one business or organization. It can be physically located at your organization’s on-site datacenter, or it can be hosted by a third-party service provider. The term private cloud shouldn't be considered a rebranding of traditional on-premises datacenters. A private cloud uses on-premises infrastructure and services to provide similar benefits of the public cloud. It uses an abstraction platform to provide cloud-like services such as Kubernetes clusters, or a complete cloud environment like Azure Stack. The organization is responsible for purchasing, configuring, and maintaining the hardware. Communication between the systems is usually on the network infrastructure that the business owns and maintains; for example, a private internal network or a dedicated fiber-optic connection between buildings.

Imagine you work at a healthcare company and you have an application that's in use at one of your datacenters. The operating environment can't be replicated in the public cloud. You have a new requirement to access data at another one of your datacenters. The database containing the data needs to remain at the other site because of regulatory compliance. This scenario is a private cloud. You have two datacenters your organization owns. You could use a public-cloud VPN over the internet to connect the datacenters. However, the scenario would be considered a private cloud, since the solution is private to the organization.

## Why private cloud?
A private cloud can provide more flexibility to an organization. Your organization can customize its cloud environment to meet specific business needs. Since resources aren't shared with others, high levels of control and security are possible. Also, private clouds can provide a level of scalability and efficiency.

Examples of why you'd use private cloud:

- Pre-existing environment: An existing operating environment that can't be replicated in the public cloud. A large investment in hardware and employees with solution expertise. A large organization can choose to commoditize their computing resources.
- Legacy applications: Business-critical legacy applications that can't easily be physically relocated.
- Data sovereignty and security: Political borders and legal requirements might dictate where data can physically exist.
- Regulatory compliance / certification: PCI or HIPAA compliance. Certified on-premises datacenter.

## Hybrid cloud
A hybrid cloud is a computing environment that combines a public cloud and a private cloud by allowing data and applications to be shared between them. When computing and processing demand fluctuates, hybrid-cloud computing gives businesses the ability to seamlessly scale their on-premises infrastructure up to the public cloud to handle any overflow without giving third-party datacenters access to the entirety of their data. Organizations gain the flexibility and computing power of the public cloud for basic and nonsensitive computing tasks, while keeping business-critical applications and data on-premises safely behind a company firewall.

Using a hybrid cloud helps eliminate the need to make up-front capital expenditures to handle short-term spikes in demand. It also has the flexibility to manage which resources are local versus resources in the cloud. Companies pay only for resources they temporarily use instead of having to purchase, program, and maintain extra resources and equipment that could remain idle over long periods of time. Integration is generally through a secure VPN between cloud providers like Azure and on-premises datacenters.

Imagine you work at a healthcare company and you have an application where customers can access their healthcare information. A regulation requires that the data needs to remain at a physical location. The customer website needs to be responsive to its many global users. As a solution, the database could be hosted in an on-premises datacenter, and the website could be hosted in the public cloud. You could use a VPN between the on-premises datacenter and the public cloud. This scenario would be considered a hybrid cloud.

## Why hybrid cloud?
A hybrid cloud allows your organization to control and maintain a private infrastructure for sensitive assets. It also gives you the flexibility to take advantage of extra resources in the public cloud when you need them. With the ability to scale to the public cloud, you pay for extra computing power only when needed. It can also ease transitioning to the cloud. You can migrate gradually by phasing in workloads over time.

Examples of why you'd use hybrid cloud:

- Existing hardware investment: Business reasons require that you use an existing operating environment and hardware.
- Regulatory requirements: Regulation requires that the data needs to remain at a physical location.
- Unique operating environment: Public cloud can't replicate a legacy operating environment.
- Migration: Move workloads to the cloud over time.

## Cloud service models

Cloud computing resources are delivered using three different service models:

- Infrastructure as a service (IaaS) provides instant computing infrastructure that you can provision and manage over the Internet.
- Platform as a service (PaaS) provides ready-made development and deployment environments that you can use to deliver your own cloud services.
- Software as a service (SaaS) delivers applications over the internet as web-based services.

-----------------------

## Infrastructure as a service

Infrastructure as a service (IaaS) is an instant computing infrastructure, provisioned and managed over the Internet. IaaS lets you quickly scale resources to meet demand and only pay for what you use. IaaS avoids the expense and complexity of buying and managing your own physical servers and other datacenter infrastructure. Each resource is offered as a separate service component, and you rent the resource as long as you need it.

As a result, IaaS is flexible. You can provision common infrastructure such as virtual machines (VMs), storage, virtual subnets, firewalls, and VPNs to build a solution. You don't need to manage physical servers and appliances. However, you're responsible for configuring and managing the components; for example, configuring firewalls, updating VM OS's, updating DBMS's, and runtimes.

## Common scenarios
Let's imagine your healthcare company needs to run a special version of desktop software. The software is only supported on a specific version of an operating system, and only one user license is required. You can create a VM with the required software. The user can use a remote desktop connection to connect to the VM to use the software.

Let's imagine another scenario. Your development teams need several unique development environments. Through the development cycle, they need to test various versions of the product. The developers can provision environments when needed. When an environment is no longer needed, your developers can easily delete it.

Some other common scenarios include:

**Website hosting**: If you want more control of hosting a website, running websites using IaaS might be a better option than traditional web hosting.

**Web apps**: IaaS provides all the infrastructure to support web apps, including storage, web and application servers, and networking resources. Organizations can quickly deploy web apps on IaaS and easily scale infrastructure up and down when demand for the apps is unpredictable.

**Storage, backup, and recovery**: Storage management can be complex, requiring a large capital investment and skilled staff to manage data and meet legal and compliance requirements. IaaS can help simplify planning, management, unpredictable demand, and steadily growing storage needs.

**High-performance computing**: If you have a workload that requires high-performance computing, you can run the workload in the cloud, thus avoiding the up-front cost of the hardware and only paying for the usage when needed.

**Big data analysis**: If you have large datasets that contain potentially valuable patterns, trends, and associations, IaaS can provide the processing power to mine data sets to locate patterns.

## Advantages
Eliminates capital expense and reduces ongoing cost: IaaS sidesteps the upfront expense of setting up and managing an on-site datacenter, making it an economical option for start-ups and businesses testing new ideas. As soon as you’ve decided to launch a new product or initiative, the necessary computing infrastructure can be ready in minutes or hours, rather than the days or weeks—and sometimes months—it could take to set up internally.

Improves business continuity and disaster recovery: Achieving high availability, business continuity, and disaster recovery is expensive, because it requires a significant amount of technology and staff. With the right service-level agreement (SLA) in place, IaaS can reduce this cost and access applications and data as usual during a disaster or outage.

Respond quicker to shifting business conditions: IaaS lets you quickly scale up resources to accommodate spikes in demand for your application—during the holidays, for example—then scale resources back down again when activity decreases to save money. Because you don’t need to first set up the infrastructure before you can develop and deliver apps, you can get them to users faster with IaaS.

Increase stability, reliability, and supportability: With IaaS, there’s no need to maintain and upgrade hardware or troubleshoot equipment problems. With the appropriate agreement in place, the service provider assures that your infrastructure is reliable and meets SLAs.

--------------------------

## Platform as a service

Platform as a service (PaaS) is a complete development and deployment environment in the cloud. With PaaS, you can build and deploy everything from simple cloud-based apps to sophisticated, cloud-enabled enterprise applications. You purchase the resources from a cloud service provider on a pay-as-you-go basis and access them over a secure internet connection.

Like IaaS, PaaS includes infrastructure such as servers, storage, and networking. In addition, it also includes middleware, development tools, and other services. PaaS supports the complete web-application lifecycle: building, testing, deploying, managing, and updating. PaaS removes the need to manage software licenses, middleware, and infrastructure of the services. You manage the applications and services you develop, and the cloud service provider typically manages everything else.

## Common scenarios
Let's imagine your healthcare company needs a website to describe a product. Your developers want to use PHP. Using PaaS, your developers have the option to create a web app. The infrastructure details such as creating a virtual machine, installing a web server, and installing middleware are abstracted away. You don't need to care on what operating system it runs or what physical hardware is required. Your developers deploy the website files to the cloud, and your website is available on the internet.

Let's imagine another scenario. Your company needs a SQL database to support data analysts for a special project. You don't have infrastructure to accommodate the request. You can quickly provision a SQL Server in the cloud that meets the project's needs. The data analysts can connect to the server. The SQL Server database is provided as a service. Therefore, you don't worry about updates, security patches, or optimizing physical storage for reads and writes.

Some other common scenarios include:

Development framework: PaaS provides a framework upon which developers can build to develop or customize cloud-based applications. Similar to the way you create an Excel macro, PaaS lets developers create applications using built-in software components. Cloud features such as scalability, high availability, and multitenant capability are included, reducing the amount of coding that developers need to do.

Analytics or business intelligence: Analysis tools provided as a service allows you to analyze and mine data. Organizations can find insights and patterns to predict outcomes to improve forecasting, product-design decisions, investment returns, and other business decisions.

## Advantages
PaaS has similar advantages as IaaS. However, PaaS has extra features, including middleware, development tools, and other business tools, that provide more advantages:

Reduced development time: PaaS development tools can reduce development time for new applications. Developers can use pre-coded application components built into the platform, such as workflow, directory services, security features, and search. PaaS components can give your development team new capabilities without you needing to add staff with the required skills.

Develop for multiple platforms: Some service providers give you development options for multiple platforms, such as desktop, mobile devices, and browsers, making cross-platform apps quicker and easier to develop.

Use sophisticated tools affordably: A pay-as-you-go model makes it possible for individuals or organizations to use sophisticated development software and business intelligence and analytics tools that they couldn't afford to purchase outright.

Support geographically distributed development teams: Because the development environment is accessed over the internet, development teams can work together on projects even when team members are at remote locations.

Efficiently manage the application lifecycle: PaaS provides all of the capabilities that you need to support the complete web application lifecycle: building, testing, deploying, managing, and updating within the same integrated environment.

-------------------------------

## Software as a service

Software as a service (SaaS) allows users to connect to and use cloud-based apps over the internet. Common examples are email, calendaring, and office tools like Microsoft 365. SaaS provides a complete software solution that you purchase on a pay-as-you-go basis from a cloud service provider. You can rent the use of an application for your organization. Your users connect to the service over the internet, usually with a web browser.

All of the underlying infrastructure, middleware, app software, and app data are located in the service provider’s data center. The service provider manages the hardware and software, and with the appropriate service agreement, ensures the availability and the security of the app and your data as well. SaaS allows your organization to get quickly up and running with an app at minimal upfront cost.

If you’ve used a web-based email service such as Outlook, Hotmail, or Yahoo! Mail, then you’ve already used a form of SaaS. With these services, you log into your account over the internet, often from a web browser. The email software is located on the service provider’s network, and your messages are stored there too. You can access your email and stored messages from a web browser on any computer or internet-connected device.

## Common scenarios
Let's imagine your healthcare company requires a customer relationship management (CRM) solution for its sales team. The team is global. You can use a SaaS CRM provider to quickly implement a solution for your organization's sales team.

For organizational use, you can rent productivity apps, such as email, collaboration, and calendaring, and sophisticated business applications such as CRM, enterprise resource planning (ERP), and document management. You pay for the use of these apps by subscription or according to the level of use.

## Advantages
Gain access to sophisticated applications: To provide SaaS apps to users, you don’t need to purchase, install, update, or maintain any hardware, middleware, or software. SaaS makes even sophisticated enterprise applications, such as ERP and CRM, affordable for organizations that lack the resources to buy, deploy, and manage the required infrastructure and software themselves. You pay only for what you use. You also save money, because the SaaS service automatically scales up and down according to the level of usage.

Use free client software: Users can run most SaaS apps directly from their web browser without needing to download and install any software. You don't need to purchase or deploy client software for your users.

Access app data from anywhere: With data stored in the cloud, users can access their information from any internet-connected computer or mobile device. Since app data is stored in the cloud, no data is lost if a user’s computer or device fails.

-----------------------------

# What is the Azure CLI?

The Azure CLI is a command-line program to connect to Azure and execute administrative commands on Azure resources. It runs on Linux, macOS, and Windows, and allows administrators and developers to execute their commands through a terminal or command-line prompt (or script) instead of a web browser. For example, to restart a virtual machine (VM), you'd use the following command:

```powershell
az vm restart -g MyResourceGroup -n MyVm
```
The Azure CLI provides cross-platform command-line tools for managing Azure resources, and you can easily install it locally on Linux, Mac, or Windows computers. You can also use the Azure CLI from a browser through the Azure Cloud Shell. In both cases, you can use it interactively or scripted. For interactive use, you'll first launch a shell (such as cmd.exe on Windows or Bash on Linux or macOS), then issue the command at the shell prompt. To automate repetitive tasks, you'll assemble the CLI commands into a shell script using the script syntax of your chosen shell, then execute the script.

## Using the Azure CLI in scripts
If you want to use the Azure CLI commands in scripts, you need to be aware of any issues around the "shell" (or environment) used for running the script. For example, in a Bash shell, you'll use this syntax when setting variables:

```bash
variable="value"
variable=integer
```
If you use a PowerShell environment for running Azure CLI scripts, you'll use this syntax for variables:
```powershell
$variable="value"
$variable=integer
```

You must install the Azure CLI before you can use it to manage Azure resources from a local computer. The installation steps vary for Windows, Linux, and macOS, but once installed, the commands are common across platforms.

## Work with the Azure CLI

The Azure CLI lets you type commands and execute them immediately from the command line. Recall that the overall goal in the software-development example is to deploy new builds of a web app for testing. Let's talk about the sorts of tasks you can do with the Azure CLI.

## What Azure resources can be managed using the Azure CLI?

The Azure CLI lets you control nearly every aspect of every Azure resource. You can work with resource groups, storage, virtual machines, Microsoft Entra ID, containers, machine learning, and so on.

Commands in the CLI are structured in groups and subgroups. Each group represents a service provided by Azure, and the subgroups divide commands for these services into logical groupings. For example, the `storage` group contains subgroups including account, blob, and queue.

So, how do you find the particular commands you need? One way is to use `az find`, the AI robot that uses the Azure documentation to tell you more about commands, the CLI, and more.

Example: find the most popular commands related to the word blob:

```powershell
az find blob
```

Example: Show me the most popular commands for an Azure CLI command group, such as az vm:

```powershell
az find "az vm"
```

Example: Show me the most popular parameters and subcommands for an Azure CLI command:

```powershell
az find "az vm create"
```

If you already know the name of the command you want, the `--help` argument for that command will get you more detailed information on the command and a list of the available subcommands for a command group. So, with our storage example, here's how you can get a list of the subgroups and commands for managing blob storage:

```powershell
az storage blob --help
```

## How to create an Azure resource

When you're creating a new Azure resource, there are typically three steps: connect to your Azure subscription, create the resource, and verify that creation was successful. The following illustration shows a high-level overview of the process.

## Connect

Because you're working with a local install of the Azure CLI, you'll need to authenticate before you can execute Azure commands by using the Azure CLI login command.

```powershell
az login
```

The Azure CLI will typically launch your default browser to open the Azure sign-in page. If this doesn't work, follow the command-line instructions and enter an authorization code at https://aka.ms/devicelogin.

After successfully signing in, you'll be connected to your Azure subscription.

## Create

You'll often need to create a new resource group before you create a new Azure service, so we'll use resource groups as an example to show how to create Azure resources from the CLI.

The Azure CLI group create command creates a resource group. You must specify a name and location. The name must be unique within your subscription. The location determines where the metadata for your resource group will be stored. You can use strings like "West US," "North Europe," or "West India" to specify the location; alternatively, you can use single-word equivalents, such as westus, northeurope, or westindia. The core syntax is:

```powershell
az group create --name <name> --location <location>
```

## Verify

For many Azure resources, the Azure CLI provides a list subcommand to view resource details. For example, the Azure CLI group list command lists your Azure resource groups. This is useful to verify whether the resource group was successfully created:

```powershell
az group list
```

To get a more concise view, you can format the output as a simple table:

```powershell
az group list --output table
```

-----------------------------

## What are resource groups?

Resource groups are a fundamental element of the Azure platform. A resource group is a logical container for resources deployed on Azure. These resources are anything you create in an Azure subscription, like virtual machines, Application Gateways, and Cosmos DB instances. All resources must be in a resource group, and a resource can only be a member of a single resource group. Many resources can be moved between resource groups, with some services having specific limitations or requirements to move. Resource groups can't be nested. Before you can provision any resource, you need a resource group in which to place it.

## Logical grouping

Resource groups exist to help manage and organize your Azure resources. By placing resources of similar usage, type, or location into resource groups, you can provide some order and organization to resources you create in Azure. Logical grouping is the aspect that you're most interested in here, because there's a lot of disorder among your company's resources.

## Lifecycle

If you delete a resource group, all resources contained within the group are also deleted. Organizing resources by lifecycle can be useful in non-production environments, where you might try an experiment and dispose of it when done. Resource groups make it easy to remove a set of resources at once.

## Authorization
Resource groups are also a scope for applying role-based access control (RBAC) permissions. By applying RBAC permissions to a resource group, you can reduce administration and limit access to allow only what's needed.

## Create a resource group
You can create resource groups by using the following methods:

- Azure portal
- Azure PowerShell
- Azure CLI
- Templates
- Azure SDKs (like .NET or Java)

## Use resource groups for organization

## Consistent naming convention

You can start with using an understandable naming convention. You named your resource group msftlearn-core-infrastructure-rg. You've given some indication of what it's used for (msftlearn), the types of resources contained within (core-infrastructure), and the type of resource it is (rg). This descriptive name gives us a better idea of what it is. If you had named it my-resource-group or rg1, you'd have no idea on a glance of what the usage may be. In this case, you can deduce that there are probably core pieces of infrastructure contained within. If you created more virtual networks, storage accounts, or other resources that the company might consider core infrastructure, you could also place them here to improve your company's resource organization. Naming conventions can vary widely between and even within companies, but some planning can help.

## Organizing principles
You can organize resource groups in a number of ways; let's take a look at a few examples. You might put all resources that are core infrastructure into this resource group, but you could also organize resources strictly by resource type. For example, you might put all virtual networks in one resource group, all virtual machines in another resource group, and all Azure Cosmos DB instances in another resource group.

## Organize for authorization
Because resource groups are a scope of RBAC, you can organize resources by who needs to administer them. If your database administration team is responsible for managing all of your Azure SQL Database instances, putting them in the same resource group simplifies administration. You could give the team the proper permissions at the resource-group level to administer the databases within the resource group. Similarly, the database administration team could be denied access to the resource group with virtual networks so they don't inadvertently make changes to resources outside their scope of responsibility.

## Organize for lifecycle
We previously described that resource groups serve as the lifecycle for the resources within them. If you delete a resource group, you also delete all the resources in the group. Use this to your advantage, especially in areas where resources are more disposable, like non-production environments. If you deploy 10 servers for a project that you know will only last a couple of months, you might put them all in a single resource group. One resource group is easier to clean up than 10 or more resource groups.

## Organize for billing
Lastly, placing resources in the same resource group is a way to group them for usage in billing reports. If you're trying to understand how your costs are distributed in your Azure environment, grouping them by resource group is one way to filter and sort the data to better understand where costs are allocated.

## Use tagging to organize resources

You've gone through your resources and moved them into resource groups that are more organized than before; but what if resources have multiple uses? How do you better search, filter, and organize these resources? Tags can be helpful as you look to improve organization of your Azure resources.

## What are tags?
Tags are name/value pairs of text data that you can apply to resources and resource groups. Tags allow you to associate custom details about your resource. In addition to the standard Azure properties, a resource has the following properties:

department (like finance, marketing, and more)
environment (prod, test, dev)
cost center
lifecycle and automation (like shutdown and startup of virtual machines)
A resource can have up to 50 tags. The name value is limited to 512 characters for all types of resources except storage accounts, which have a limit of 128 characters. The tag value is limited to 256 characters for all types of resources. Tags aren't inherited from parent resources. Not all resource types support tags, and you can't apply tags to classic resources.

You can add and manipulate tags through the Azure portal, Azure CLI, Azure PowerShell, Azure Resource Manager templates, and through the REST API. For example, to add a resource tag to a virtual network using the Azure CLI, you could use the following command:

```powershell
az resource tag --tags Department=Finance --resource-group msftlearn-core-infrastructure-rg --name msftlearn-vnet1 --resource-type "Microsoft.Network/virtualNetworks"
```

You can use Azure Policy to automatically add or enforce tags for resources your organization creates based on policy conditions that you define. For example, you could require that a value for the Department tag is entered when someone in your organization creates a virtual network in a specific resource group.

--------------------------------------

## Use policies to enforce standards

You're organizing your resources better in resource groups, and you've applied tags to your resources to use them in billing reports and in your monitoring solution. Resource grouping and tagging have made a difference in the existing resources, but how do you ensure that new resources follow the rules? Let's take a look at how policies can help you enforce standards in your Azure environment.

## What is Azure Policy?

Azure Policy is a service you can use to create, assign, and manage policies. These policies apply and enforce rules that your resources need to follow. These policies can enforce these rules when resources are created, and you can evaluate them against existing resources to give visibility into compliance.

Policies can enforce rules such as only allowing specific types of resources to be created or only allowing resources in specific Azure regions. You can enforce naming conventions across your Azure environment. You can also enforce that specific tags are applied to resources. Let's take a look at how policies work.

## Create a policy
You'd like to ensure that all resources have the Department tag associated with them and block creation if the tag doesn't exist. You'll need to create a new policy definition and assign it to a scope; in this case, the scope is our msftlearn-core-infrastructure-rg resource group. You can create and assign policies through the Azure portal, Azure PowerShell, or Azure CLI. This exercise takes you through creating a policy in the portal.

-------------------------------------

## Secure resources with role-based access control

Implementing Azure Policy ensured that all our employees with Azure access are following our internal standards for creating resources, but we have a second issue we need to solve: how do we protect those resources once they're deployed? We have IT personnel who need to manage settings, developers who need to have read-only access, and administrators who need to be able to control them completely. Enter Role-Based Access Control (RBAC).

RBAC provides fine-grained access management for Azure resources, allowing you to grant users the specific rights they need to perform their jobs. RBAC is considered a core service and is included with all subscription levels at no cost.

Using RBAC, you can:

- Allow one user to manage VMs in a subscription and another user to manage virtual networks.
- Allow a database administrator (DBA) group to manage SQL databases in a subscription.
- Allow a user to manage all resources in a resource group, such as VMs, websites, and virtual subnets.
- Allow an application to access all resources in a resource group.
To view access permissions, use the Access control (IAM) panel for the resource in the Azure portal. On this panel, you can determine who can access an area and their assigned role. Using this same panel, you can also grant or remove access.

## How RBAC defines access
RBAC uses an allow model for access. When you're assigned to a role, RBAC allows you to perform specific actions, such as read, write, or delete. Therefore, if one role assignment grants you read permissions to a resource group, and a different role assignment grants you write permissions to the same resource group, you will have both read and write permissions on that resource group.

## Best Practices for RBAC
Here are some best practices you should use when setting up resources:

- Segregate duties within your team and grant users only the amount of access that they need to perform their jobs. Instead of giving everybody unrestricted permissions in your Azure subscription or resources, allow only specific actions at a particular scope.
- When planning your access control strategy, grant users the lowest privilege level that they need to do their work.
- Use Resource Locks to ensure critical resources aren't modified or deleted (as you'll learn in the next unit).

## Use resource locks to protect resources

In a recent conversation, your manager mentioned that there had been instances where critical Azure resources were mistakenly deleted. Because there was disorganization across their Azure environment, good intentions of cleaning up unnecessary resources resulted in accidental deletions of resources critical to other systems. You've heard of resource locks on Azure. You mention to your manager that you think you can help prevent this type of incident from happening in the future. Let's take a look at how you could use resource locks to solve this problem.

## What are resource locks?
Resource locks are a setting that you can apply to any resource to block modification or deletion. You can set resource locks to either Delete or Read-only. Delete will allow all operations against the resource, but block the ability to delete it. Read-only will only allow read activities to be performed against it, blocking any modification or deletion of the resource. You can apply resource locks to subscriptions, resource groups, and to individual resources. Resource locks are inherited when applied at higher levels.

--------------------------

# Identify incorrectly assigned resources in Azure

## Organize Azure resources into resource groups

You use resource groups to logically group resources together. Each resource must be part of a single resource group. A resource group can hold many different types of resources in different regions.

Generally, resource groups hold resources that are related. For example, you can have a resource group for testing and development, and a separate one for production. A production resource group might hold resources that support a live website. These resources can include several virtual machines (VMs), storage accounts, virtual networks, and Azure SQL Database instances.

Make sure that all the resources in your resource group have a single lifecycle. You want to update, delete, or deploy these resources together. If you believe a resource doesn't fit into the lifecycle of other resources, move it to another resource group.

You can control which resources are available to different types of users. In this way, resource groups help you protect your resources and control costs.

To change the billing assignment for resources in resource groups, you can move resources from one resource group to another resource group in a different subscription. In this case, you need to put any dependent resources into one resource group. Then, move the resources from that resource group into a new resource group in the other subscription.

##  Use a consistent naming convention

To help identify and organize your resource groups, use a consistent naming convention. For example, you might have a resource group named project-infrastructure-resource-group to denote that it's a resource group for a certain project's infrastructure.

## Use tags to find resources
Tags are name and value pairs that you apply to resources. For example, you can set the name environment and its value as development for all resources that aren't meant for production. In this way, you ensure that you can easily find related resources and keep them organized.


  








