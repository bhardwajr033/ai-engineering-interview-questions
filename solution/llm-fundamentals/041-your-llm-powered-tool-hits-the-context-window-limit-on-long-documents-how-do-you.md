# Your LLM-powered tool hits the context window limit on long documents. How do you handle it?

**Topic:** LLM Fundamentals

## Operational Playbook

Treat this as a production failure mode: reproduce it, constrain the system, improve the weak component, and add evaluation so it does not regress.

Key points:
- Do not send the full input blindly; parse, chunk, retrieve, summarize, or process with a map-reduce workflow.
- Use layout-aware parsing for PDFs and preserve table structure, headings, page numbers, and metadata.
- Track token budgets for prompt, retrieved context, tool output, and response.
- Constrain the agent with explicit tool schemas, permissions, max iterations, timeouts, and budgets.
- Log each thought/action/observation in structured traces so failures can be replayed.
- Add human approval for irreversible actions and make dangerous tools idempotent or dry-run by default.

## Example

For example, if a RAG assistant answers without evidence, return `I do not have enough source context` and log the missing-retrieval case for index improvement.

## Current Software Engineering Use Case

Used in enterprise knowledge assistants where employees ask questions over policies, contracts, tickets, and runbooks with citations.
