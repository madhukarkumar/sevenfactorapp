---
description: >-
  This page describes the fourth point of the Seven-Factor Enterprise AI app
  around use of tools and functions for AI agents in a Multi-Agent RAG Systems
  (MARS).
---

# IV. Dynamic Tools, Upgradeable Skills

A tool is typically an API endpoint that can be invoked remotely (for example REST) or through a function that has been implemented for a specific task or action, for example, vectorizing a given input stream or scraping a web site or retrieving a specific piece of information across a specific data set. All tools must follow the enterprise's security standards for authorization and authentication with audit and rate limiting capabilities.

A function used as a tool should ideally return information using the[ OpenAPI schema](https://swagger.io/specification/) to ensure standardization of communication between and through different agents. Each tool should be independently upgradeable and deployable.&#x20;

For large enterprises, the tools should be discoverable through a catalog and developers should be able to create new or encapsulate functionalities within the Tools OpenAPI schema and publish to the catalog, similar to docker containers.&#x20;

A collection of specific tools, along with specific prompt and fine tuned domain-specific knowledge (data) can be encapsulated as a skill for an agent. For example, an agent that has access to keyword research API, web scraping APIs, web analytics APIs and access to fine tuned LLM with specific prompt could be referred to a an Agent with the enterprise SEO skill.&#x20;
