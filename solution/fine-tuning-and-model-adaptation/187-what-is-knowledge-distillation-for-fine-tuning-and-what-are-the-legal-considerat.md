# What is knowledge distillation for fine-tuning, and what are the legal considerations?

**Topic:** Fine-Tuning and Model Adaptation

## Model Distillation

Distillation trains a smaller student model to imitate a larger teacher model.

Key points:
- The student can learn from teacher logits, generated answers, rationales, or preference labels.
- It reduces latency and cost but may lose reasoning depth or rare capabilities.
- Good distillation uses diverse tasks, hard examples, and evaluations that cover teacher strengths.

## Example

Example: generate labeled examples with a strong teacher model, then train a smaller student model for high-volume intent classification.

## Current Software Engineering Use Case

A company can distill a large model into a smaller support-classification model that runs cheaply at high traffic.
