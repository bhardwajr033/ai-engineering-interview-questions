# What is RLAIF (RL from AI Feedback), and how does it differ from RLHF?

**Topic:** Fine-Tuning and Model Adaptation

## Preference Optimization

Preference optimization aligns model behavior with human or AI feedback after supervised training.

Key points:
- RLHF usually trains a reward model from human preferences and optimizes the policy with an algorithm such as PPO.
- DPO directly optimizes chosen-vs-rejected response pairs without a separate reward model.
- GRPO compares outputs within groups and is useful for reasoning-focused optimization where relative quality matters.

## Example

Example: given two candidate support replies, preference training teaches the model to choose the one that is accurate, polite, and policy-compliant.

## Current Software Engineering Use Case

Chatbot teams use preference optimization to make responses more helpful, harmless, concise, and instruction-following.
