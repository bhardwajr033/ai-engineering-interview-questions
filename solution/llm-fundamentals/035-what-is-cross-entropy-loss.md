# What is Cross-Entropy Loss?

**Topic:** LLM Fundamentals

## Source

- [Math Behind Cross-Entropy Loss](https://outcomeschool.com/blog/math-behind-cross-entropy-loss)

## Cross-Entropy Loss

Cross-entropy loss measures how well predicted probabilities match the correct target token or class.

Key points:
- For language modeling, the target is usually the next token.
- Lower loss means the model assigns higher probability to the correct token.
- Perplexity is derived from cross-entropy and is often used to compare language models.

## Example

Example: if the correct next token is `policy`, cross-entropy is low only when the model assigns high probability to `policy`.

## Current Software Engineering Use Case

Model teams track validation cross-entropy during pre-training and fine-tuning to detect underfitting, overfitting, or data regressions.
