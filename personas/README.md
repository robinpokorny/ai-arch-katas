---
title: Personas
layout: default
nav_order: 4
has_children: true
permalink: /personas/
---

# AI Persona Cards

Each persona file has a description (personality, expertise, blind spots, catchphrase) and a **ready-to-use prompt** that participants copy and paste into ChatGPT, Claude, Gemini, or any other AI chat.

The personas are deliberately one-dimensional. Real architects hold multiple concerns in their head simultaneously. The point of the exercise is to experience what happens when you can only see through one lens — and to discover, as a team, what that lens reveals and what it hides.

## How to use a persona

1. Open the file for your assigned persona.
2. Read the description to understand the personality, expertise, and blind spots.
3. Copy the prompt from the **Prompt** section.
4. Paste it into your AI chat as the first message.
5. Then paste or describe your kata problem and start designing.

The prompt sets up the AI's character. Everything after that is your architectural conversation — filtered through that character's very specific worldview.

<div id="persona-actions"></div>
<script>
  const personas = [{% for p in site.pages %}{% if p.parent == "Personas" and p.nav_order != 0 %}`{{ p.url | relative_url }}`,{% endif %}{% endfor %}];
  const container = document.getElementById("persona-actions");
  container.className = "d-flex my-4";
  container.style.gap = "1rem";

  const buttons = [
    { label: "🎭 Random Persona", cls: "btn-blue", href: "#", onclick: (e) => { e.preventDefault(); window.location.href = personas[Math.floor(Math.random() * personas.length)]; } },
    { label: "🖨 Print Cards", cls: "btn-outline", href: `{{ '/personas/print/' | relative_url }}` },
  ];

  buttons.forEach(({ label, cls, href, onclick }) =>
    container.appendChild(Object.assign(document.createElement("a"), {
      className: `btn ${cls}`,
      textContent: label,
      href,
      ...(onclick && { onclick }),
    }))
  );
</script>
