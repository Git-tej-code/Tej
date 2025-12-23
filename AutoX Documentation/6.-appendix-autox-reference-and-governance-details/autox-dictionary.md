# AutoX Dictionary

### Agent

An intelligent execution component capable of reasoning, interpreting context, and producing non-deterministic outcomes using language models, tools, and memory. Agents are invoked through **Agent Tasks** and are always governed, versioned, and observable.

***

### Agent Builder

A dedicated interface within AutoX used to create, test, version, and manage agents. It provides a visual canvas, component library, playground for testing, MCP integration, and agent-specific settings.

***

### Agent Observer

A specialized observability interface that provides deep visibility into agent and workflow execution, including traces, sessions, cost, latency, and quality metrics.

***

### Agent Task

A task type used within an activity to invoke an agent. It passes structured inputs to the agent and receives structured outputs, ensuring agent behavior is traceable and governed.

***

### Attribute-Based Access Control (ABAC)

An access control mechanism that restricts actions based on contextual attributes such as organization, department, environment, or deployment stage. ABAC works alongside RBAC in AutoX to enforce fine-grained governance.

***

### Activity

A reusable unit of execution logic that defines _how work is performed_. Activities contain tasks and are orchestrated by processes. They are versioned, lockable, and reusable across multiple processes.

***

### Audit Log

An immutable record of sensitive actions such as role changes, deployments, configuration updates, and access modifications. Audit logs support compliance and forensic analysis.

***

### Connector Task

A task type used to call external systems through a configured integration. Connector tasks handle deterministic API interactions and should be preferred over MCP when logic is rule-based.

***

### Custom Role

A role defined by administrators to provide tailored access that does not fully align with default roles. Custom roles allow fine-grained permission control while preserving AutoX governance rules.

***

### Department

A structural unit representing a business domain or organizational area (e.g., Finance, HR, IT). Departments group functions and provide ownership boundaries.

***

### Deployment

The controlled promotion of a package into an environment (such as UAT or Production). Deployment in AutoX always happens through packages and never directly from editable artefacts.

***

### Environment

A logical boundary representing stages such as Development, UAT, or Production. Access, integrations, and deployments may differ by environment.

***

### Function

A business capability within a department (e.g., Invoice Processing, Claims Handling). Functions group related processes.

***

### Human Task

A task type that pauses execution and waits for human input or approval. Human tasks allow human-in-the-loop automation while maintaining auditability.

***

### Integration

A governed configuration that defines how AutoX connects to an external system or service. Integrations centralize endpoints, authentication, and parameters for secure reuse.

***

### Listener Task

A task that waits for an external event or message to trigger execution. Listener tasks are commonly used in event-driven automation.

***

### Lock

A governance action that freezes an artefact (process, activity, agent, or package) to prevent further modification. Locked artefacts ensure execution stability.

***

### MCP (Model Context Protocol)

A standardized protocol that allows agents to securely discover and use external tools through MCP servers. MCP decouples agent logic from tool implementation while preserving observability and control.

***

### MCP Client

The component within AutoX (used by agents) that connects to an MCP server to request tool execution.

***

### MCP Server

An external or internal service that exposes tools or capabilities to agents via MCP. MCP servers enforce access rules and input/output contracts.

***

### Observability

The ability to understand system behavior through traces, logs, metrics, cost, latency, and quality data. Observability in AutoX applies to both workflows and agents.

***

### Package

An immutable deployment unit that bundles specific versions of processes, activities, agents, and configurations. Packages are the only artefacts that can be deployed.

***

### Playground

A chat-based testing interface in Agent Builder used to test agents interactively. Playground sessions are logged and observable.

***

### Process

An end-to-end business workflow that orchestrates activities to achieve a defined outcome. Processes define _what happens_ and _in what order_, not execution details.

***

### RBAC (Role-Based Access Control)

An access control model where permissions are granted based on user roles. RBAC defines _what a user can do_ in AutoX.

***

### Scheduler

A mechanism used to trigger processes based on time or events. AutoX supports time-based and event-based scheduling.

***

### Session

A logical grouping of related interactions, especially in conversational or agent-driven workflows. Sessions help track multi-step agent behavior.

***

### Span

A single execution unit within a trace, such as a task execution, agent call, or integration invocation.

***

### Task

The smallest executable unit in AutoX. Tasks perform atomic actions and are composed inside activities.

***

### Trace

A complete, end-to-end execution record of a process or agent interaction. Traces provide visibility into execution flow, timing, cost, and failures.

***

### Version

A specific, immutable snapshot of an artefact (process, activity, agent). New changes always create a new version.

***

### Versioning (Sacred Principle)

A core AutoX principle where artefacts are never overwritten or deleted. All changes result in new versions, enabling auditability and safe rollback.

***

### WorkJam

A design interface used to model processes at a business level. WorkJam focuses on flow and intent rather than execution logic.

***

### Workflow

A generic term referring to the coordinated execution of processes, activities, tasks, and agents to achieve a business goal.

***

### Final Note

This dictionary is intentionally:

* **Precise**
* **Non-overlapping**
* **Governance-aware**
* **Enterprise-ready**

It can be safely shared with:

* Customers
* Auditors
* Partners
* Internal teams

###
