---
title: "07 Revival"
layout: default
parent: Katas
nav_order: 7
---

# Kata 7: Revival

**A platform for digitising and preserving endangered languages.**

A non-profit working with indigenous communities wants to build a platform where community members can record spoken language, elders can validate translations, and linguists can build dictionaries and grammar models. The platform must respect the communities' ownership of their language data.

**Users:** 50 indigenous communities, ~200 active contributors per community. 20 linguist researchers.

## Requirements

- Audio recording and annotation tools (browser and mobile)
- Community-governed access control (each community decides who sees what)
- Dictionary builder with audio pronunciation links
- Grammar pattern detection (semi-automated with linguist review)
- Offline-first for communities with limited internet
- Data sovereignty: community data stays on infrastructure they control

## Constraints

- Many users have older Android phones (Android 8+, low storage)
- Internet access may be satellite-based (high latency, low bandwidth)
- No cloud dependency for core functionality — communities must be able to run locally
- Budget: grant-funded, €100,000 total for v1
- Must handle languages with non-Latin scripts and tonal notation

## Additional context

This is not just a technical problem. Data sovereignty means the architecture must allow communities to physically own their data — possibly on-premise hardware donated to the community. Centralised cloud is acceptable only as an opt-in replication target.

[Back to all katas](../README.md#the-katas)
