# Your LLM generates responses that are too verbose. How do you control response length?

**Topic:** LLM Fundamentals

## Operational Playbook

Treat this as a production failure mode: reproduce it, constrain the system, improve the weak component, and add evaluation so it does not regress.

Key points:
- Specify a response budget, structure, and stopping rules in the prompt.
- Use schema fields with maximum lengths where possible.
- Evaluate length compliance and add retries or truncation only after semantic validation.

## Example

For example, if a RAG assistant answers without evidence, return `I do not have enough source context` and log the missing-retrieval case for index improvement.

## Current Software Engineering Use Case

Used by software teams building llm fundamentals features that must balance quality, latency, cost, safety, and maintainability.
