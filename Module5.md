[RBAC](#rbac)

[Conditional access](#conditional-access)

[Azure Policy](#azure-policy)

[Azure Blueprint](#azure-blueprints)

[Cloud adoption framework](#cloud-adoptation-framework)

[Can you trust Azure ? --> Azure Compliance, Azure US Gov](#azure-compliance-and-privacy)

### Multi-factor Authentication (MFA)
Process of authentication using more than one factor (evidence) to prove identity
Factor types
- Knowledge Factor – “Something you know”, ex. password, pin
- Possession Factor – “Something you have”, ex. phone, token, card, key
- Physical Characteristic Factor – “Something you are”, ex. fingerprint, voice, face, eye iris
- Location Factor – “Somewhere you are”, ex. GPS location
Supported by Azure AD by default (simple on-off switch)

> Basic principal of IAM = Give what they need, no extra permission ... (Principle of Least Privilege)

## Azure Active Directory
- Identity and Access Management service in Azure
- Identities management – users, groups, applications
- `IT Administrators` can use Azure AD to control access to applications and resources based on their business requirements
- `Application management`
You can manage your cloud and on-premises apps by using Azure AD. 
Access management – subscriptions, resource groups, roles, role assignments, authentication & authorization settings, etc.
-  `device management` It also allows for device-based Conditional Access policies to restrict access attempts to only those coming from known devices, regardless of the requesting user account.
- U can also `connect to your existing AD using Azure AD connect`
sed by multiple Microsoft cloud platforms
Azure
Microsoft 365
Office 365
Live.com services (Skype, OneDrive, etc.)

### single sign on 
Login (give credentials once, açcess all services) eg - Login into one Google account, get signed into all other services like Gmail, YouTube, drive etc.

### Conditional Access

- #### User or group membership
Policies can be targeted to specific users and groups giving administrators fine-grained control over access.
- #### IP Location information
Organizations can create trusted IP address ranges that can be used when making policy decisions.
Administrators can specify entire countries/regions IP ranges to block or allow traffic from.
Device
Users with devices of specific platforms or marked with a specific state can be used when enforcing Conditional Access policies.
Application
Users attempting to access specific applications can trigger different Conditional Access policies.
- #### Real-time and calculated risk detection
Signals integration with Azure AD Identity Protection allows Conditional Access policies to identify risky sign-in behavior. Policies can then force users to change their password, do multi-factor authentication to reduce their risk level, or block access until an administrator takes manual action.
- #### Microsoft Defender for Cloud Apps
Enables user application access and sessions to be monitored and controlled in real time, increasing visibility and control over access to and activities done within your cloud environment.


## RBAC
#### What is a Role?
Role (role definition) is a collection of actions that the assigned identity will be able to perform.

Role definition is an `answer to a question “What can be done?”`

#### What is a Security Principal?
Security Principal is an Azure object (identity) that can be assigned to a role (ex. users, groups or applications).

Security Principal assignment is an `answer to a question “Who can do it?”`

#### What is a Scope?
Scope is one or more Azure resources that the access applies to.

Scope assignment is an answer to a question “`Where can it be done?”`

#### What is a Role Assignment?
Role assignment is a combination of the role definition, security principal and scope.

### Azure Role-based Access Control (RBAC)
- Authorization system built on Azure Resource Manager (ARM)
- Designed for fine-grained access management of Azure Resources
- Role assignment is combination of
- Role definition – list of permissions like create VM, delete SQL, assign permissions, etc.
- Security Principal – user, group, service principal and managed identity and
- Scope – resource, resource groups, subscription, management group
Hierarchical
Management Groups > Subscriptions > Resource Groups > Resources
Built-in and Custom roles are supported

### Resource locks 
`Resource locks apply regardless of RBAC permissions. Even if you're an owner of the resource, you must still remove the lock before you can perform the blocked activity.`

To make the protection process more robust, you can combine resource locks with Azure Blueprints. Azure Blueprints enables you to define the set of standard Azure resources that your organization requires. For example, you can define a blueprint that specifies that a certain resource lock must exist. Azure Blueprints can automatically replace the resource lock if that lock is removed.

### Azure Policy
A service in Azure that enables you to create, assign, and manage policies that control or audit your resources. 

- Azure Policy evaluates your resources and highlights resources that aren't compliant with the policies you've created. Azure Policy can also prevent noncompliant resources from being created.
- you can define both individual policies and groups of related policies, known as initiatives.
- **Build in policy for compute, Networking** - if you define a policy that allows only a certain SKU (stock-keeping unit) size for the virtual machines (VMs) to be used in your environment, that policy is invoked when you create a new VM and whenever you resize existing VMs.
- create custom policy like -- Restrict resource deployment to a particular region only. 

### Azure Blueprints

-----
Let me ask you a question. Would you consider building a house without knowing what it would look like when you're done? The supplies needed? Ofcourse No 😏
-----
> So as a Cloud Engineer Deviating from my company's design principles and best practices increases support costs and leads to unhappy customers. 

Azure Blueprints use existing Azure services like Azure Policies, permissions and ARM templates to give you control of the rollout of your environment. 

These building blocks of Azure 🔵 Blueprint are known as Artifact's
- ARM Templates - Use It for creation of resources
- Resource Groups - Specify the resource groups you want to create
- Roles Assignments - Apply IAM roles to the deployed resource groups to apply permissions to users and/or groups
- Policies Assignments - Apply Azure Policies and/or Initiatives to your environments


### Cloud Adoptation Framework
Cloud Adoption Framework consists of tools, documentation, and proven practices. The Cloud Adoption Framework includes these stages:

- Define your strategy.
- Make a plan.
- Ready your organization.
- Adopt the cloud.
- Govern and manage your cloud environments.

# Azure Compliance and Privacy
🔏 ![✅](https://github.com/Ananyojha/spare-images/blob/main/IMG_20220109_164933.jpg?raw=true)
