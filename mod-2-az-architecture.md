## 

## Azure Account (how to get subscription and start using azure)
you can help them reddem their azure pass 

## Azure Physical Infra
[MS learn](https://docs.microsoft.com/en-us/learn/modules/describe-core-architectural-components-of-azure/5-describe-azure-physical-infrastructure)
**Draw Diagram --:Read slide**

## Azure Regions 
go to link in slide --> explore data residency --> services not avialable in all regions
click on browse --> vm 

## Availability Zones
ZONAL SERVICE : azure vm --> create vm --> avaialbility options ---> avialability zones --> select zone 
ZONE REDUNDANT SERVICE : ZRS In azure storage account 

## Region Pairs
[region-pairs-ms-docs](https://docs.microsoft.com/en-us/azure/availability-zones/cross-region-replication-azure)

## Walkthrough
It's link of azure globe 
(click 2-3 times in a point at azure globe to see that )

## Sovereign Regions (Azure for Government) : 
- dedicated portal (https://portal.azure.us/)
- Azure Government provides an extra layer of protection to customers through contractual commitments regarding storage of customer data in the United States and limiting potential access to systems processing customer data to screened US persons.

```
https://docs.microsoft.com/en-us/azure/azure-government/compare-azure-government-global-azure
https://azure.microsoft.com/en-in/global-infrastructure/government/?cdn=disable
```
**Draw + slide**

## Azure Resources
Anything you create, provision, deploy, etc. is a resource. Virtual Machines (VMs), virtual networks, databases, cognitive services, etc. are all considered resources within Azure.
Azure Resource makes profit of yours.

## Resource Group
What is RG ? 
A logical Container of Resources

How it helps : 
- lifecycle management : common lifecycle of underlying resources 
- simple access control : access at RG level = access to all of its Resources

It's properties : 
- 1 Resource to only 1 RG
- PARENT CHILD RELATIONSHIP
- Resources can be moved : Some resources may be moved between resource groups, but when you move a resource to a new group, it will no longer be associated with the former group.

What you can't do ?
- RG Can't be nested 
- RG can't be renamed

Portal

## azure subscription
[Check here AZ 305 notes](https://github.com/Ananyojha/az-305/blob/main/Module-1.md#subscription)

## azure management group
- 10,000 management groups can be supported in a single directory.
- A management group tree can support up to six levels of depth. This limit doesn't include the root level or the subscription level

# compute & Networking

**In portal + slide**

## VM 
- VMs PROVIDE (IaaS) in the form of a virtualized server 
- Just like your physical computer, you can customize all of the software running on your VM.
[Show your VM] 

## VM SCALE SET
- you simply created multiple VMs with the same purpose

**Availability Set** 



## Azure Virtual Desktop : 
- (end user Computing) --> Helps you create a windows 10,11 like env on the cloud which can be pooled (shared to multiple people at same time) --> can set up max connection limit
 / individual use
- multiple concurrent users on a single VM.
- can be connected to your on-prem ADDS
- you can login using web clinet or desktop/andriod/Ios client
- host pools (the VM's used to create this, all have same os,size)

## Containers 
> Some of my developers uses windows, while some mac os (I want a portable app)
Containers are lightweight packages of your application code together with dependencies such as specific versions of programming language runtimes and libraries required to run your software services.
- Containers are lightweight and designed to be created, scaled out, and stopped dynamically.
 Hence more agile way of app development.
> Ice cream machine choclate & strawberry 🍓 flavours if some glitch with choclate
- Containers are often used to create solutions by using a microservice architecture. This architecture is where you break solutions into smaller, independent pieces

## ACI 
- Paas 

## Azure Function
Serverless : 
- Azure Functions is an event-driven, serverless compute option that doesn’t require maintaining virtual machines or containers
- Pay : you're only charged for the CPU time used while your function runs.

## Azure Migrate : 
Azure Migrate provides a centralized hub to assess and migrate on-premises servers, infrastructure, applications, and data to Azure.
[Show in azure docs --> then in portal that you can migrate on prem to cloud](https://docs.microsoft.com/en-us/azure/migrate/migrate-services-overview)
- Not only on -prem You migrate AWS (other cloud) VMs to Azure by treating them as physical servers.

## Data Box 
- When 100 TB data, it's difficult to transfer it using internet as a medium via  portal, azcopy 
- order data box , connect your server laptop to data box via cables
- send it to MS datacenter
- get it uploaded to Azure 

You can also get TB's of data from Azure to your facility using same workflow as above. 

- based on Size of data : Data box disks, Data box Heavy and simply databox

[Pricing + Details](https://azure.microsoft.com/en-us/services/databox/)

# [MS LEARN FOR MODULE 2](https://docs.microsoft.com/en-us/learn/paths/azure-fundamentals-describe-azure-architecture-services/)
