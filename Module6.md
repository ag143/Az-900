[minimising cost](#minimising-cost)

[SLA](#what-effects-your-sla)

[Service lifecycle -> public preview and generally available](#service-lifecycle)

# Cost Management 

### Factors affecting Cost 

1. **Resource Type**
- `How you configure your resource`
For example, with a storage account you specify a type (such as block blob storage or table storage), a performance tier (standard or premium), and an access tier (hot, cool, or archive). These selections present different costs.

2. **Purchasing Services**
`The usage rates and billing period varies`
- enterprise customers (pay annually)
- web direct (pay monthly)
- CSP [Cloud Solutions Provider] (Your CSP bills you for your Azure usage at a price they determine)
- free tier (with some 12 months free services + some credits to spend)

3. **Location**
`Azure is Globally distributed, but every region gives different Pricing`
You may choose a cheaper region but data transfer cost also applies. 

4. **Bandwidth**
`Data into Azure free; outside Costs money 💲💵`

5. **Reserved Instance**
`Prepay or commit your resource usuage... in turn you get huge discounts 🤑`
- Azure Reservations can save you up to 72 percent as compared to pay-as-you-go prices. To receive a discount, you reserve services and resources by paying in advance.
For example, you can prepay for one year or three years of use of VMs, database compute capacity, database throughput, and other Azure resources.

6. **Hybrid use benefit** 
`use your present license,save money😁`
- If you've purchased licenses for Windows Server or SQL Server, and your licenses are covered by Software Assurance, you might be able to repurpose those licenses on VMs on Azure.

## minimising cost

#### Azure Cost Management
- A centralized service for reporting usage and billing of Azure environment
- Self-service cost exploration capabilities
- Budgets & alerts
- Cost recommendations
- Automated exports

#### Minimizing Costs in Azure
- Azure Pricing Calculator to choose the low-cost region
Good latency
All required services are available
Data sovereignty/compliance requirements
- Hybrid use benefit and Azure Reservations
- Azure Cost Management monitoring, budgets, alerts and recommendations
- Understand service lifecycle and automate environments
- Use autoscaling features to your advantage
- `Azure Monitor to find and scale down underutilized resources`
- Use tags & policies for effective governance
 


# SLA

### What effects your SLA
- To ensure high availability, you might plan for your application to have duplicate components across several regions, known as redundancy. 
        - To reduce cost, you can also shut down the above extra capacity for non critical time (like midnight)
- Adding More services reduces SLA .... Why ?? <br>
        - more services means more complex and more risky application

[Check SLA HERE (from MS Website)](https://azure.microsoft.com/en-us/support/legal/sla/summary/)
  
**Example** - 
![This is the architecture ](https://docs.microsoft.com/en-us/learn/azure-fundamentals/choose-azure-services-sla-lifecycle/media/4-special-orders-architecture.svg)

| Service| SLA |
|------| ----- |
| VM | 99.9|
| SQL | 99.99 |
| Azure Load Balancer | 99.99 |

**Composite SLA (Your Application's Uptime or Application SLA)** = 99.9% × 99.9% x 99.99% x 99.99% = 0.999 x 0.999 x 0.9999 x 0.9999 = 0.9978 = **99.78%**

### Logical AND - adding dependency

**Availability of S1 AND S2 = Availability(S1) * Availability(S2)**

##### Scenario - Azure website with SQL backend db
Availability = Availability(web) app * Availability(sql)
Availability = 99.95% * 99.95%
Availability = 0.9995 * 0.9995
Availability = 0.99900025
Availability ~ 99.9%

### Logical OR - adding redundancy

**Availability of S1 OR S2 = 100% - ( Unvailability(S1) * Unvailability(S2) )**

Scenario - Two redundant web apps behind a load balancer
Availability(both-web) = 100% - ( Unvailability(web1) * Unvailability(web2) )
Availability(both-web) = 100% - ( 0.05% * 0.05% )
Availability(both-web) = 1 – ( 0.0005 * 0.0005 )
Availability(both-web) = 1 – 0.00000025
Availability(both-web) = 0.99999975
Availability(both-web) ~ 99.9999%

## Service lifecycle

After developing services for Microsoft Azure to test them Microsoft Microsoft after developing launches them for public preview and then after working on feedbacks and improving it. Launches for general public (known as Generally Available)


- Every service in Azure follows its own service lifecycle
- Public preview is a ‘beta’ stage of the service available to general public use
- Features can also be in preview stages
       • Designed for testing, not production solutions
- General availability is a ‘production’ release of the service

### Public Preview Key Info
- No SLA
- Some services have no support coverage
- Limited region availability
- Limited functionality
- Pricing changes
- A dedicated portal to check all  previews . [Azure Portal Previews](https://preview.portal.azure.com)
