# A pre-trained model from an open-source repo may contain a hidden backdoor. How do you detect it?

**Topic:** AI Safety, Ethics, and Responsible AI

## Open vs Closed LLMs

Open-source or open-weight LLMs provide more deployment control, while closed-source APIs provide convenience and often stronger managed capabilities.

Key points:
- Choose open models for data control, customization, offline deployment, cost at scale, or vendor independence.
- Choose closed APIs for fastest integration, strong general quality, managed scaling, and reduced infrastructure burden.
- The practical decision depends on security, latency, compliance, quality, cost, and team expertise.

## Example

Example: use a closed API for a prototype that needs best quality quickly, then evaluate an open model when cost, data residency, or customization becomes dominant.

## Current Software Engineering Use Case

An enterprise may use a closed frontier model for complex reasoning and a self-hosted open model for high-volume internal classification.
