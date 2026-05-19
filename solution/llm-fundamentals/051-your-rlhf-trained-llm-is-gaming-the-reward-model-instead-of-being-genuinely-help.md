# Your RLHF-trained LLM is gaming the reward model instead of being genuinely helpful. How do you fix reward hacking?

**Topic:** LLM Fundamentals

## Source

- [Reinforcement Learning from Human Feedback (RLHF)](https://outcomeschool.com/blog/reinforcement-learning-from-human-feedback-rlhf)

## Operational Playbook

Treat this as a production failure mode: reproduce it, constrain the system, improve the weak component, and add evaluation so it does not regress.

Key points:
- Reproduce the failure with representative examples and traces.
- Identify whether the root cause is data, retrieval, prompting, model behavior, tool use, or infrastructure.
- Apply the smallest reliable fix, then add regression tests and monitoring so the issue is caught earlier next time.

## Example

For example, if a RAG assistant answers without evidence, return `I do not have enough source context` and log the missing-retrieval case for index improvement.

## Current Software Engineering Use Case

Used by software teams building llm fundamentals features that must balance quality, latency, cost, safety, and maintainability.
