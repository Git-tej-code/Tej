# Agent Errors

1. **Agent returns unexpected results**

**Cause**

* Prompt design issue
* Incorrect input mapping
* Model selection mismatch

**Resolution**

* Test agent in Playground
* Review input payload in trace
* Evaluate agent output quality using Observer

&#x20;

2. **Agent execution is slow or costly**

**Cause**

* Model latency
* Large context size
* Looping or repeated calls

**Resolution**

* Analyze latency and cost charts
* Review span-level breakdown
* Optimize prompt or model choice
