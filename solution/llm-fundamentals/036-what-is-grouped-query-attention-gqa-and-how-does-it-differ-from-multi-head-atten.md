# What is Grouped-Query Attention (GQA), and how does it differ from Multi-Head Attention (MHA)?

**Topic:** LLM Fundamentals

## Source

- [Grouped Query Attention](https://outcomeschool.com/blog/grouped-query-attention)

## Attention Head Variants

Multi-head attention runs multiple attention heads in parallel; GQA shares key/value heads across groups of query heads.

Key points:
- Multiple heads let the model attend to different syntactic, semantic, and positional relationships.
- MHA gives each query head its own key and value projections, which is expressive but memory-heavy.
- GQA reduces KV-cache size and inference bandwidth while preserving much of MHA quality.

## Example

Example: one attention head may track syntax, another may track entity references, and GQA can share key/value heads to reduce serving memory.

## Current Software Engineering Use Case

Serving teams use GQA in chat models to reduce memory pressure and increase tokens-per-second during high-volume inference.
