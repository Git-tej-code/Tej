---
description: AutoX Platform – Product Usage Documentation (One-Page Summary)
---

# How to Use  This Documentation?

**Overview**

AutoX is an enterprise-grade, agentic automation platform designed to orchestrate business processes, AI agents, integrations, and human decision points with strong governance, observability, and version control.

This documentation serves as a complete usage guide for users, builders, administrators, and observers to design, deploy, monitor, and govern intelligent automation using AutoX.

&#x20;

**Documentation Structure**

The documentation is organized into five logical phases, each addressing a distinct user need:

1. Introduction & Getting Started\
   Introduces AutoX, its vision, platform components, login flows, and navigation. Helps new users understand where to work (Main Platform, Agent Builder, Agent Observer) and how AutoX differs from traditional automation tools.
2. AutoX Fundamentals\
   Explains core concepts such as:
3. Orchestration hierarchy (Department → Function → Process → Activity → Task)
4. Agents and agentic execution
5. Integrations and credential governance
6. Packages, versioning, and deployment philosophy
7. Observability concepts (Traces, Spans, Sessions)\
   This section answers what AutoX is and why it works this way.
8. How-To Guides (Operational Usage)\
   Step-by-step instructions for:
9. Creating departments and functions
10. Designing and developing processes and activities
11. Using tasks (human, connector, agent, subworkflow)
12. Building and testing agents in Agent Builder
13. Configuring integrations
14. Managing packages and deployments
15. Observing executions, cost, latency, and quality in Agent Observer\
    This is the primary working section for daily users.
16. Roles, Access & Governance\
    Defines AutoX’s RBAC + ABAC access model, including:
17. Super Admin
18. Platform Admin
19. Power User
20. Agent Developer
21. Business User\
    It documents:
22. Who can do what
23. Why some actions are restricted
24. Versioning and deployment governance
25. Audit logs and system performance controls
26. Troubleshooting & FAQ\
    Provides categorized troubleshooting for:
27. Common errors and system messages
28. Access-denied issues
29. Locked or archived items
30. Failed executions
31. Agent and integration failures\
    Includes FAQs addressing versioning, rollback, roles, AI behavior, security, and cost visibility.

&#x20;

**Key Platform Principles Captured**

* Versioning is sacred: No deletion of core artefacts; rollback via redeployment.
* Governance-first design: Safety, auditability, and compliance over convenience.
* Hybrid automation: Deterministic workflows combined with intelligent agents.
* Separation of concerns: Clear boundaries between orchestration, AI, integration, and observation.
* Enterprise observability: Every execution is traceable, measurable, and auditable.

&#x20;

**Intended Audience**

* New users onboarding to AutoX
* Power users and builders designing automation
* Agent developers building AI-driven logic
* Admins managing access, deployment, and governance
* Stakeholders reviewing platform capabilities and controls

&#x20;

**Outcome**

By following this documentation, a user can:

* Confidently design and deploy intelligent automation
* Safely use AI agents within governed workflows
* Integrate external systems without breaking compliance
* Monitor cost, latency, and quality
* Operate AutoX at enterprise scale with clarity and control
