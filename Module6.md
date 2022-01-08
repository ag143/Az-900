

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

# SLA

### What effects your SLA
- To ensure high availability, you might plan for your application to have duplicate components across several regions, known as redundancy. 
        - To reduce cost, you can also shut down the above extra capacity for non critical time (like midnight)
- Adding More services reduces SLA .... Why ?? <br>
        - more services means more complex and more risky application
  
         **Example** - 
           | Service | SLA |
            --------. -----
           | VM | 99.9|
