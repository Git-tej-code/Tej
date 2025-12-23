# Packages & Deployment

AutoX uses a **package-based deployment model** to ensure that automation is released in a **controlled, auditable, and reversible** manner. Packages act as immutable containers that group together specific versions of processes, activities, agents, and configurations for deployment across environments.

This approach prevents accidental changes, preserves execution history, and enables safe evolution of automation at enterprise scale.

***

#### Why Packages Exist

In traditional automation, changes are often made directly to live workflows, leading to unpredictable behavior and compliance risks. AutoX avoids this by enforcing packaging and versioning.

Packages exist to:

* Ensure deployment safety
* Preserve execution consistency
* Enable controlled promotion across environments
* Support audit and rollback

Every deployment in AutoX happens through a package—**never directly from editable artefacts**.

***

#### What a Package Contains

A package may include:

* One or more **process versions**
* Associated **activity versions**
* Referenced **agent versions**
* Configuration metadata

Each item inside a package is locked to a **specific version**, ensuring predictable execution.

#### Package Complete Diagram/Screenshots

📐 Diagram REQUIRED (Critical)

Show:

&#x20;

Package v1\
&#x20;├─ Process A v2.1\
&#x20;└─ Process B v1.3

***

#### Package Immutability (Sacred Rule)

Once a package is created and locked:

* It **cannot be modified**
* It **cannot be deleted**
* Its contents and versions are preserved permanently

If changes are required, the correct approach is to **duplicate**, modify, and create a **new package**.

This rule guarantees trust, traceability, and compliance.

***

#### Deployment Lifecycle

Packages move through environments in a controlled lifecycle:

```
Created → Locked → UAT → Deployed → Archived
```

* **Created**: Package assembled with selected versions
* **Locked**: No further edits allowed
* **UAT**: Validated in a test environment
* **Deployed**: Promoted to production
* **Archived**: Retained for history and audit

Rollback is achieved by redeploying a **previous package**, not by undoing changes.

***

#### Custom Version Selection

AutoX allows users to:

* Select custom versions of processes, activities, and agents when creating a package
* Mix stable and experimental versions intentionally
* Control deployment granularity

This provides flexibility without sacrificing governance.

***

#### Roles and Deployment Control

Deployment actions are restricted by role:

* Only authorized users can create or promote packages
* Locking is required before promotion
* Audit logs capture who deployed what and when

This prevents unauthorized or accidental production changes.

***

#### Observability and Audit

Every package deployment is:

* Logged
* Traceable to execution runs
* Visible in observability dashboards

This enables:

* Root cause analysis
* Compliance reporting
* Operational confidence

