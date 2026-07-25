# Digital Onboarding Sequence Builder

A rule-based engine that generates a multi-touch, automated onboarding sequence (email + in-app messaging) tailored to account segment and product complexity — the kind of scaled, digital-led motion that replaces 1:1 onboarding calls once an account base gets too large to onboard manually.

**[Live demo →](#)** (https://melissamcgowan.github.io/Digital-Onboarding-Sequence-Builder/)

## What it does

Given an account **segment** (SMB/self-serve, Mid-Market, Enterprise) and a **product complexity** level, it builds out a day-by-day cadence of touchpoints — each tagged by channel (email, in-app, or both) — with:

- A rationale for why that touchpoint exists at that point in the journey
- Preview content (subject line / body for email, banner or checklist copy for in-app)
- Segment-appropriate cycle length (5 touchpoints over 14 days for SMB, up to 10 touchpoints over 90 days for Enterprise)
- Complexity-aware checkpoints (e.g., an admin-configuration step is only inserted for high-complexity products)
- A built-in stall-check / escalation touchpoint late in the Enterprise sequence — the automated equivalent of a CSM catching a plateaued account

Sequences can be exported as JSON for use in an actual marketing automation or in-app messaging tool (e.g., as a spec handed to Customer.io, Iterable, or Pendo).

## Why this exists

Manual 1:1 onboarding calls don't scale past a certain account volume. This project prototypes the logic a CS team would need to encode once before it can hand onboarding off to automation — segment-aware cadence, channel selection, and a defined point where the system should stop emailing and flag a human instead.

## Tech

Single-file static app — vanilla HTML/CSS/JS, no build step, no dependencies. Deploys directly via GitHub Pages.

## Part of a larger portfolio

This is one piece of a broader AI-powered CS automation portfolio. See the [profile README](../) for the full set of projects, including the Customer Health Score & Churn Prediction Model this sequence logic is designed to eventually pair with (health-triggered save-plays vs. calendar-triggered onboarding).
