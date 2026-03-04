---
title: Home
layout: default
nav_order: 1
permalink: /
---

# AI-Enabled Architectural Katas

A ready-to-run format for practising software architecture with a twist: **all teams solve the same problem**, but each team gets a different **AI persona** that constrains how they can use their AI assistant. The personas have specific expertise, blind spots, and strong opinions — forcing teams to work _with_ and _around_ their AI, just like working with a real (opinionated) colleague.

Two baselines frame the experiment: one team works **without any AI** (the human-only control), while the facilitator lets **AI run autonomously** to produce a pure-AI solution. Comparing these three approaches — human-only, persona-constrained AI, and full-AI — is where the deepest learning happens.

This format explores a question nobody else in the community is asking yet: **What happens to architectural decisions when your AI collaborator has a specific worldview?**

## What are architectural katas?

Architectural katas are practice exercises for software architects, originally created by Ted Neward and popularised by Neal Ford. The word "kata" comes from martial arts — a pattern practised until it becomes second nature. In the architecture context, teams receive a realistic problem and design a high-level architecture under time pressure, then present for peer feedback. The [O'Reilly Architectural Katas](https://learning.oreilly.com/featured/architectural-katas/) (moderated by Sam Newman) and [Ted Neward's ArchKatas](https://github.com/tedneward/ArchKatas) are the best-known examples.

<div id="random-buttons"></div>
<script>
  const pickRandom = (arr) => arr[Math.floor(Math.random() * arr.length)];

  const katas = [{% for p in site.pages %}{% if p.parent == "Katas" %}`{{ p.url | relative_url }}`,{% endif %}{% endfor %}];
  const personas = [{% for p in site.pages %}{% if p.parent == "Personas" and p.nav_order != 0 %}`{{ p.url | relative_url }}`,{% endif %}{% endfor %}];

  const container = document.getElementById("random-buttons");
  container.className = "d-flex flex-justify-around my-6";

  const buttons = [
    { label: "🎲 Random Kata", cls: "btn-purple", urls: katas },
    { label: "🎭 Random AI Persona", cls: "btn-blue", urls: personas },
  ];

  buttons.forEach(({ label, cls, urls }) =>
    container.appendChild(Object.assign(document.createElement("a"), {
      className: `btn ${cls}`,
      textContent: label,
      href: "#",
      onclick: (e) => { e.preventDefault(); window.location.href = pickRandom(urls); },
    }))
  );
</script>

## Quick start

1. The facilitator picks **one kata** from the [`katas/`](./katas/) folder — all teams solve the same problem.
2. Form teams of 4–6 people.
3. One team is the **no-AI control group** — they work without any AI assistance.
4. Every other team gets a random **AI persona card** from the [`personas/`](./personas/) folder.
5. The facilitator kicks off an **autonomous AI run** using the [AI baseline prompt](./personas/00-the-ai-baseline.md) — this produces the pure-AI solution.
6. Teams design their architecture in 60–90 minutes.
7. Each team presents for 5–7 minutes, then the facilitator reveals the AI-only solution.
8. Retrospective: compare human-only, persona-constrained, and pure-AI architectures.

See the [facilitator guide](./facilitator-guide.md) for detailed timing, retrospective questions, and tips.

### How to use a persona

1. Open the file for your assigned persona.
2. Read the description to understand the personality, expertise, and blind spots.
3. Copy the prompt from the **Prompt** section.
4. Paste it into your AI chat as the first message.
5. Then paste or describe your kata problem and start designing.

The prompt sets up the AI's character. Everything after that is your architectural conversation — filtered through that character's very specific worldview.

### A note on learning

The personas are deliberately one-dimensional. Real architects hold multiple concerns in their head simultaneously. The point of the exercise is to experience what happens when you can only see through one lens — and to discover, as a team, what that lens reveals and what it hides.

The most interesting learning happens during the retrospective, when teams compare their AI-shaped architectures and realise how much the persona influenced their decisions.

## Inspired by

- [O'Reilly Architectural Katas](https://learning.oreilly.com/featured/architectural-katas/) — the multi-week competition moderated by Sam Newman, which introduced the "AI-Enabled Architecture" theme in 2025.
- [Ted Neward's ArchKatas](https://github.com/tedneward/ArchKatas) — the canonical open-source collection of kata problems.
- [Neal Ford's _Fundamentals of Software Architecture_](https://www.oreilly.com/library/view/fundamentals-of-software/9781492043447/) — where many of the kata patterns originate.

## Licence

These materials are shared for community use. Feel free to adapt them for your own meetups, workshops, and events. Attribution appreciated.

If you run an event using these materials, we'd love to hear about it — open an issue or PR with your experience!
