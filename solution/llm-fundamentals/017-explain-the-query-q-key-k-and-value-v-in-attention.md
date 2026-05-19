# Explain the Query(Q), Key(K), and Value(V) in attention.

**Topic:** LLM Fundamentals

## Source

- [Math behind Attention - Q, K, and V](https://outcomeschool.com/blog/math-behind-attention-qkv)

## Q, K, and V in Attention

Queries, keys, and values are learned projections used by attention to decide what information each token should read.

Key points:
- A query represents what the current token is looking for.
- Keys represent what each token offers for matching.
- Values carry the content that gets mixed together after attention weights are computed from query-key similarity.

## Example

Example: when generating a function body, the current token's query can match keys from the function signature, while values carry the parameter names and types forward.

## Current Software Engineering Use Case

In code generation, a token generating a function argument can attend to earlier function signatures and variable names through Q/K matching, then use V vectors to carry that context forward.
