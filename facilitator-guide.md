# Facilitator Guide

Everything you need to run an AI-enabled architectural kata session.

## Format overview

Each team receives two things:

1. **A kata** — the architecture problem to solve (from the [`katas/`](./katas/) folder)
2. **An AI persona card** — defining how the team's AI assistant behaves (from the [`personas/`](./personas/) folder)

The AI persona is NOT a general-purpose helper. It has a specific personality, expertise, blind spots, and quirks. Teams must learn to work *with* their AI's strengths and *around* its limitations — just like working with a real (opinionated) colleague.

One team gets no persona card. Instead, they get the **control group** card and let AI do everything — full delegation, no constraints. This is the "what happens when you just let the machine drive?" baseline.

## Suggested schedule

Adapt the timing to your event. A 2.5–3 hour slot works best.

| Phase | Duration | Activity |
|-------|----------|----------|
| Introduction | 10–15 min | Explain the kata format and the AI twist; hand out persona cards |
| Team formation + reveal | 5 min | Groups of 4–6 people; each team gets their kata and persona card |
| Design session | 60–90 min | Teams work on their architecture, using AI according to their persona |
| Presentations | 5–7 min per team | Present architecture AND how AI shaped the process |
| Retrospective | 15–20 min | Group discussion (see questions below) |

### Example evening schedule

| Time | Phase |
|------|-------|
| 18:15 | Doors open — snacks, drinks, socialisation |
| 18:45 | Introduction |
| 18:55 | Team formation + reveal |
| 19:00 | Design session (~90 min) |
| 20:30 | Presentations |
| ~21:00 | Retrospective |
| 21:15 | End |

## Retrospective questions

These are the heart of the learning. Don't skip this part.

- How did your AI persona influence the architecture you designed?
- What trade-offs did the AI push you toward — and did you agree?
- Where did the AI's blind spots actually help you think more carefully?
- Control group: What happened when you let AI drive? Where did it shine, where did it go off the rails?
- Would you want this AI persona on your real team? Why or why not?
- What did you learn about working with AI that you'll take back to your day job?

## Tips for facilitators

- **Assign katas and personas randomly** — half the fun is the surprise.
- **Encourage teams to actually use AI** during the session (ChatGPT, Claude, Gemini, Copilot — whatever they have). Ask attendees in advance to bring access to at least one AI tool.
- **Consider a prompting cheat sheet** — a one-pager with basic prompting tips helps teams who are new to using AI for architecture work get started quickly.
- **The persona card is a constraint, not a suggestion** — teams should lean into it.
- **Remind the control group**: they should genuinely defer to AI, not just use it as a tool.
- **During presentations**: ask teams to show HOW they used AI, not just WHAT they designed.
- **Have fun with it** — the personas are deliberately colourful; embrace the chaos.

## Scaling for different group sizes

| Attendees | Teams | Katas | Personas | Presentation time |
|-----------|-------|-------|----------|-------------------|
| 10–20 | 3–4 | 3–4 (can share) | 3–4 + control | 5 min each |
| 20–40 | 5–8 | 5–8 | 5–8 + control | 5 min each |
| 40–60 | 8–10 | Pick 8–10 | Pick 8–10 + control | 5 min each, or split into tracks |
| 60+ | 10+ | All 10 | All 10 + control | Split into parallel tracks with shared retro |

For larger groups, consider giving multiple teams the same kata with different personas — the comparison is fascinating.

## What you'll need

- A room (or rooms) where teams can work without disturbing each other
- WiFi strong enough for everyone to use AI tools simultaneously
- A projector or screen for presentations
- Printed persona cards (one per team) — or share the GitHub links
- Printed kata cards (one per team) — or share the GitHub links
- Whiteboard, flip chart, or paper for teams to sketch diagrams
- A timer visible to all teams

## Materials

- [`katas/`](./katas/) — 10 architectural katas (one file each)
- [`personas/`](./personas/) — 10 AI persona cards + control group (one file each, with copy-pasteable prompts)

[Back to main README](./README.md)
