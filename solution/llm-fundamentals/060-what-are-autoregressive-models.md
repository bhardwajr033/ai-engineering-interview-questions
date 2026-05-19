# What are Autoregressive Models?

**Topic:** LLM Fundamentals

## Source

- [Autoregressive Models](https://outcomeschool.com/blog/autoregressive-models)

## Autoregressive vs Masked Modeling

Autoregressive models predict the next token from previous tokens, while masked language models predict hidden tokens from bidirectional context.

Key points:
- Autoregressive modeling naturally supports open-ended generation.
- Masked modeling builds strong representations for classification, retrieval, and ranking.
- Encoder-decoder systems combine bidirectional input encoding with autoregressive output decoding.

## Example

Example: GPT-style models generate `The answer is ...` left to right; BERT-style models fill masked words using both left and right context.

## Current Software Engineering Use Case

Chat models are mostly autoregressive, while many embedding and reranking models use encoder-style bidirectional representations.
