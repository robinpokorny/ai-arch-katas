# Kata 6: Nomad

**A platform for async-first distributed teams.**

A future-of-work startup building tools for fully distributed companies (no offices, no time zones, no synchronous meetings by default). Think of it as the operating system for a company where nobody is ever online at the same time.

**Users:** 10,000 users across 200 companies at launch. Companies range from 5 to 500 people.

## Requirements

- Asynchronous video/audio messaging with threading (like voice memos that form conversations)
- Decision-making workflows (proposals, votes, decisions — all async)
- Context hand-off system ("here's where I left off, here's what you need to know")
- Timezone-aware scheduling for the rare synchronous moments
- Activity digests: AI-generated summaries of what happened while you were asleep
- Integration with existing tools (GitHub, Jira, Notion, Slack)

## Constraints

- Messages must sync reliably even with intermittent connectivity (nomad lifestyles)
- End-to-end encryption for all communications
- Multi-tenancy with strict data isolation between companies
- Must support low-bandwidth environments (some users are on 3G)
- Team of 12 engineers, half backend, half frontend

## Additional context

The founders believe meetings are a bug, not a feature. The architecture should reflect this philosophy — no component should require synchronous interaction.

[Back to all katas](../README.md#the-katas)
