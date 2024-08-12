---
description: >-
  The page describes the fifth point of the Seven-Factor Enterprise AI App
  around orchestration and collaboration among AI agents in the Multi-Agent RAG
  System (MARS).
---

# V. Collaboration and Orchestration at Scale

In a Seven-Factor App, there are primarily two big categories of collaboration with AI agents.

1. **Role-based collaboration** - In this method, agents have different roles. A task is decomposed into smaller tasks and assigned based on roles. The output is then verified, critiques and assimilated by other role based agents and then returned as an output. Role-based collaboration work well when dealing with asynchronous goals and objectives and does not have real-time response requirements.&#x20;
2. **Workflow-based orchestration** - In this method, the sequence of task is defined as a workflow or graph. The workflow consists of nodes and edges. A node could be a task or represent an agent with skills and knowledge to do a specific task. The workflow also has conditional branches and loops to ensure the sequence of tasks happen in a certain order based on enterprise rules - for example, create embeddings only after the raw data has been summarized and categorized. A workflow based orchestration can also invoke certain tasks in parallel for faster response times.

One of the key requirements of agent collaboration is the ability to observe and record the communication and actions between agents that can then be enriched with human feedback for further long-term optimization and also for audit requirements.
