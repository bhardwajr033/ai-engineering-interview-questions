# Implement a conversation memory system for a chatbot (sliding window, summary, buffer).

**Topic:** Coding and Practical Implementation

## Implementation Approach

Implement the feature as a small, testable pipeline instead of mixing parsing, model calls, and business logic in one function.

Key points:
- Define the interface first: inputs, outputs, errors, timeouts, and observability fields.
- Keep model calls behind a small adapter so providers and models can be swapped.
- Validate all inputs and outputs, especially tool arguments and structured model responses.
- Add deterministic unit tests for pure logic and fixture-based tests for model-facing behavior.

## Example

```text
1. Parse and validate input.
2. Retrieve or compute the required context.
3. Call the model/tool adapter.
4. Validate output.
5. Log trace, latency, token usage, and errors.
```

Example: start with a small local test fixture, then add provider integration tests behind mocked model responses.

## Current Software Engineering Use Case

Used by software teams building coding and practical implementation features that must balance quality, latency, cost, safety, and maintainability.
