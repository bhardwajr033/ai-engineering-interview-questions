# What are logits, and how are they used in text generation?

**Topic:** LLM Fundamentals

## Source

- [Understanding Logits in Machine Learning](https://x.com/amitiitbhu/status/1927927814923207146)

## Logits

Logits are raw, unnormalized scores the model produces for each possible next token before softmax.

Key points:
- Softmax converts logits into probabilities.
- Decoding parameters modify or filter logits before a token is selected.
- Logit bias can increase or decrease the chance of specific tokens when an API supports it.

## Example

Example: before choosing the next token, the model may assign high logits to `refund` and `return`; decoding settings turn those scores into the final selection.

## Current Software Engineering Use Case

Structured-output systems can bias or constrain logits to improve valid JSON generation and reduce unwanted tokens.
