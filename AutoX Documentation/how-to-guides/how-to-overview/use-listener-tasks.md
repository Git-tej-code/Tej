# Use Listener Tasks

**Who can do this**

* Platform Admin
* Power User

&#x20;

**What is a Listener Task?**

A Listener Task waits for an external event before proceeding.

Common use cases:

* Webhook triggers
* Message queues
* External system callbacks

&#x20;

**Steps**

1. Drag Listener Task into the activity
2. Configure:
3. Event type
4. Channel or source
5. Timeout (if applicable)
6. Connect it to the workflow
7. Click Save

&#x20;

**What Happens Next**

* Activity pauses at listener
* Execution resumes when event is received

&#x20;

**Important Notes**

* Listener tasks are event-driven
* Timeouts must be defined carefully
* All events are logged

&#x20;

📸 Screenshot Required

* Listener Task configuration screen
