# Explain WordPiece and SentencePiece.

**Topic:** LLM Fundamentals

## WordPiece and SentencePiece

WordPiece and SentencePiece are subword tokenization approaches used to represent text with reusable pieces rather than only full words.

Key points:
- WordPiece chooses subword units that improve likelihood under a language model and is associated with BERT-style tokenizers.
- SentencePiece treats text as a raw stream and can tokenize without pre-splitting on whitespace, which helps multilingual systems.
- Both reduce out-of-vocabulary failures but can still split domain-specific terms poorly if the tokenizer was trained on mismatched data.

## Example

Example: a multilingual assistant can tokenize English, Hindi, and Japanese text without relying only on spaces between words.

## Current Software Engineering Use Case

A multilingual search or assistant product may choose SentencePiece to handle languages without clear whitespace boundaries and WordPiece/BPE for compatibility with existing model families.
