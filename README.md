# AI-Enabled Architectural Katas

*Created by [Software Design Berlin](https://www.meetup.com/software-design-berlin/)*

A ready-to-run format for practising software architecture with a twist: each team gets an **AI persona** that constrains how they can use their AI assistant. The personas have specific expertise, blind spots, and strong opinions — forcing teams to work *with* and *around* their AI, just like working with a real (opinionated) colleague.

One team serves as the **control group**, letting AI drive everything with no constraints. Comparing their output to the persona-constrained teams is where the most interesting discussion happens.

This format explores a question nobody else in the community is asking yet: **What happens to architectural decisions when your AI collaborator has a specific worldview?**

## What are architectural katas?

Architectural katas are practice exercises for software architects, originally created by Ted Neward and popularised by Neal Ford. The word "kata" comes from martial arts — a pattern practised until it becomes second nature. In the architecture context, teams receive a realistic problem and design a high-level architecture under time pressure, then present for peer feedback. The [O'Reilly Architectural Katas](https://learning.oreilly.com/featured/architectural-katas/) (moderated by Sam Newman) and [Ted Neward's ArchKatas](https://github.com/tedneward/ArchKatas) are the best-known examples.

## Quick start

1. Form teams of 4–6 people.
2. Each team gets a random **kata** (the problem) and a random **AI persona card** (the constraint).
3. One team is the control group (unrestricted AI).
4. Teams design their architecture in 60–90 minutes, using AI according to their persona.
5. Each team presents for 5–7 minutes, covering both the architecture **and** how AI shaped it.
6. Retrospective: compare how different AI personas led to different architectures.

See the [facilitator guide](./facilitator-guide.md) for detailed timing, retrospective questions, and tips.

## The Katas

Each kata has a realistic scenario, users, requirements, constraints, and a built-in tension that forces trade-off decisions. Pick whichever ones suit your group — you don't need all 10.

| # | Kata | Domain | Key tension |
|---|------|--------|-------------|
| 01 | [GhostKitchen](./katas/01-ghostkitchen.md) | Virtual restaurants | Founder vs CTO on microservices |
| 02 | [PaperTrail](./katas/02-papertrail.md) | Compliance documents | SharePoint migration under regulation |
| 03 | [Tidal](./katas/03-tidal.md) | Collaborative music production | Real-time vs eventually consistent |
| 04 | [Greenhouse](./katas/04-greenhouse.md) | IoT vertical farming | Unreliable connectivity + reliability obsession |
| 05 | [Polyglot](./katas/05-polyglot.md) | Conference translation | Human-in-the-loop AI at scale |
| 06 | [Nomad](./katas/06-nomad.md) | Async-first teamwork | "Meetings are a bug" philosophy |
| 07 | [Revival](./katas/07-revival.md) | Endangered languages | Data sovereignty + offline-first |
| 08 | [Sentinel](./katas/08-sentinel.md) | City infrastructure | Legacy SCADA + government security |
| 09 | [Bazaar](./katas/09-bazaar.md) | Federated marketplace | Decentralisation vs usability |
| 10 | [Chronos](./katas/10-chronos.md) | Historical simulations | AI accuracy in education |

## AI Persona Cards

Each persona file has a description (personality, expertise, blind spots, catchphrase) and a **ready-to-use prompt** that participants copy and paste into ChatGPT, Claude, Gemini, or any other AI chat.

| # | Persona | Lens |
|---|---------|------|
| 00 | [The Control Group](./personas/00-the-control-group.md) | Unrestricted AI — no constraints |
| 01 | [The Archaeologist](./personas/01-the-archaeologist.md) | Legacy systems, migration, backward compatibility |
| 02 | [The Visionary](./personas/02-the-visionary.md) | Cutting-edge tech, emerging patterns |
| 03 | [The Accountant](./personas/03-the-accountant.md) | Cost optimisation, cloud economics |
| 04 | [The Chaos Monkey](./personas/04-the-chaos-monkey.md) | Resilience, fault tolerance, disaster recovery |
| 05 | [The User Whisperer](./personas/05-the-user-whisperer.md) | UX, accessibility, front-end architecture |
| 06 | [The Compliance Officer](./personas/06-the-compliance-officer.md) | Security, privacy, regulatory compliance |
| 07 | [The Philosopher](./personas/07-the-philosopher.md) | Domain-driven design, bounded contexts |
| 08 | [The Scale Fanatic](./personas/08-the-scale-fanatic.md) | High-throughput, scaling, performance |
| 09 | [The Diplomat](./personas/09-the-diplomat.md) | Team topology, Conway's Law, sociotechnical design |
| 10 | [The Minimalist](./personas/10-the-minimalist.md) | Simplicity, boring technology |

### How to use a persona

1. Open the file for your assigned persona.
2. Read the description to understand the personality, expertise, and blind spots.
3. Copy the prompt from the **Prompt** section.
4. Paste it into your AI chat as the first message.
5. Then paste or describe your kata problem and start designing.

The prompt sets up the AI's character. Everything after that is your architectural conversation — filtered through that character's very specific worldview.

### Design principles behind the prompts

The prompts follow established prompting practices:

- **Second person** ("You are...") to set the AI's role clearly.
- **Explicit expertise** so the AI knows what domain to draw from.
- **Concrete behavioural rules** ("You must never...", "You always...") to constrain responses.
- **Personality and tone** to make the interaction feel human and memorable.
- **Context** about the kata exercise so the AI understands the setting.
- **Stay-in-character instruction** at the end to prevent the AI from dropping the persona.

### A note on learning

The personas are deliberately one-dimensional. Real architects hold multiple concerns in their head simultaneously. The point of the exercise is to experience what happens when you can only see through one lens — and to discover, as a team, what that lens reveals and what it hides.

The most interesting learning happens during the retrospective, when teams compare their AI-shaped architectures and realise how much the persona influenced their decisions.

## Running your own event

These materials are designed to work for any meetup, workshop, conference, or training session. You can:

- **Pick a subset of katas** that match your audience's domain expertise or interests.
- **Pick a subset of personas** — even 4–5 personas plus a control group makes for a great session.
- **Adjust the timing** — the [facilitator guide](./facilitator-guide.md) has a suggested schedule, but the format works in 2–3 hours.
- **Write your own katas** — follow the structure: scenario, users, requirements, constraints, additional context with a built-in tension.
- **Write your own personas** — follow the pattern: expertise, personality, behavioural rules, blind spots, catchphrase, stay-in-character instruction.

If you run an event using these materials, we'd love to hear about it. Open an issue or PR with your experience!

## Inspired by

- [O'Reilly Architectural Katas](https://learning.oreilly.com/featured/architectural-katas/) — the multi-week competition moderated by Sam Newman, which introduced the "AI-Enabled Architecture" theme in 2025.
- [Ted Neward's ArchKatas](https://github.com/tedneward/ArchKatas) — the canonical open-source collection of kata problems.
- [Neal Ford's *Fundamentals of Software Architecture*](https://www.oreilly.com/library/view/fundamentals-of-software/9781492043447/) — where many of the kata patterns originate.

## Licence

These materials are shared for community use. Feel free to adapt them for your own meetups, workshops, and events. Attribution to [Software Design Berlin](https://www.meetup.com/software-design-berlin/) appreciated.

---

*Created by [Software Design Berlin](https://www.meetup.com/software-design-berlin/). First run at Thoughtworks Berlin, March 2026.*
