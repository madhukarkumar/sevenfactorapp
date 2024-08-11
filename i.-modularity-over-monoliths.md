---
description: >-
  Step 1 of the seven-factor enterprise app that describes building enterprise
  gen AI app in a modular way similar to microservices.
---

# I. Modularity Over Monoliths

The Seven-Factor App is inherently modular and follows the best practices of microservices architecture. This enables iterative changes, deployment and scalability at scale. Modularity can be achieved by either packaging coherent set of functionalities as microservices but an emerging architecture specifically for generative AI applications is preferred called Multi-Agent RAG Systems (MARS).

MARS enables building AI Agents that are capable of both Reasoning and Action (ReACT agents) and built with collaborating at scale with other agents.&#x20;

A typical ReACT agent consists of three primary constructs:&#x20;

1. Intelligence - Access to one or more LLMs.
2. Tools - Access to receptors and effectors through webhooks and APIs.
3. Knowledge - Access to both structured and unstructured data specific to the agent's goals and objectives.&#x20;

An agent also maintains state or has both long-term and short-ter "memory" that can be encapsulated within knowledge.

### Collaboration

As of writing this document, there are two primary ways of collaboration between agents.&#x20;

1. **Supervisor and Worker collaboration** - In this method, the supervisor assigns tasks to other agents, collates and then either returns the information and/or completes and action. In this method, the results are non-deterministic and not always explainable which is why the second method is more appropriate for enterprise use cases.
2. **Sequential workflows -** In this method, a workflow or graph consists of nodes and edges. The nodes could be agents that are called based on sequential algorithm and executed based on the graph/workflow overall requirement. In this method, there is more control but requires more effort to build and continue to maintain and iterate based on changing requirements.

