# Activity

An **Activity** in AutoX represents a **reusable unit of execution logic** that performs a well-defined part of a business process. Activities encapsulate how work is executed—through tasks, integrations, agents, and human interactions—while remaining independent of any single process.

Activities are the primary mechanism AutoX uses to achieve **modularity, reuse, and governance** across automation.

***

#### Role of an Activity in AutoX

In the AutoX orchestration hierarchy, an activity sits between **Processes** and **Tasks**:

```
Process
 → Activity
   → Task
```

A process orchestrates _when_ an activity runs, while the activity defines _how_ that work is performed.

***

#### Why Activities Exist

Activities exist to solve three core problems:

1. **Reuse**\
   The same activity can be used across multiple processes without duplication.
2. **Separation of Concerns**\
   Processes remain high-level and readable, while activities contain execution logic.
3. **Governance & Safety**\
   Changes to execution logic are versioned, reviewed, and controlled.

***

#### What an Activity Contains

An activity typically contains:

* A sequence of **Tasks**
* Conditional logic and branching
* Integration calls
* Agent invocations
* Human tasks (where required)

Activities do **not** define business ownership or deployment rules—that responsibility remains with processes and packages.

***

#### Activity Design Principles

Effective activities follow these principles:

* Focus on **one responsibility**
* Be **reusable across processes**
* Avoid embedding business-specific routing logic
* Keep agent usage intentional and controlled

If an activity grows too large, it should be split into smaller activities or subworkflows.

***

#### Versioning and Lifecycle

Every activity in AutoX is:

* Automatically versioned
* Immutable once locked
* Never deleted

Typical lifecycle:

```
Created → In Progress → Locked → Used by Processes → Archived
```

Processes always reference a **specific version** of an activity, ensuring predictable execution.

***

#### Activities and Human Interaction

Activities are the correct place to introduce **Human Tasks**, such as:

* Approvals
* Reviews
* Manual decisions

This allows human involvement to be governed, audited, and resumed cleanly within automation.

***

#### When to Use an Activity (and When Not To)

**Use an activity when:**

* Logic needs to be reused
* Execution involves multiple steps
* Integration or agent logic is required

**Avoid activities for:**

* Single-step actions
* Business flow definitions (use processes instead)
