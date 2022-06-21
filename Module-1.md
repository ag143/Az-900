# Private Cloud : 
- create cloud like environment in your data center (like use **NAS** : network-attached storage (NAS) device is a data storage device that connects to and is accessed through a network, instead of connecting directly to a computer.)
- A number of datacentres under 1 single org 

# Hybrid Cloud : 
- OEM partners : who provide you MS approved hardware to connect to MS
- NO. of services : expressroute, Azure for VMware, azure sphere etc

# Cloud Terms 

#### Fault Tolerance : A fault tolerant environment has no service interruption but a significantly higher cost, while a highly available environment has a minimal service interruption

#### Disaster Recovery : How quickly you start your application once any man made/ natural Disaster occurred
[MS DOCS](https://docs.microsoft.com/en-us/azure/architecture/framework/resiliency/backup-and-recovery) 
- the cloud, plan before hand that failures will happen. Instead of trying to prevent failures altogether, the goal is to minimize the effects of a single failing component
**Methods** : 
1. Redeploy from scratch (less costly ---> time taken is most)
2. Active / passive
3. Active / active (most costly ---> time is least)

