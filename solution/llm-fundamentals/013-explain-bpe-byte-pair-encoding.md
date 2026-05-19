# Explain BPE (Byte Pair Encoding).

**Topic:** LLM Fundamentals

## Source

- [Byte Pair Encoding](https://outcomeschool.com/blog/bpe-in-llms)

## Byte Pair Encoding

BPE is a subword tokenization algorithm that starts with small units and repeatedly merges the most frequent adjacent pairs.

Key points:
- Common words can become single tokens while rare words are split into meaningful subword pieces.
- It provides an open vocabulary because unseen words can still be represented as smaller pieces.
- The merge table learned during tokenizer training must be reused consistently at inference time.

## Example

Example: after repeated merges, a frequent phrase piece like `tion` may become one token, while a rare domain word is still represented by smaller subword tokens.

## Current Software Engineering Use Case

BPE-style tokenizers are widely used in LLMs because they balance vocabulary size, sequence length, and robustness to rare or newly coined terms.
