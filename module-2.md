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
