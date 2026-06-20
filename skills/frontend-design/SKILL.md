---
name: Frontend Design
description: Use when building web UI (React/Next.js/Tailwind/HTML) — distinctive, accessible, production-grade interfaces that avoid generic AI look.
version: 1.0.0
---

# Frontend Design

Build interfaces that look intentional, not template-generated. Pair this with the `ui-ux-pro-max` skill for color/type/style data.

## Principles
- **One clear hierarchy** — the eye should know where to look first. Size, weight, space, color in that order.
- **Real spacing rhythm** — use a scale (4/8/12/16/24/32). Don't eyeball random margins.
- **SVG icons, never emoji** as UI icons (Lucide / Heroicons). Consistent 24×24 viewBox.
- **Accessible by default** — 4.5:1 text contrast, visible focus rings, 44px touch targets, labels on inputs.
- **Motion with restraint** — 150–300ms, `transform`/`opacity` only, respect `prefers-reduced-motion`.

## Avoid the "AI slop" look
- No center-everything purple-gradient hero with three emoji feature cards.
- Pick a point of view: editorial, terminal/IDE, brutalist, soft-minimal — and commit across all pages.
- Vary section rhythm (don't stack identical cards). Use asymmetry and real content widths (65–75 chars).

## Before shipping
Run the `ui-ux-pro-max` pre-delivery checklist: contrast, hover feedback, cursor-pointer on clickables, responsive at 375/768/1024/1440, no horizontal scroll.
