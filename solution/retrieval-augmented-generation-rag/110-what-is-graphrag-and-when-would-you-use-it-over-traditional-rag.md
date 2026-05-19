# What is GraphRAG, and when would you use it over traditional RAG?

**Topic:** Retrieval-Augmented Generation (RAG)

## Source

- [GraphRAG](https://outcomeschool.com/blog/graphrag)

## GraphRAG

GraphRAG augments retrieval with a graph of entities, relationships, and communities extracted from documents.

Key points:
- It is useful when answers require connecting facts across many documents.
- Graph structure can improve global summaries, relationship questions, and conflict analysis.
- It costs more to build and maintain than plain vector search, so it should be used when relationships matter.

## Example

Example: build a graph linking services, owners, incidents, and dependencies so the assistant can answer relationship-heavy outage questions.

## Current Software Engineering Use Case

An enterprise knowledge assistant can use GraphRAG to answer questions like which services, owners, incidents, and dependencies relate to a major outage.
