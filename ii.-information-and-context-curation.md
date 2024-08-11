# II. Information and Context Curation

A typical enterprise consists of multiple databases, data sources and ETL pipelines. However, in a gen AI application if the LLM does not have access to the most current information, it runs the risk of returning information that is inaccurate or running an action that is no longer needed, for example creating a customer support ticket when an issue was resolved based on a real-time conversation with a customer support representative.

A Seven-Factor App is designed to provide the most relevant and accurate information to LLMs and Agents in a few milliseconds in one round-trip query by searching across ALL data in an enterprise. Due to this requirement, the Seven-Factor App recommends one single data assimilation layer that can be queried with both semantic and exact keyword matches and the data is returned in a structured format.  This data layer should have access to the enterprise's structured (for example, Iceberg data) and unstructured data (for example, binary files and pdfs) across both transactional and data warehouses, data lakes, data lake houses data.&#x20;

The information layer thus should have the following components accessible for Retrieval Augmented Generation (RAG) retrievers and agents:

1. Real-time Change Data Capture (CDC) in and out from different data sources.
2. Ability to store vector data for unstructured data along with relational, hierarchical and structured data.
3. Ability to define optimized structured queries that can be called as functions from agents and APIs, tools.
4. Ability to run hybrid search including vector functions along with keyword search and analytics (aggregate functions) across all data ideally in single round-trip hops.
5. The information layer should have the capability to match existing corpus of enterprise data with fast emerging streaming real-time data to provide effective contextualization for LLMs.
6. The information layer should be able to honor data access, governance and policy and audit requirements of the enterprise.
7. For certain use cases, the information layer should be able to provide a catalog of all data available.
8. The information layer should provide a way for developers and data engineers to discover data through published meta data, create prototypes of applications (for example Jupyter notebooks) and the ability to deploy data apps as microservices that are resilient to underlying schema changes (for example, through the use of materialized views).
9. The information layer should provide branching as a feature to enable viewing and iterating over different versions of data states.
10. The information layer should also allow persisting feedback of query responses from different agents and apps that can then be enriched with Reinforced Learning from Human Feedback (RLHF) and then continuously fine tune certain LLMs.
