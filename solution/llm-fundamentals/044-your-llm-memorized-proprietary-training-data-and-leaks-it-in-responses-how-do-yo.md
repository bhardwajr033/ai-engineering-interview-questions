# Your LLM memorized proprietary training data and leaks it in responses. How do you prevent this?

**Topic:** LLM Fundamentals

## Operational Playbook

Treat this as a production failure mode: reproduce it, constrain the system, improve the weak component, and add evaluation so it does not regress.

Key points:
- Minimize sensitive data sent to the model and redact secrets before inference.
- Treat system prompts as policy hints, not secrets; enforce real authorization outside the model.
- Add prompt-injection tests, output filters, and logging for attempted exfiltration.

## Example

For example, if a RAG assistant answers without evidence, return `I do not have enough source context` and log the missing-retrieval case for index improvement.

## Current Software Engineering Use Case

Used by software teams building llm fundamentals features that must balance quality, latency, cost, safety, and maintainability.
