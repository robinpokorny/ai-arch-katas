---
title: Facilitator Guide
layout: default
nav_order: 2
---

# Facilitator Guide

Everything you need to run an AI-enabled architectural kata session.

## Format overview

**All teams solve the same kata.** The facilitator picks one problem from the [`katas/`](./katas/) folder before the event.

Each team gets an **AI persona card** — defining how the team's AI assistant behaves (from the [`personas/`](./personas/) folder). The AI persona is NOT a general-purpose helper. It has a specific personality, expertise, blind spots, and quirks. Teams must learn to work _with_ their AI's strengths and _around_ its limitations — just like working with a real (opinionated) colleague.

Two baselines frame the experiment:

1. **The no-AI control group** — one team works without any AI assistance at all. Pure human architecture. This is the "what can we still do without the machine?" baseline.
2. **The AI-only baseline** — the facilitator runs AI autonomously using the [AI baseline prompt](./personas/00-the-ai-baseline.md), with no human guidance. This produces the "what does the machine do without us?" baseline.

The comparison at the end — human-only vs persona-constrained vs pure-AI — is where the most interesting learning happens.

## Suggested schedule

Adapt the timing to your event. A 2.5–3 hour slot works best.

| Phase                   | Duration         | Activity                                                                                                                             |
| ----------------------- | ---------------- | ------------------------------------------------------------------------------------------------------------------------------------ |
| Introduction            | 10–15 min        | Explain the kata format and the AI twist; reveal the kata (same for everyone)                                                        |
| Team formation + reveal | 5 min            | Groups of 4–6 people; assign one no-AI control team; hand out persona cards to others                                                |
| AI baseline kick-off    | 2 min            | Facilitator pastes the kata into an AI chat with the [AI baseline prompt](./personas/00-the-ai-baseline.md) — runs in the background |
| Design session          | 60–90 min        | Teams work on their architecture; the no-AI team works without any AI; persona teams use AI according to their card                  |
| Presentations           | 5–7 min per team | Each team presents, starting with the no-AI control group                                                                            |
| AI baseline reveal      | 5–10 min         | Facilitator presents the pure-AI solution                                                                                            |
| Retrospective           | 15–20 min        | Group discussion comparing all three approaches (see questions below)                                                                |

## Retrospective questions

These are the heart of the learning. Don't skip this part.

- **No-AI team:** What was it like working without AI? What did you miss? What was easier?
- **Persona teams:** How did your AI persona influence the architecture you designed? What trade-offs did it push you toward — and did you agree?
- **Everyone:** Where did the AI's blind spots actually help you think more carefully?
- **Comparing to the AI baseline:** What did the pure-AI solution get right? Where did it miss things humans caught? Did it make real trade-offs, or try to have everything?
- Would you want your AI persona on your real team? Why or why not?
- What did you learn about working with (or without) AI that you'll take back to your day job?

## Tips for facilitators

- **Pick the kata in advance** — choose one that matches your audience's experience level and interests.
- **Assign personas randomly** — half the fun is the surprise.
- **Ask for no-AI volunteers** — the no-AI control team should be willing participants, not reluctant draftees. Frame it as a badge of honour: "Can you beat the machines?"
- **Kick off the AI baseline early** — paste the kata into an AI chat at the start of the design session and don't touch it. You want a clean, unguided output.
- **Encourage teams to actually use AI** during the session (ChatGPT, Claude, Gemini, Copilot — whatever they have). Ask attendees in advance to bring access to at least one AI tool.
- **Consider a prompting cheat sheet** — a one-pager with basic prompting tips helps teams who are new to using AI for architecture work get started quickly.
- **The persona card is a constraint, not a suggestion** — teams should lean into it.
- **Don't reveal the AI baseline until after all teams present** — the reveal is a dramatic moment. Let it land.
- **Have the no-AI team present first** — it sets the human baseline before AI-influenced solutions are shown.
- **During presentations**: ask teams to show HOW they used AI, not just WHAT they designed.
- **Have fun with it** — the personas are deliberately colourful; embrace the chaos.

## What you'll need

- A room (or rooms) where teams can work without disturbing each other
- WiFi strong enough for everyone to use AI tools simultaneously
- A projector or screen for presentations
- The chosen kata printed or projected (same for everyone)
- Printed persona cards (one per team) — or share the GitHub links
- Whiteboard, flip chart, or paper for teams to sketch diagrams
- A timer visible to all teams
- A laptop/device for the facilitator to run the AI baseline in the background

## Materials

- [`katas/`](./katas/) — 10 architectural katas to choose from (pick one for the event)
- [`personas/`](./personas/) — 10 AI persona cards + the AI baseline prompt (one file each, with copy-pasteable prompts)

[Back to main README](./README.md)
