# Kata 3: Tidal

**A real-time collaborative music production platform.**

A music tech company wants to build a browser-based digital audio workstation (DAW) where musicians can collaborate in real time — like Google Docs, but for music. Multiple users should be able to add tracks, adjust effects, and hear changes in near real-time.

**Users:** 10,000 musicians at launch, targeting 500,000 within 2 years. Sessions typically have 2–5 collaborators.

## Requirements

- Real-time collaborative editing of multi-track audio projects
- Low-latency audio playback (<50ms perceived latency)
- Plugin/effect system (reverb, EQ, compression) running in-browser
- Version history with the ability to "branch" a project (like git for music)
- Asset library for samples, loops, and presets
- Export to standard formats (WAV, MP3, FLAC, MIDI)

## Constraints

- Must work in modern browsers without installing anything
- Audio processing must not depend on server round-trips for playback
- Storage: each project can be up to 2 GB of raw audio
- The team has deep audio expertise but limited distributed systems experience

## Additional context

Latency is king. Musicians will abandon the platform if collaboration feels "laggy." Think carefully about what needs to be real-time versus eventually consistent.

[Back to all katas](../README.md#the-katas)
