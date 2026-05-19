# What is tokenization in LLMs?

**Topic:** LLM Fundamentals

## Source

- [Tokenization in Large Language Models (LLMs)](https://www.youtube.com/watch?v=sK2s9I84EVI)
  - Transcript notes: the tokenization video explains that models operate on numbers, so text is converted into tokens and token ids. It compares word, subword, and character tokenization and highlights BPE-style subword tokenization as a practical balance.

## Tokenization

Tokenization converts raw text into smaller units called tokens, then maps those tokens to numeric ids the model can process.

Key points:
- Tokens may be words, characters, bytes, or subwords.
- Subword tokenization handles rare words better than word-level tokenization while keeping sequences shorter than character-level tokenization.
- Tokenization affects cost, latency, context usage, multilingual quality, and how well domain terms are represented.

## Example

Example: `unbelievable` might be split into `un`, `believ`, and `able`; this lets the model handle rare words without needing every possible word in its vocabulary.

## Current Software Engineering Use Case

In production, teams measure token counts before calling an LLM, design chunk sizes for RAG, and sometimes extend or retrain tokenizers for specialized legal, medical, or code vocabularies.
