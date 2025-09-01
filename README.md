# Dremio MCP Server (Source: [Dremio University](https://university.dremio.com/path-player?courseid=dremio-mcp&unit=6807a2a7d0f7b759600cd7d8Unit))

Model Context Protocol (MCP) is an open, JSON-RPC-based protocol that sits between large-language-model (LLM) clients (agents, IDE copilots, chatbots, etc.) and the external "stuff" they need-files, APIs, shell commands, prompt templates, and even other models. It defines one consistent way to expose four kinds of capabilities:
- **Resources**: Things the model can read (logs, code, database rows, and screenshots)
- **Tools**: Callable functions with typed inputs/outputs that the model can invoke
- **Prompts**: Reusable prompt templates the user can trigger
- **Sampling**: Server-side code can ask the host's model to generate a completion

These capabilities are hosted on servers - either local scripts or cloud services. A client running inside a host (the app that embeds the LLM) maintains a single connection to each server, translating messages over either stdio or HTTP with Server-Sent-Events (SSE). The many to many relationship between clients and servers means any model can mix and match tools or data sources without bespoke glue code.

## Prerequisites

This assumes familiarity with the following concepts:
- Setting up local Python environments, including installing dependencies
- Writing new Python code and reviewing the provided code
- Popular LLMs and how they support AI agents
- Working Dremio environment with an API key

## Introduction to MCP ([link](introduction-to-mcp.md))

## The Dremio MCP Server ([link](dremio-mcp-server.md))