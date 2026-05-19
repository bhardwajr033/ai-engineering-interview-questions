# What are benchmark suites (MMLU, HumanEval, GSM8K), and how do you interpret them?

**Topic:** Evaluation and Testing

## Evaluation and Testing

AI evaluation measures whether model behavior is useful, correct, safe, robust, and cost-effective for a target workflow.

Key points:
- Offline evaluation uses golden datasets, task metrics, LLM-as-a-judge, human review, and regression tests.
- Online evaluation uses A/B tests, user feedback, business metrics, latency, and incident rates.
- LLM outputs require qualitative rubrics and adversarial cases because exact-match metrics are often insufficient.

## Example

Example: evaluate a RAG answer on retrieval relevance, answer faithfulness, citation correctness, latency, and user task success.

## Current Software Engineering Use Case

Teams run continuous evals on RAG faithfulness, answer relevance, tool-call accuracy, safety, and latency before promoting prompt or model changes.
