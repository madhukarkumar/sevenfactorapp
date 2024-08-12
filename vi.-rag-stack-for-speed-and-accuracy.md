---
description: >-
  This page describes the sixth point of the Seven-Factor Enterprise AI app
  around the requirements of latency, accuracy and relevancy across Multi-Agent
  RAG Systems (MARS)
---

# VI. RAG Stack for Speed and Accuracy

A Seven-Factor App requires Retrieval Augment Generation (RAG) tech stack that fullfils the following requirements:

1. **Safety, Security and Privacy** - Any query or request to an agent or a workflow should first be handled by guardrails that records, makes a design and acts on whether that task or information should proceed to the next step. This should happen both at input and output. These safety, security and data privacy rules should be adhered to based on the enterprise's codified rules for example, masking certain kinds of data, guardrails to prevent insecure or unauthorized data access etc.&#x20;
2. **Accuracy and Relevancy** - Input queries should be enriched with context by asking questions, seeking clarification and approval when appropriate and needed (for example, before running a command). For accuracy, the app must take advantage of re-ranking, evaluations, fine-tuning with RLHF as methods at output validation. In addition, care should be taken to use fine-tuned embedding models and matching LLMs to ensure the information is vectorized (when needed) and retrieved for highly contextualized information. Guardrails should also be enforced to reject retrieval queries not related to enterprise corpus of data.
3. **Speed and Scalability** - A RAG stack should be capable of querying and retrieving data across multiple datatypes, multiple data stores (Lakehouses and transactional DBs), use both vector and keyword match search across of petabytes of data and with latency of less than a second as listed under the [second point](ii.-information-and-context-curation.md) of the Seven-Factor App. Semantic caching, use of local GPU based inference microservices, and memory-first architectures should be used to achieve sub-second latency.&#x20;
