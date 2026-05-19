# What is Model Context Protocol (MCP), and how does it standardize tool integration?

**Topic:** AI Agents and Agentic Systems

## Source

- [AI Engineering Explained: LLM, RAG, MCP, Agent, Fine-Tuning, Quantization](https://www.youtube.com/watch?v=lnfWvX66FUk)
  - Transcript notes: the video frames AI engineering around six practical building blocks: LLMs for language generation, RAG for grounding answers in external knowledge, MCP for standardized tool/data integration, agents for goal-directed tool use, fine-tuning for behavior or domain adaptation, and quantization for cheaper deployment.

## Model Context Protocol

MCP is a standard protocol for connecting AI applications to tools, resources, and prompts exposed by external servers.

Key points:
- It separates the model client from tool-provider implementation details.
- Servers can expose filesystem, database, SaaS, or internal API capabilities in a consistent shape.
- Standardization reduces one-off integrations and makes tools reusable across clients.

## Example

Example: expose GitHub issues, database queries, and filesystem resources as MCP servers so multiple AI clients can use the same tools.

## Current Software Engineering Use Case

A developer assistant can use MCP servers for GitHub, Slack, calendars, local files, and internal services through the same integration model.
