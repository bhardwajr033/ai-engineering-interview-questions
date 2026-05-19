# Your summarization system hallucinated facts not in the original article. How do you fix it?

**Topic:** LLM Fundamentals

## Operational Playbook

Treat this as a production failure mode: reproduce it, constrain the system, improve the weak component, and add evaluation so it does not regress.

Key points:
- Ground the answer in retrieved or supplied evidence and require citations.
- Add an abstention path with confidence thresholds: if evidence is missing or contradictory, say that the answer is not known.
- Evaluate faithfulness separately from fluency using adversarial and no-answer examples.

## Example

For example, if a RAG assistant answers without evidence, return `I do not have enough source context` and log the missing-retrieval case for index improvement.

## Current Software Engineering Use Case

Used by software teams building llm fundamentals features that must balance quality, latency, cost, safety, and maintainability.
