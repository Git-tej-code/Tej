# Task

A **Task** in AutoX represents the **smallest executable unit of work** within an activity. Tasks perform atomic actions such as calling an API, invoking an agent, waiting for an event, executing code, or capturing human input. Together, tasks form the execution logic of an activity.

Tasks are designed to be **simple, focused, and predictable**, ensuring that complex workflows can be composed safely from small, well-defined steps.

***

#### Role of a Task in AutoX

In the AutoX orchestration hierarchy, a task sits at the lowest execution level:

```
Activity
 → Task
```

An activity defines _how multiple tasks are arranged_, while each task defines _what exactly is executed_ at a given step.

***

#### Why Tasks Exist

Tasks exist to ensure:

* **Atomic execution**\
  Each task performs one clear action.
* **Clear data flow**\
  Inputs and outputs are explicitly defined and traceable.
* **Observability**\
  Each task produces logs and execution data.
* **Controlled complexity**\
  Large workflows are built by composing small, manageable units.

***

#### Types of Tasks in AutoX

AutoX provides multiple task types to support different execution needs:

* **Standard Tasks**\
  Core workflow actions such as start, end, and control logic.
* **Connector Tasks**\
  Invoke external systems via integrations and APIs.
* **Agent Tasks**\
  Execute AI agents for reasoning, classification, or generation.
* **Listener Tasks**\
  Wait for external events or messages before continuing.
* **Human Tasks**\
  Pause execution for human input or approval.
* **Subworkflow Tasks**\
  Trigger another process as part of execution.

Each task type is purpose-built and governed.

#### Diagram / Screenshots

📐 Diagram REQUIRED (Medium Priority)

Type: Categorization tree

&#x20;

Tasks\
&#x20;├─ Standard\
&#x20;└─ Custom

***

#### Task Inputs and Outputs

Every task defines:

* **Inputs** received from previous tasks or static values
* **Outputs** passed to downstream tasks

This explicit input/output model ensures:

* Predictable execution
* Easier debugging
* Clear data lineage

***

#### Task Execution and Error Handling

Tasks execute sequentially or conditionally based on the activity logic.\
If a task fails:

* Execution stops (unless handled)
* The failure is logged
* A trace is generated for analysis

Error handling and retries are implemented at the **activity or process level**, not within individual tasks.

***

#### Versioning and Governance

Tasks inherit governance from the activity they belong to:

* Tasks cannot exist outside activities
* Task behavior is versioned through activity versions
* Locked activities ensure task logic cannot change unexpectedly

This guarantees consistent execution across environments.

***

#### When to Use a Task (and When Not To)

**Use a task when:**

* A single, well-defined action is needed
* Integration, agent, or human interaction is required
* Clear inputs and outputs can be defined

**Avoid complex logic in a single task.**\
If logic grows too complex, split it into multiple tasks or activities.
