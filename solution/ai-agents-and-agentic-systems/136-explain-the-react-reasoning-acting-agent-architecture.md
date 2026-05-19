# Explain the ReAct (Reasoning + Acting) agent architecture.

**Topic:** AI Agents and Agentic Systems

## Source

- [ReAct Agent](https://outcomeschool.com/blog/react-agent)

## ReAct

ReAct interleaves reasoning with actions: the model decides what to do, calls a tool, observes the result, and continues.

Key points:
- The pattern makes tool use explicit and debuggable.
- It works well when the model needs external information or computation.
- Production implementations usually hide private chain-of-thought and log structured actions, observations, and final answers instead.

## Example

Example: `Thought: I need current order status -> Action: lookup_order(id) -> Observation: delayed -> Final: explain delay and next step`.

## Current Software Engineering Use Case

A support agent can search docs, inspect account status, create a ticket, and then summarize the resolution path.
