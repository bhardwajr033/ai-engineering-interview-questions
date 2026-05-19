# Explain the architecture of a basic RAG system.

**Topic:** Retrieval-Augmented Generation (RAG)

## Source

- [AI Engineering Explained: LLM, RAG, MCP, Agent, Fine-Tuning, Quantization](https://www.youtube.com/watch?v=lnfWvX66FUk)
  - Transcript notes: the video frames AI engineering around six practical building blocks: LLMs for language generation, RAG for grounding answers in external knowledge, MCP for standardized tool/data integration, agents for goal-directed tool use, fine-tuning for behavior or domain adaptation, and quantization for cheaper deployment.

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
