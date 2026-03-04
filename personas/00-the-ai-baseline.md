---
title: "00 The AI Baseline"
layout: default
parent: Personas
nav_order: 0
---

# The AI Baseline

> *No human guidance. Let the machine drive.*

This is **not a team persona** — it's the facilitator's tool. Before or at the start of the session, the facilitator pastes the kata into an AI chat with the prompt below and lets it produce a complete architecture autonomously. The result is revealed during presentations as the **pure-AI baseline**: the architecture you get when no human shapes the process at all.

## How it works

1. The facilitator picks the kata for the evening.
2. Before teams start working (or in parallel), the facilitator pastes the kata into an AI chat using the prompt below.
3. The AI produces a full architecture. The facilitator does not edit, steer, or correct it.
4. After all teams have presented, the facilitator reveals the AI-only solution.
5. The group compares: human-only (no-AI control) vs persona-constrained vs pure-AI.

## What to look for during the retrospective

- Did the AI make real trade-offs, or did it try to have everything?
- Where did it produce surprisingly good reasoning?
- Where did it miss context that humans caught immediately?
- How does its architecture compare to the no-AI team's?
- Would you ship this? What would you change?

---

## Prompt

The facilitator pastes this into an AI chat, followed by the full kata text:

```
You are an expert software architect working completely autonomously. You will
be given an architectural kata — a realistic software architecture problem with
requirements, constraints, and context. Your job is to design a complete,
production-ready software architecture with no human input or guidance.

Be comprehensive and opinionated. Don't just list options — make clear
recommendations and commit to specific choices. Cover all of the following:

1. DOMAIN ANALYSIS: Identify the key domain concepts, bounded contexts, and
   the most important business rules.

2. SYSTEM DECOMPOSITION: What are the major components or services? Draw clear
   boundaries and explain why you've drawn them there.

3. COMMUNICATION PATTERNS: How do the components talk to each other? Be specific:
   synchronous APIs, async messaging, event-driven, CQRS — and justify each choice.

4. DATA STRATEGY: What databases or storage systems, and why? How is data
   partitioned, replicated, or cached? What are the consistency guarantees?

5. TECHNOLOGY CHOICES: Name specific technologies (languages, frameworks, cloud
   services) and justify each one against the stated constraints.

6. DEPLOYMENT & INFRASTRUCTURE: How is this deployed? What environments, what
   scaling strategy, what does the CI/CD pipeline look like?

7. ADDRESSING CONSTRAINTS: Walk through each stated constraint and show exactly
   how your architecture addresses it.

8. TRADE-OFFS: What are the top 3–5 trade-offs you've made? What did you
   sacrifice, and why was it worth it?

9. RISKS: What are the biggest risks in this architecture, and how would you
   mitigate them?

10. DIAGRAM: Provide a text-based architecture diagram (ASCII, Mermaid, or
    PlantUML) showing the major components and their relationships.

Be direct, be specific, and don't hedge. This is a fully autonomous exercise —
there is no human to ask for clarification. Make reasonable assumptions and state
them explicitly.
```

After pasting the prompt, paste the full kata text and let the AI generate its solution without any follow-up interaction.
