# Process

A **Process** in AutoX represents an **end-to-end business workflow** that coordinates multiple activities, decisions, integrations, agents, and human interactions to achieve a specific business outcome. Processes define _what needs to happen_ across a business function, without embedding low-level execution details directly inside them.

Processes act as the **primary orchestration layer** where business intent is translated into structured, governed automation.



**AutoX intentionally separates responsibilities:**

* Business users define workflow intent
* Technical users define execution logic
* Agents handle intelligence
* Platform enforces safety

This separation reduces rework, risk, and ownership conflicts.

&#x20;

**Diagram OPTIONAL**

Swimlane diagram:

* Business lane
* Technical lane
* Platform governance lane

***

#### Role of a Process in AutoX

In the AutoX hierarchy, a process sits between **Functions** and **Activities**:

```
Function
 → Process
   → Activity
```

A process:

* Defines the **overall flow**
* Orchestrates **multiple reusable activities**
* Controls **execution order and decision paths**
* Acts as the unit of **deployment and governance**

***

#### What a Process Is (and Is Not)

**A process is:**

* A logical representation of a business flow
* A container that orchestrates activities
* A governed, versioned artefact

**A process is not:**

* A place for detailed execution logic
* A monolithic script
* A collection of unrelated steps

Execution details belong in **Activities and Tasks**, not in the process itself.

***

#### Process Design vs Process Execution

AutoX separates process work into two complementary views:

* **Design (WorkJam)**\
  Used for business-level flow design, review, and collaboration
* **Develop (Canvas)**\
  Used for defining execution order, activity connections, and logic

This separation allows business and technical users to collaborate without conflict.

***

#### Versioning and Lifecycle

Every process in AutoX is:

* Versioned automatically
* Immutable once locked
* Never deleted

Typical lifecycle:

```
Created → In Progress → Locked → Packaged → Deployed → Archived
```

New changes always result in a **new version**, preserving history and auditability.

***

#### Process and Governance

Processes are governed through:

* Role-based access control (who can edit or deploy)
* Attribute-based access control (where it can be used)
* Package-based deployment
* Full audit trails

This ensures processes can evolve safely without impacting running or deployed workflows.

***

#### When to Create a New Process

Create a new process when:

* There is a distinct business outcome to achieve
* The workflow spans multiple activities or teams
* Reuse and governance are required

Avoid creating a process for:

* Single-step logic
* Highly reusable execution units (use Activities instead)

#### Diagram / Screenshots

📐 Diagram REQUIRED (High Priority)

Type: Version timeline

&#x20;

Process v1.0 → v1.1 → v2.0 (Locked)\
&#x20;                   ↘ v2.1 (In Progress)

***

####
