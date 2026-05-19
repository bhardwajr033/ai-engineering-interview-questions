# Compare RAG vs fine-tuning. When would you use each?

**Topic:** Retrieval-Augmented Generation (RAG)

## Source

- [AI Engineering Explained: LLM, RAG, MCP, Agent, Fine-Tuning, Quantization](https://www.youtube.com/watch?v=lnfWvX66FUk)
  - Transcript notes: the video frames AI engineering around six practical building blocks: LLMs for language generation, RAG for grounding answers in external knowledge, MCP for standardized tool/data integration, agents for goal-directed tool use, fine-tuning for behavior or domain adaptation, and quantization for cheaper deployment.

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
