---
description: >-
  This page defines the seventh point of the Seven-Factor Enterprise AI apps as
  an independent layer for interacting with Multi-Agent RAG Systems (MARS)
---

# VII. User Experience for Agents

A Seven-Factor Enterprise AI App uses a disaggregrated UI layer that fall under one or several of the User Experience (UX) paradigms of interacting with Multi-Agent Systems.

1. **Information Retrieval Use Cases** - The most common user experience is this scenario is a conversational user interface with with the following mechanisms available for input - a structured file like csv, an audio file or an image or pdf or a video. The input should ALWAYS be explicitly provided by the user and never be automatically added (for example audio or vision without the user's explicit knowledge and approval).  The output typically consists of streaming text and when appropriate, rich information in the form or analytical charts and widgets with actionable buttons and the ability to persist them within a web page. The rich output may also include audio and video files that can be persisted by the users.&#x20;
2. **Agentic Use Cases** - When an action needs to be performed, a widget or a command line explicitly requiring users to approve the action should be used. In order to receive approval, the agent or the system should explicitly describe what will happen as part of the action. Each of these approvals should then be recorded for audit requirements.&#x20;
3. **Build Use Cases** - In an enterprise, developers from different teams are required to build apps, services and automation across multiple data sets and by utilizing services built by other teams. In  these scenarios, developers should have a way to discover tools, services and access to data catalog. When appropriate, they should also be able to use templatized notebooks or microservices to build applications, services and workflow and debug and deploy independently using company standards.
