# How do you merge multiple LoRA adapters?

**Topic:** Fine-Tuning and Model Adaptation

## Source

- [LoRA - Low-Rank Adaptation of LLMs](https://outcomeschool.com/blog/lora-low-rank-adaptation-of-llms)

## Fine-Tuning and Adaptation

Fine-tuning adapts a base model by training it on task or domain examples; PEFT methods update only a small set of parameters.

Key points:
- Full fine-tuning updates all weights and is expensive but flexible.
- LoRA trains low-rank adapter matrices while freezing base weights; QLoRA combines LoRA with quantized base weights to reduce memory.
- Prompt/prefix tuning learns soft prompt vectors; adapter tuning inserts small trainable modules.

## Example

Example: fine-tune with high-quality support conversations so the model consistently follows company tone and escalation rules.

## Current Software Engineering Use Case

Fine-tuning is useful for consistent tone, domain-specific formats, classification behavior, tool-call style, or specialized reasoning patterns that prompting and RAG do not solve.
