# Your model passes one fairness metric but fails another. How do you handle conflicting audit results?

**Topic:** Evaluation and Testing

## Operational Playbook

Treat this as a production failure mode: reproduce it, constrain the system, improve the weak component, and add evaluation so it does not regress.

Key points:
- Measure outcomes across protected and intersectional groups, not only aggregate accuracy.
- Remove or constrain proxy features, rebalance data, and involve domain/legal review.
- Monitor drift after deployment and provide appeal paths for affected users.

## Example

For example, if a RAG assistant answers without evidence, return `I do not have enough source context` and log the missing-retrieval case for index improvement.

## Current Software Engineering Use Case

Used by software teams building evaluation and testing features that must balance quality, latency, cost, safety, and maintainability.
