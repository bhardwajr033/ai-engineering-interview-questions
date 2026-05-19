# What are chunking strategies, and how do you choose the right chunk size?

**Topic:** Retrieval-Augmented Generation (RAG)

## Chunking

Chunking splits documents into retrievable units for search and generation.

Key points:
- Fixed-size chunking is simple but can split related ideas.
- Recursive chunking respects structure such as headings, paragraphs, and sentences.
- Semantic chunking groups text by meaning, while parent-child chunking retrieves small child chunks and sends larger parent context to the model.

## Example

Example: split a runbook by headings and procedures, not every 500 characters, so each retrieved chunk contains a complete operational step.

## Current Software Engineering Use Case

A documentation Q&A system tunes chunk size and overlap to maximize answer faithfulness while minimizing redundant context.
