# Assign Roles

AutoX uses a combination of **default roles** and **custom roles** to control user access across the platform. Role assignment determines **what a user can see, create, modify, deploy, or observe**, while still enforcing AutoX’s governance rules such as version locking, package immutability, and audit logging.

Roles work together with attribute-based controls (ABAC) to ensure access is both **secure and context-aware**.

***

#### Who Can Assign or Manage Roles

* **Super Admin**
  * Manages roles at the organization level
  * Onboards Platform Admins
  * Can create and assign both default and custom roles
* **Platform Admin**
  * Manages users and roles within their organization
  * Can create and assign custom roles

Other roles **cannot assign or modify roles**.

***

#### Assigning a Default Role

Default roles are predefined by AutoX and cover the most common responsibilities.

**Examples of default roles:**

* Platform Admin
* Power User
* Agent Developer
* Business User

Use a **default role** when:

* A user’s responsibilities clearly match a single role
* Standard access patterns are sufficient
* Long-term, stable access is required

Default roles are **fixed**, audited, and cannot be modified.

***

#### Creating and Using Custom Roles

Custom roles allow administrators to define **fine-grained access** when default roles are not sufficient.

Custom roles are useful when:

* A user’s responsibilities do not fully match any single default role
* Partial access is needed across multiple areas
* **Temporary or project-specific access** is required
* Access must be restricted more tightly than default roles allow

Custom roles can control permissions across:

* Departments and Functions
* Processes and Activities
* Agent Builder
* Agent Observer
* Integrations
* Packages and deployment
* Reports and observability

Permissions typically follow **View / Create / Edit / Delete** patterns.

***

#### How Roles Are Applied

1. An administrator assigns one or more roles to a user
2. The user’s navigation and capabilities update automatically
3. Access is enforced across:
   * Main Platform
   * Agent Builder
   * Agent Observer

A user may have:

* **One default role**
* **Multiple roles**
* A combination of **default and custom roles**

All role assignments are logged for audit purposes.

***

#### Default vs Custom Roles (Quick Guide)

| Scenario                          | Recommended Role |
| --------------------------------- | ---------------- |
| Clear, standard responsibility    | Default role     |
| Partial access across features    | Custom role      |
| Temporary or project-based access | Custom role      |
| Need to limit permissions tightly | Custom role      |
| Full platform control             | Platform Admin   |

***

#### Important Governance Rules

* Roles define **capability**, not data ownership
* Roles do **not bypass** versioning, locking, or deployment rules
* Removing a role immediately revokes access
* Role changes are auditable and traceable

***

#### Common Issues

* **User cannot see a feature**\
  → Required role or permission not assigned
* **User has more access than needed**\
  → Replace default role with a custom role
* **Temporary access needed**\
  → Assign a custom role and remove it when the project ends

***

#### Please Insert a Screenshots for Making these roles with examples&#x20;
