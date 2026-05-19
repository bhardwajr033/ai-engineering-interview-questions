# You need to choose between a complex agentic system that scores 15% better on benchmarks, or a simpler RAG pipeline that is easier to maintain. How do you decide?

**Topic:** Behavioral and Scenario-Based Questions

## Operational Playbook

Treat this as a production failure mode: reproduce it, constrain the system, improve the weak component, and add evaluation so it does not regress.

Key points:
- Constrain the agent with explicit tool schemas, permissions, max iterations, timeouts, and budgets.
- Log each thought/action/observation in structured traces so failures can be replayed.
- Add human approval for irreversible actions and make dangerous tools idempotent or dry-run by default.

## Example

For example, if a RAG assistant answers without evidence, return `I do not have enough source context` and log the missing-retrieval case for index improvement.

## Current Software Engineering Use Case

Used in enterprise knowledge assistants where employees ask questions over policies, contracts, tickets, and runbooks with citations.
