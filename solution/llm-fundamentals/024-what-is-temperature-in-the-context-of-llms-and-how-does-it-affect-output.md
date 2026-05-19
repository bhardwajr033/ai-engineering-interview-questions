# What is temperature in the context of LLMs, and how does it affect output?

**Topic:** LLM Fundamentals

## Source

- [What is temperature in the context of LLMs?](https://x.com/amitiitbhu/status/1964990603927687493)

## Generation Controls

Temperature, top-k, and top-p control how the next token is selected from model probabilities.

Key points:
- Lower temperature makes outputs more deterministic; higher temperature increases diversity and risk.
- Top-k samples only from the k most likely tokens.
- Top-p samples from the smallest set of tokens whose cumulative probability reaches p.

## Example

Example: use temperature 0-0.2 for invoice extraction, but a higher value for brainstorming alternative marketing copy.

## Current Software Engineering Use Case

Production systems use low temperature for extraction and compliance workflows, moderate temperature for drafting, and repetition penalties or decoding constraints for long-form generation.
