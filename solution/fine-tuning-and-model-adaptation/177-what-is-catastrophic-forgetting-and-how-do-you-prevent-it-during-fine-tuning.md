# What is catastrophic forgetting, and how do you prevent it during fine-tuning?

**Topic:** Fine-Tuning and Model Adaptation

## Fine-Tuning Data Quality

Fine-tuning quality depends more on clean, representative data than on simply adding more examples.

Key points:
- Datasets should include realistic inputs, desired outputs, refusals, edge cases, and negative examples.
- Catastrophic forgetting happens when adaptation over-specializes the model and damages general capabilities.
- Mitigations include mixed training data, lower learning rates, early stopping, regularization, and evaluation on both domain and general tasks.

## Example

Example: include both correct answers and refusal examples so a medical assistant learns when to escalate instead of guessing.

## Current Software Engineering Use Case

A finance assistant fine-tune should include real workflow examples, compliance refusals, and regression tests for general summarization and reasoning.
