---
title: "10 Chronos"
layout: default
parent: Katas
nav_order: 10
redirect_from:
  - /k10
  - /katas/10
---

# Kata 10: Chronos

**A platform for interactive historical simulations used in education.**

An edtech company wants to build a platform where history students can "enter" historical scenarios (the fall of the Berlin Wall, the Apollo 11 mission, the signing of the Treaty of Westphalia) and explore them interactively. AI characters represent historical figures. Students make decisions and see how outcomes might have changed.

**Users:** 200 schools, ~50 students per class, 3 classes per school using it at any time. 30 content creators (historians and educators).

## Requirements

- Interactive scenario engine with branching narratives
- AI-driven historical characters that respond contextually and accurately
- Content authoring tools for educators to create and modify scenarios
- Multiplayer mode: entire classes experience a scenario together, different students play different roles
- Assessment integration (track student decisions for grading)
- Multimedia support (maps, images, audio narration, primary source documents)

## Constraints

- Must run on school hardware (Chromebooks, iPads, low-end Windows laptops)
- School networks are restrictive (firewalls, content filters, limited bandwidth)
- AI characters must be historically accurate — no hallucinations that would misinform students
- COPPA/GDPR compliance for student data (many users are minors)
- Content must be reviewable and approvable by educators before going live

## Additional context

The biggest concern from educators: "What if the AI says something historically wrong and students believe it?" The architecture must have guardrails — factual grounding, educator review, and clear signals when the AI is speculating versus citing sources.