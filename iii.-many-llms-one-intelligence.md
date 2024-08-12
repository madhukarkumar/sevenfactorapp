---
description: >-
  This page describes the 3rd point of the Seven-Factor Enterprise AI app around
  use of disaggregated LLMs in Multi-Agent RAG Systems (MARS) to maintain model
  and provider agnosticism.
---

# III. Many LLMs, One Intelligence

Due to the first principle of modularity of the Seven-Factor App, an enterprise generative AI application should not rely on one single provider, model or version of a Large Language Model (LLM). There are several reasons for this but the three most common ones include

1. The evolution for fast LLM model iterations.
2. Pricing.
3. Requirements of certain agents and information to reside locally in a VPC or in a geo.
4. The requirement to fine-tune smaller models for highly specific tasks.

The ensemble of LLMs can be spread across multiple agents or similar to the information layer be discoverable, fine tuned and then deployed using technologies similar to AWS's Bedrock, Azure AI Studio, Nvidia's Inference Microservices (NIMs) platform or Google's Vertex AI.&#x20;

A Seven-Factor App may include either a specialized agent, graph or an LLM router to dynamically route queries and requests to other agents or LLMs.
