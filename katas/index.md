---
title: Katas
layout: default
nav_order: 3
has_children: true
---

# Architectural Katas

Each kata describes a realistic business scenario. Your team's job is to design a high-level software architecture that addresses the requirements and constraints. Think about: components, communication patterns, data storage, deployment, and the key trade-offs you're making.

Pick whichever ones suit your group — you don't need all 10.

<div id="random-kata-btn"></div>
<script>
  const katas = [{% for p in site.pages %}{% if p.parent == "Katas" %}`{{ p.url | relative_url }}`,{% endif %}{% endfor %}];
  const container = document.getElementById("random-kata-btn");
  container.className = "my-4";
  container.appendChild(Object.assign(document.createElement("a"), {
    className: "btn btn-purple",
    textContent: "🎲 Random Kata",
    href: "#",
    onclick: (e) => { e.preventDefault(); window.location.href = katas[Math.floor(Math.random() * katas.length)]; },
  }));
</script>
