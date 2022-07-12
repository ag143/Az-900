## 

## Azure Account (how to get subscription and start using azure)
you can help them reddem their azure pass 

## Azure Physical Infra
[MS learn](https://docs.microsoft.com/en-us/learn/modules/describe-core-architectural-components-of-azure/5-describe-azure-physical-infrastructure)
> **Draw Diagram --:Read slide**

## Azure Regions 
- A region is a geographical area on the planet that contains at least one, but potentially multiple datacenters that are nearby and networked together with a low-latency network.

go to link in slide --> explore data residency --> services not avialable in all regions
click on browse --> vm 

## Availability Zones
- DC UNDER REGIONS
ZONAL SERVICE : azure vm --> create vm --> avaialbility options ---> avialability zones --> select zone 
ZONE REDUNDANT SERVICE : ZRS In azure storage account 

## Region Pairs
- STORAGE ACCOUNT OVERVIEW : PRIMARY & SECONDARY REGION
[region-pairs-ms-docs](https://docs.microsoft.com/en-us/azure/availability-zones/cross-region-replication-azure)

## Walkthrough
It's link of azure globe 
(click 2-3 times in a point at azure globe to see that )

## Sovereign Regions (Azure for Government) : 
- dedicated portal (https://portal.azure.us/)
- Azure Government provides an extra layer of protection to customers through contractual commitments regarding storage of customer data in the United States and limiting potential access to systems processing customer data to screened US persons.

## Azure China
- Microsoft doesn't directly maintain the datacenters.

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

**2 point in slide : The actual desktop and apps are running in the cloud, meaning the risk of confidential data being left on a personal device is reduced.

## Containers 
> Some of my developers uses windows, while some mac os (I want a portable app)
Containers are lightweight packages of your application code together with dependencies such as specific versions of programming language runtimes and libraries required to run your software services.
- Containers are lightweight and designed to be created, scaled out, and stopped dynamically.
 Hence more agile way of app development.
> Ice cream machine choclate & strawberry 🍓 flavours if some glitch with choclate
- Containers are often used to create solutions by using a microservice architecture. This architecture is where you break solutions into smaller, independent pieces

## ACI 
- Paas 

## AKS
-K8s, is an open-source system for automating deployment, scaling, and management of containerized applications

## Azure App Service 


## Azure Function
Serverless : 
- Azure Functions is an event-driven, serverless compute option that doesn’t require maintaining virtual machines or containers
- Pay : you're only charged for the CPU time used while your function runs.

## Azure Vnet 
- Software emulation of your network
- helps connect your azure resources (like VM,Databases, web apps etc) together or to the internet or other networks.

## VPN 
- VPNs can enable networks to safely and securely share sensitive information.
- site to site & Point to site 

## Azure ExpressRoute
CHECK DOCS 

## Azure DNS 
- MS IS IN 140 + COUNTRIES --  DNS query is answered by the closest available DNS server to provide fast performance and high availability for your domain
 - YOU CAN'T BUT DOMAIN HERE


## azure storage account
- Azure Storage offers two options for copying your data to a secondary region: geo-redundant storage (GRS) and geo-zone-redundant storage (GZRS). GRS is similar to running LRS in two regions, and GZRS is similar to running ZRS in the primary region and LRS in the secondary region.
- secondary region read write not available unless primary unavailable.

```
azcopy make "https://<storage-account-name.blob.core.windows.net/mycontainer_name"
azcopy copy "local-file-path" "https://<storage-account-name>.blob.core.windows.net/<container-name>/<blob-name>"

```

> Azure supports both real-time migration of infrastructure, applications, and data using Azure Migrate as well as asynchronous migration of data using Azure Data Box.

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

# IAM 
## AAD SERVICE
Azure Active Directory (Azure AD) is Microsoft’s cloud-based identity and access management service, which helps your employees sign in and access resources

## MFA 
search in windows connect --> cast in intex --> show authenticator app 

## B2B 
Invite users 

## B2C
APPLICATION --> SAML OAUTH TOKENS 

## conditional access 
If then statement

## RBAC 
once you can login to azure now what permissions you have

## zero trust
TRSUT NO ONE :- because it’s within the corporate network, it requires everyone to authenticate. Then grants access based on authentication rather than location

## Defence in depth
To protect against security breach You can visualize defense-in-depth as a set of layers, so if one layer is broken. Your data is safe from attack.
- perimeter layer just b4 network to protect my network like DDOS

## MS DEFENDER FOR CLOUD
| **Security Requirements** | Description |
| --- | --- |
| `Continuous assessment` - Understand your current security posture. |  Secure score - A single score so that you can tell, at a glance, your current security situation: the higher the score, the lower the identified risk level.|
| `Secure Environment` Secure - Harden all connected resources and services| You implement a recommendation by following the detailed remediation steps provided in the recommendation. For many recommendations, Defender for Cloud offers a "Fix" button for automated implementation!|
|`Defend` Detect and resolve threats to those resources and services. | These alerts appear in the Azure portal and Defender for Cloud can also send them by email to the relevant personnel in your organization. Alerts can also be streamed to SIEM, SOAR, or IT Service Management solutions as required.|


[Pricing + Details](https://azure.microsoft.com/en-us/services/databox/)

# [MS LEARN FOR MODULE 2](https://docs.microsoft.com/en-us/learn/paths/azure-fundamentals-describe-azure-architecture-services/)
