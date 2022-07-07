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

## Azure Resources
Azure Resource make profit of yours.

**Draw + slide**

## Resource Group
Portal

## azure subscription

## azure management group

# compute & Networking

**In portal + slide**


## Azure Virtual Desktop : 
- (end user Computing) --> Helps you create a windows 10,11 like env on the cloud which can be pooled (shared to multiple people at same time) --> can set up max connection limit
 / individual use
- can be connected to your on-prem ADDS
- you can login using web clinet or desktop/andriod/Ios client
- host pools (the VM's used to create this, all have same os,size)

## Containers 
Containers are lightweight packages of your application code together with dependencies such as specific versions of programming language runtimes and libraries required to run your software services.


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
