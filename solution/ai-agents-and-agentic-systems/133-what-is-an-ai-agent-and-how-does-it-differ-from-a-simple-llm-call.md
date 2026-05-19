# What is an AI agent, and how does it differ from a simple LLM call?

**Topic:** AI Agents and Agentic Systems

## Source

- [AI Engineering Explained: LLM, RAG, MCP, Agent, Fine-Tuning, Quantization](https://www.youtube.com/watch?v=lnfWvX66FUk)
  - Transcript notes: the video frames AI engineering around six practical building blocks: LLMs for language generation, RAG for grounding answers in external knowledge, MCP for standardized tool/data integration, agents for goal-directed tool use, fine-tuning for behavior or domain adaptation, and quantization for cheaper deployment.
- [AI Agent Explained](https://outcomeschool.com/blog/ai-agent)

## AI Agents

An AI agent is an LLM-powered system that can plan, call tools, observe results, update state, and continue until a goal is reached.

Key points:
- A simple LLM call returns one response; an agent runs a controlled loop around model decisions and external actions.
- Core parts include instructions, tools, memory/state, planning strategy, termination conditions, and guardrails.
- Agents need observability and limits because tool use can fail, loop, or take harmful actions.

## Example

Example: a research agent can search the web, read documents, write notes, and stop when it has enough cited evidence.

## Current Software Engineering Use Case

Engineering teams build agents for code migration, support triage, research workflows, data analysis, and operations automation.
