# Access Control Model

**RBAC and ABAC in AutoX**

AutoX uses a hybrid access control model combining:

**Role-Based Access Control (RBAC)**

RBAC determines what actions a user can perform.

Permissions are defined at role level for:

* Create
* View
* Edit
* Delete
* Deploy
* Observe

Users inherit permissions only from roles.

There are no per-user overrides.

&#x20;

**Attribute-Based Access Control (ABAC)**

ABAC determines where and on what scope actions can be performed.

Access is constrained by attributes such as:

* Organization
* Department
* Function
* Project
* Environment (Dev / QA / UAT / Prod)

RBAC answers “What can you do?”

ABAC answers “Where can you do it?”

&#x20;

**Important Governance Rules**

* RBAC is static and intentional
* ABAC is evaluated at runtime
* Missing UI items usually indicate access restriction, not missing features

