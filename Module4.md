Security Information and Event Management (SIEM) is a set of tools and services offering a holistic view of an organization's information security. SIEM tools provide: Real-time visibility across an organization's information security systems. Event log management that consolidates data from numerous sources.

## Azure Security Centre 

> Azure Security Center and Azure Defender are now called Microsoft Defender for Cloud

| **Security Requirements** | Description |
| --- | --- |
| `Continuous assessment` - Understand your current security posture. |  Secure score - A single score so that you can tell, at a glance, your current security situation: the higher the score, the lower the identified risk level.|
| `Secure Environment` Secure - Harden all connected resources and services| You implement a recommendation by following the detailed remediation steps provided in the recommendation. For many recommendations, Defender for Cloud offers a "Fix" button for automated implementation!|
|`Defend` Detect and resolve threats to those resources and services. | These alerts appear in the Azure portal and Defender for Cloud can also send them by email to the relevant personnel in your organization. Alerts can also be streamed to SIEM, SOAR, or IT Service Management solutions as required.|

## Azure Sentinel

**Now called as MS Sentinel**
- It provides a `birds eye view of your org
- Microsoft Sentinel delivers intelligent security analytics and threat intelligence across the enterprise, providing a single solution for attack detection, threat visibility, proactive hunting, and threat response
- Investigate threats with artificial intelligence, and hunt for suspicious activities at scale, tapping into years of cyber security work at Microsoft.

## Azure Key Vault 
- Azure Key Vault is a cloud service for securely storing and accessing secrets. A secret is anything that you want to tightly control access to, such as API keys, passwords, certificates, or cryptographic keys.

## Azure Dedicated Host 
- A dedicated physical server to host your Azure VMs for Windows and Linux
- so server rack not shared with other customers. This host-level isolation helps address compliance requirements. As you provision the host, you gain visibility into and control over the placement of your Azure VMs and you determine the host's maintenance policies
- Offers pricing and benefits for Windows Server and SQL Server available only on Azure

# Defence in Depth 
- The objective of defense in depth is to protect information and prevent it from being stolen by those who aren't authorized to access it.

- A defense-in-depth strategy uses a series of mechanisms to slow the advance of an attack that aims at acquiring unauthorized access to data.

`Benefit is` :- slows down an attack and provides alert telemetry that security teams can act upon, either automatically or manually.


## Azure DDoS Protection
- Backed by the Microsoft global network, DDoS Protection brings massive DDoS mitigation capacity to every Azure region. Filter traffic at the Azure network edge before it can impact the availability of your service.
- Cover all resources on a virtual network when you enable Azure DDoS Protection via simplified configuration. 
- `DDoS Protection automatically mitigates the attack as soon as it’s detected`
- The DDoS Protection service will have a fixed monthly charge

## Defence in Depth Reviewed
The perimeter layer uses distributed denial of service (DDoS) protection to filter large-scale attacks before they can cause a denial of service for users.
The network layer limits communication between resources through segmentation and access controls.

## Real life use -- 
> Deployed with Azure Application Gateway Web Application Firewall, DDoS Protection defends against a comprehensive set of network layer (layer 3/4) attacks, and protects web apps from common application layer (layer 7) attacks, such as SQL injection, cross-site scripting attacks, and session hijacks. Web Application Firewall comes preconfigured to handle threats identified by the Open Web Application Security Project top 10 common vulnerabilities.

[Security Center ](https://www.ibm.com/in-en/topics/siem)

