[COURSE-INTRO--MS-LEARN](https://docs.microsoft.com/en-gb/learn/modules/describe-cloud-compute/1-introduction-microsoft-azure-fundamentals?ns-enrollment-type=learningpath&ns-enrollment-id=learn.wwl.microsoft-azure-fundamentals-describe-cloud-concepts)

In 1 module, you’ll be introduced to general cloud concepts. You’ll start with an introduction to the cloud in general. Then you'll dive into concepts like shared responsibility, different cloud models, and explore the unique pricing method for the cloud.

Basic terms : 
**draw diagram**

- servers 
- storage
- network
- identity provider 

 The company is responsible for maintaining the physical space, ensuring security, and maintaining or replacing the servers if anything happens. The IT department is responsible for maintaining all the infrastructure and software needed to keep the datacenter up and running. They’re also likely to be responsible for keeping all systems patched and on the correct version

Owning a home is much better than renting if your requirements are stable, but if you know you’re likely to move a lot, renting is the better deal.
-------------------------------------------------------------------------------------------------------------------------------------------------------

Cloud is not important only for IT Companies as almost every company is now IT enabled company - i.e relies heavily on IT like banks, Zomato , vedantu  

## What is cloud Computing 
- delivery of computing resources over a network.
- Cloud services also expand the traditional IT offerings to include things like Internet of Things (IoT), machine learning (ML), and artificial intelligence (AI).

## Shared Responsibility model
**YOUR CLOUD SERVICE PROVIDER IS RESPONSIBLE FOR SECURITY OF THE CLOUD & AS CUSTOMERS YOU MANAGE IN THE CLOUD**
- Physical security, power, cooling, and network connectivity are the responsibility of the cloud provider
-  the consumer is responsible for the data and information stored in the cloud
-  You’ll always be responsible for:

The information and data stored in the cloud
Devices that are allowed to connect to your cloud (cell phones, computers, and so on)
The accounts and identities of the people, services, and devices within your organization

- The cloud provider is always responsible for:

The physical datacenter
The physical network
The physical hosts

- Your service model will determine responsibility for things like:

Operating systems
Network controls
Applications
Identity and infrastructure


## Private Cloud 
- create cloud like environment in your data center (like use **NAS** : network-attached storage (NAS) device is a data storage device that connects to and is accessed through a network, instead of connecting directly to a computer.)
- A number of datacentres,resources used by single org 

## Public Cloud 

## Private Cloud 

## Model Comparision 

## Capex vs opex
- CapEx is typically a one-time, up-front expenditure to purchase Resources
- opex (operational + expenditure) : pay as you operate

## Consumption based model
[Slide]

## Cloud Benefits -- 
two of the biggest considerations are uptime (or availability) and the ability to handle demand (or scale
- Scalability : Scalability refers to the ability to adjust resources to meet demand
Vertical Scalable : CPU/ RAM SPECIFICATIONS
HORIZONTAL : 

- Reliable : What if there a disaster in the region where your services are deployed ?
With Azure's global scale you can fail over to other region. In some cases this happens auto
Like GRS 

* Reliability is the ability of a system to recover from failures and continue to function

Also known as DR

- predicting : cost (PRICING CAL + SUBSCRIPTION --> MSDN --> COST ANALYSIS)

- Security : MS Spends $1 Billion year on security of the cloud + AS developers we have services like **WAF**, **AZURE FIREWALL**, **AZURE DDOS** etc

- Governance means your company standards, rules and regulations are followed in your Azure cloud env for which we have **RBAC, AZ BLUEPRINT, AZ POLICY**

- easily manage Resources in more agile way [MS DOCS](https://docs.microsoft.com/en-gb/learn/modules/describe-benefits-use-cloud-services/5-manageability-cloud)

[MS-LEARN](https://docs.microsoft.com/en-gb/learn/modules/describe-benefits-use-cloud-services/2-high-availability-scalability-cloud)


## Cloud Services 

IaaS is similar to take and bake — you don’t have to shop for separate ingredients, but you still have to heat the oven, set the table and clean up. One level up is delivery — no oven to heat, but you still have to figure out drinks and dishes. One additional level up is going out to a restaurant, which is similar to SaaS, where you have the least work and you’re paying someone else to wash the dishes.

## iaas
- You are a infra guy
- Rent the hardware 
- lift and shift migration
- You need control of your app

## paas
- it is developer friendly
- **show app service** : Cloud features such as scalability, high-availability,

## saas 


## Comparison 

------------------------------------------------------------------------------------------

--------


-------
# Private Cloud : 


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

# Serverless 
enables developers to build applications faster by eliminating the need for them to manage infrastructure. With serverless applications, the cloud service provider automatically provisions, scales and manages the infrastructure required to run the code.
- Servers are still used but invisible to the developer.
## use cases : 
build web applications and mobile backends in a faster, more agile way
