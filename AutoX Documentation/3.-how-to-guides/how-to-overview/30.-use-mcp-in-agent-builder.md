# Use MCP in Agent Builder

### Prerequisites

* Access to **Agent Builder**
* Permission to use **MCP Connections**
* An MCP Server already approved and available

> If MCP options are not visible, your role does not have access.

***

### Step 1: Configure MCP Connection (One-Time)

1. Open **Agent Builder**
2. Go to **Settings → MCP Connections**
3. Click **Add MCP Server**
4. Enter MCP server details and save

The MCP server is now available for use across agents (subject to access control).

***

### Step 2: Open an Agent Workflow

1. From **Agent Builder Home**:
   * Open an existing agent, or
   * Create a new agent workflow
2. The **Agent Canvas** opens

***

### Step 3: Use MCP on the Agent Canvas

1. In the **left panel**, use **Search (Ctrl + K)**
2. Add an **MCP-enabled component** to the canvas
3. Select the component and configure:
   * MCP Server
   * Tool exposed by the server
   * Required inputs and outputs

This binds the agent to the selected MCP tool.

***

### Step 4: Control MCP Usage in Agent Logic

In the agent’s configuration:

* Define **when** the agent should use the MCP tool
* Keep MCP usage conditional and intentional

Agents should not invoke MCP tools by default unless required by context.

***

### Step 5: Test Using Playground

1. Open **Playground**
2. Start a test session
3. Provide input that requires tool usage
4. Validate:
   * Agent response
   * Tool invocation behavior

***

### Step 6: Save and Version the Agent

* Save the agent workflow
* Lock the agent version after validation
* Duplicate the agent to make future changes

All MCP usage follows AutoX **versioning and governance rules**.

***

### Key AutoX Guidelines for MCP

* Use MCP **only for agent-driven tool usage**
* Do not use MCP for simple deterministic API calls
* MCP access is governed by **roles and environments**
* All MCP interactions are observable in **Agent Observer**



**Attach Screenshots to show use case of MCP Usage**
