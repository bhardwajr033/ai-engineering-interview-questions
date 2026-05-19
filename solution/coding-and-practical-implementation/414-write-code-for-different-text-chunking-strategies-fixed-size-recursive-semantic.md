# Write code for different text chunking strategies (fixed-size, recursive, semantic).

**Topic:** Coding and Practical Implementation

## Implementation Approach

Implement the feature as a small, testable pipeline instead of mixing parsing, model calls, and business logic in one function.

Key points:
- Define the interface first: inputs, outputs, errors, timeouts, and observability fields.
- Keep model calls behind a small adapter so providers and models can be swapped.
- Validate all inputs and outputs, especially tool arguments and structured model responses.
- Add deterministic unit tests for pure logic and fixture-based tests for model-facing behavior.

## Example

```python
def fixed_chunks(text, size=800, overlap=120):
    step = max(1, size - overlap)
    return [text[i:i + size] for i in range(0, len(text), step)]
```

Example: start with a small local test fixture, then add provider integration tests behind mocked model responses.

## Current Software Engineering Use Case

Used in developer tools for code generation, review, migration, test writing, and repository-aware assistance.
