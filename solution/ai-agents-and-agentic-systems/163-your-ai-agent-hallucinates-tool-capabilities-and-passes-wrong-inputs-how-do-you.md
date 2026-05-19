# Your AI agent hallucinates tool capabilities and passes wrong inputs. How do you fix it?

**Topic:** AI Agents and Agentic Systems

## Operational Playbook

Treat this as a production failure mode: reproduce it, constrain the system, improve the weak component, and add evaluation so it does not regress.

Key points:
- Ground the answer in retrieved or supplied evidence and require citations.
- Add an abstention path with confidence thresholds: if evidence is missing or contradictory, say that the answer is not known.
- Evaluate faithfulness separately from fluency using adversarial and no-answer examples.
- Constrain the agent with explicit tool schemas, permissions, max iterations, timeouts, and budgets.
- Log each thought/action/observation in structured traces so failures can be replayed.
- Add human approval for irreversible actions and make dangerous tools idempotent or dry-run by default.

## Example

For example, if a RAG assistant answers without evidence, return `I do not have enough source context` and log the missing-retrieval case for index improvement.

## Current Software Engineering Use Case

Used by software teams building ai agents and agentic systems features that must balance quality, latency, cost, safety, and maintainability.
