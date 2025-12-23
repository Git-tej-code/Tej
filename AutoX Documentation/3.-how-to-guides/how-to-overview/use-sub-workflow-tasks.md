# Use Sub-workflow Tasks

**Who can do this**

* Platform Admin
* Power User

&#x20;

**What is a Subworkflow Task?**

A Subworkflow Task executes another Process within an activity.

Use cases:

* Reuse common logic
* Modularize large workflows

&#x20;

**Steps**

1. Drag Subworkflow Task into the activity
2. Select the target Process
3. Map required inputs
4. Configure output handling
5. Click Save

&#x20;

**What Happens Next**

* Child process executes within parent context
* Execution trace links parent and child

&#x20;

**Important Notes**

* Circular dependencies are not allowed
* Subworkflow versions are locked at runtime
* Logs are visible across both processes

&#x20;

📸 Screenshot Required

* Subworkflow task configuration
