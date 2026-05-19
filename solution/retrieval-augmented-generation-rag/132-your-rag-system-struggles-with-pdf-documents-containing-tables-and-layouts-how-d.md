# Your RAG system struggles with PDF documents containing tables and layouts. How do you fix PDF parsing?

**Topic:** Retrieval-Augmented Generation (RAG)

## Operational Playbook

Treat this as a production failure mode: reproduce it, constrain the system, improve the weak component, and add evaluation so it does not regress.

Key points:
- Do not send the full input blindly; parse, chunk, retrieve, summarize, or process with a map-reduce workflow.
- Use layout-aware parsing for PDFs and preserve table structure, headings, page numbers, and metadata.
- Track token budgets for prompt, retrieved context, tool output, and response.

## Example

For example, if a RAG assistant answers without evidence, return `I do not have enough source context` and log the missing-retrieval case for index improvement.

## Current Software Engineering Use Case

Used in enterprise knowledge assistants where employees ask questions over policies, contracts, tickets, and runbooks with citations.
