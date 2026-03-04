---
title: "09 Bazaar"
layout: default
parent: Katas
nav_order: 9
---

# Kata 9: Bazaar

**A peer-to-peer marketplace for handmade goods with no central inventory.**

An artisan collective wants to build an alternative to Etsy — fully decentralised, where each seller manages their own catalogue and the platform aggregates them. No warehouse, no central product database. Think: federated marketplace.

**Users:** 5,000 sellers at launch, 100,000 buyers. Average seller has 20–50 products.

## Requirements

- Federated product catalogue (each seller hosts their own, platform aggregates)
- Global search across all federated catalogues
- Order and payment processing (escrow-style for buyer protection)
- Reputation system (reviews, seller ratings) that is tamper-resistant
- Seller analytics dashboard
- Support for physical goods (shipping) and digital goods (instant delivery)

## Constraints

- Sellers must be able to operate even if the central platform is down
- Product data must remain under seller ownership
- Payment processing must comply with PSD2 (EU payment regulation)
- Some sellers are non-technical; onboarding must be dead simple
- Budget: crowdfunded, lean team of 4 developers

## Additional context

The collective has strong opinions about platform power. The architecture must avoid creating any single point of control. They've looked at ActivityPub and AT Protocol for inspiration.

[Back to all katas](../README.md#the-katas)
