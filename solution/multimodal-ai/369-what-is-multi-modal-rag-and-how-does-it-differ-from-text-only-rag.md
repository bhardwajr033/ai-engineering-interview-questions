# What is multi-modal RAG, and how does it differ from text-only RAG?

**Topic:** Multimodal AI

## Retrieval-Augmented Generation

RAG grounds an LLM response by retrieving relevant external context before generation.

Key points:
- The pipeline usually ingests documents, chunks them, embeds chunks, stores vectors, retrieves top matches, optionally reranks them, and prompts the LLM with the selected context.
- RAG is best for changing or private knowledge that should not be baked into model weights.
- Quality depends heavily on parsing, chunking, retrieval, reranking, prompting, and evaluation.

## Example

Example: a user asks about parental leave; the system retrieves the current HR policy chunks and asks the LLM to answer with citations.

## Current Software Engineering Use Case

Enterprise assistants use RAG to answer questions from policies, tickets, contracts, runbooks, and product documentation with citations.
