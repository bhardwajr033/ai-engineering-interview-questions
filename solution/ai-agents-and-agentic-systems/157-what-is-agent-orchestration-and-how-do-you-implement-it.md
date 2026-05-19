# What is agent orchestration, and how do you implement it?

**Topic:** AI Agents and Agentic Systems

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
