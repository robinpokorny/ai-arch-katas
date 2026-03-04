---
title: "05 Polyglot"
layout: default
parent: Katas
nav_order: 5
redirect_from:
  - /k05
  - /katas/05
---

# Kata 5: Polyglot

**A real-time translation platform for international conferences.**

An events company wants to build a platform that provides real-time speech translation for conferences with 500+ attendees speaking different languages. Attendees get translations through their phones. Speakers see live transcription on a confidence monitor.

**Users:** 500–5,000 attendees per event. 10–50 events per month. Speakers in 20+ languages.

## Requirements

- Real-time speech-to-text with speaker identification
- Translation into attendee's selected language within 3 seconds of speech
- Mobile app for attendees to select language and read/hear translations
- Confidence monitor integration for speakers (showing live transcript)
- Post-event: searchable transcript archive with timestamps
- Support for technical jargon (configurable glossaries per event)

## Constraints

- Must work in conference venues with potentially poor WiFi (thousands of devices)
- Translation accuracy must be >95% for supported language pairs
- Privacy: recordings must be deletable per GDPR and speaker consent
- Some venues have no reliable internet — consider hybrid/edge options
- Maximum €2 per attendee per event for compute costs

## Additional context

The company currently uses human interpreters. The platform doesn't replace them — it augments them. Human interpreters can override/correct the AI translation in real time.