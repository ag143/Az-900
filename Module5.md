### Multi-factor Authentication (MFA)
Process of authentication using more than one factor (evidence) to prove identity
Factor types
- Knowledge Factor – “Something you know”, ex. password, pin
- Possession Factor – “Something you have”, ex. phone, token, card, key
- Physical Characteristic Factor – “Something you are”, ex. fingerprint, voice, face, eye iris
- Location Factor – “Somewhere you are”, ex. GPS location
Supported by Azure AD by default (simple on-off switch)


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

[Azure AD vs RBAC](https://tutorialsdojo.com/azure-active-directory-ad-vs-role-based-access-control-rbac/)

### Resource locks 
`Resource locks apply regardless of RBAC permissions. Even if you're an owner of the resource, you must still remove the lock before you can perform the blocked activity.`

### Azure Policy
A service in Azure that enables you to create, assign, and manage policies that control or audit your resources. 

- Azure Policy evaluates your resources and highlights resources that aren't compliant with the policies you've created. Azure Policy can also prevent noncompliant resources from being created.
- you can define both individual policies and groups of related policies, known as initiatives.
- **Build in policy for compute, Networking** - if you define a policy that allows only a certain SKU (stock-keeping unit) size for the virtual machines (VMs) to be used in your environment, that policy is invoked when you create a new VM and whenever you resize existing VMs.
- create custom policy like -- Restrict resource deployment to a particular region only. 

### Azure Blueprint
**Enabling quick, repeatable creation of governed environments**
- Helps Govern Multiple Subscription 
- With Azure Blueprints, the relationship between the blueprint definition (what should be deployed) and the blueprint assignment (what was deployed) is preserved. This connection supports improved tracking and auditing of deployments. 
- #### Package of various Azure components (artifacts)
- Resource Groups
- ARM Templates
- Policy Assignments
- Role Assignments
- Centralized storage for organizationally approved design patterns
1. Blueprint definition – describing what should happen (reusable package)
2. Blueprint assignment – describing where it should happen (package deployment)

> To make the protection process more robust, you can combine resource locks with Azure Blueprints. Azure Blueprints enables you to define the set of standard Azure resources that your organization requires. For example, you can define a blueprint that specifies that a certain resource lock must exist. Azure Blueprints can automatically replace the resource lock if that lock is removed.

### Azure Cloud Adoptation Framework
The Cloud Adoption Framework includes these stages:

- Define your strategy.
- Make a plan.
- Ready your organization.
- Adopt the cloud.
- Govern and manage your cloud environments.
