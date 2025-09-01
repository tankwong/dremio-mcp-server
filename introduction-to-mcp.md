# The Importance of MCP

## What is MCP

Model Context Protocol (MCP) is an open, JSON-RPC-based protocol that standardizes the way any LLM client (an agent, IDE co-pilot, chatbot, etc.) can discover and use resources (read-only data), tools (functions that act), prompts (reusable templates) and sampling (server-initiated completions). There are some very compelling reasons for the introduction of the MCP:
- Decouples Models from Everything Else
    - Current frameworks hard-wire your code to a single LLM vendor and its quirks. MCP introduces a vendor-neutral "socket" so any model (OpenAI, Anthropic, local, or future) can be swapped in without refactoring tools, memory stores, or prompts.
- Standardizes Context Handling
    - Deciding what to feed a model is still an art and an error-prone one. MCP defines a common format for representing, filtering, and prioritizing context (task instructions, retrieved documents, and memory), turning ad-hoc prompt building into a predictable, testable layer.

# Resources and Tools in MCP


# Message Lifecycle in MCP
