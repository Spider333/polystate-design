---
version: alpha
name: Polystate
description: >-
  Design system for the Polystate ecosystem — polystate.io (main app),
  fund site, admin dashboard, docs, and all landing pages. Inspired by
  Stripe (shadows, fintech trust), Apple (typography discipline, cinematic
  sections), Coinbase (pill CTAs), and Kraken (subtle elevation).

colors:
  primary: "#0E36A5"
  primary-hover: "#0C2E8A"
  bg-dark: "#030B21"
  bg-light: "#F9F9F9"
  bg-white: "#FFFFFF"
  light-blue: "#CADDFF"
  accent-green: "#D8F2DC"
  accent-green-hover: "#C5ECC9"
  accent-green-shadow: "#A3F9B0"
  text-dark: "#0A0F1E"
  text-dark-secondary: "#1E2537"
  text-light: "#EAEAEA"
  text-muted-dark: "#78788C"
  text-muted-light: "#636373"
  border-light: "#E5E5E5"
  neutral-dark-grey: "#2E364D"

typography:
  display-hero:
    fontFamily: General Sans
    fontSize: 96px
    fontWeight: 400
    lineHeight: 1.0
    letterSpacing: -2px
  display:
    fontFamily: General Sans
    fontSize: 64px
    fontWeight: 400
    lineHeight: 1.05
    letterSpacing: -1.2px
  h1:
    fontFamily: General Sans
    fontSize: 48px
    fontWeight: 500
    lineHeight: 1.1
    letterSpacing: -0.96px
  h2:
    fontFamily: General Sans
    fontSize: 36px
    fontWeight: 500
    lineHeight: 1.15
    letterSpacing: -0.5px
  h3:
    fontFamily: General Sans
    fontSize: 24px
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: -0.24px
  body-lg:
    fontFamily: General Sans
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.4
  body:
    fontFamily: General Sans
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.4
  body-sm:
    fontFamily: General Sans
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.4
  button:
    fontFamily: General Sans
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.0
  caption:
    fontFamily: General Sans
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.4
  micro:
    fontFamily: General Sans
    fontSize: 10px
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: 0.5px

rounded:
  micro: 4px
  sm: 8px
  md: 12px
  lg: 16px
  xl: 24px
  full: 9999px

spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  "2xl": 48px
  "3xl": 64px
  section: 96px
  section-lg: 128px

components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.bg-white}"
    typography: "{typography.button}"
    rounded: "{rounded.xl}"
    padding: 16px 48px
  button-primary-hover:
    backgroundColor: "{colors.primary-hover}"
    textColor: "{colors.bg-white}"
  button-accent:
    backgroundColor: "{colors.accent-green}"
    textColor: "{colors.text-dark}"
    typography: "{typography.button}"
    rounded: "{rounded.xl}"
    padding: 16px 48px
  button-accent-hover:
    backgroundColor: "{colors.accent-green-hover}"
    textColor: "{colors.text-dark}"
  button-ghost-dark:
    backgroundColor: "transparent"
    textColor: "{colors.text-light}"
    rounded: "{rounded.xl}"
    padding: 16px 48px
  button-secondary:
    backgroundColor: "{colors.light-blue}"
    textColor: "{colors.primary}"
    typography: "{typography.button}"
    rounded: "{rounded.xl}"
    padding: 12px 32px
  section-light:
    backgroundColor: "{colors.bg-light}"
    textColor: "{colors.text-dark}"
  card-light:
    backgroundColor: "{colors.bg-white}"
    textColor: "{colors.text-dark}"
    rounded: "{rounded.md}"
    padding: 28px 24px
  card-light-border:
    backgroundColor: "{colors.border-light}"
    textColor: "{colors.text-dark}"
  caption-dark:
    backgroundColor: "{colors.bg-dark}"
    textColor: "{colors.text-muted-dark}"
    typography: "{typography.caption}"
  caption-light:
    backgroundColor: "{colors.bg-white}"
    textColor: "{colors.text-muted-light}"
    typography: "{typography.caption}"
  secondary-text-light:
    backgroundColor: "{colors.bg-white}"
    textColor: "{colors.text-dark-secondary}"
  secondary-text-dark:
    backgroundColor: "{colors.bg-dark}"
    textColor: "{colors.neutral-dark-grey}"
  card-dark:
    backgroundColor: "{colors.bg-dark}"
    textColor: "{colors.text-light}"
    rounded: "{rounded.md}"
    padding: 28px 24px
  card-featured:
    backgroundColor: "{colors.bg-white}"
    textColor: "{colors.text-dark}"
    rounded: "{rounded.lg}"
    padding: 32px 28px
  badge-success:
    backgroundColor: "{colors.accent-green}"
    textColor: "{colors.text-dark}"
    typography: "{typography.micro}"
    rounded: "{rounded.xl}"
    padding: 4px 12px
  input-light:
    backgroundColor: "{colors.bg-white}"
    textColor: "{colors.text-dark}"
    rounded: "{rounded.sm}"
    padding: 12px 16px
  input-dark:
    backgroundColor: "{colors.bg-dark}"
    textColor: "{colors.text-light}"
    rounded: "{rounded.sm}"
    padding: 12px 16px
  nav-light:
    backgroundColor: "{colors.bg-white}"
    textColor: "{colors.text-dark}"
    height: 64px
  nav-dark:
    backgroundColor: "{colors.bg-dark}"
    textColor: "{colors.text-light}"
    height: 64px
---

## Overview

Polystate helps globally mobile people navigate residency, citizenship,
taxation, and legal change. The brand reads as *sovereign, premium, and
trustworthy* — closer to a private bank or broadsheet than a SaaS tool.

Two modes alternate for cinematic pacing: **dark** (`#030B21`) for
immersive hero and fund contexts, **light** (`#F9F9F9` / `#FFFFFF`) for
open informational sections. Each background change signals a new
"scene."

Typography is disciplined: **General Sans** everywhere, weight 400 for
body and 500 for headings — never 600+. Negative letter-spacing tightens
progressively as size grows (-2px at 96px, relaxing to normal at 16px).

Shadows are always brand-tinted (`rgba(3,11,33,...)`), never neutral
grey. The dotted globe/grid pattern is the signature motif.

## Colors

The palette is built around a single saturated blue anchor
(`#0E36A5`) and a calm neutral spine. Green is reserved for success
and status — never decorative.

- **Primary (#0E36A5):** The sovereign Polystate blue. CTAs, links,
  active states, brand accent. Exact value — not lighter, not darker.
- **Primary Hover (#0C2E8A):** Slightly darker for interactive lift.
- **BG Dark (#030B21):** Near-black navy for immersive sections, fund
  site, hero, app chrome.
- **BG Light (#F9F9F9):** Warm off-white for open content sections.
  Prefer over pure white for body backgrounds.
- **BG White (#FFFFFF):** Cards and elevated surfaces on light mode.
- **Light Blue (#CADDFF):** Gradient text highlights and accent tints.
  Never used as a solid fill.
- **Accent Green (#D8F2DC):** Success badges, dual-CTA pair-mate,
  positive status. Never used for informational neutral surfaces.
- **Text Dark (#0A0F1E):** Near-black for body text on light. Never
  pure `#000000`.
- **Text Light (#EAEAEA):** Body text on dark. Never pure `#FFFFFF`.
- **Text Muted (#78788C / #636373):** Dark / light mode captions and
  metadata.

## Typography

**General Sans** is the only display and body face. Inter is permitted
only for data tables and dense numeric grids.

Letter-spacing scales negatively with size: `-2px` at 96px, `-1.2px` at
64px, `-0.96px` at 48px, relaxing to normal at 16px and below. Line
height compresses with size: `1.0` at display, `1.1–1.2` at heading,
`1.4` at body.

Font smoothing must always be enabled
(`-webkit-font-smoothing: antialiased`).

## Layout

Layout is generous and rhythmic. Max content width is **1152px**
(`max-w-6xl`). Section vertical padding follows a cinematic cadence:
`py-28 sm:py-36` for primary sections, `py-16` for interstitials.
Horizontal page padding is `px-6`.

Spacing uses an 8px base scale. Grid gaps are `gap-4` to `gap-6`.

## Elevation & Depth

Shadows are always tinted with the dark brand blue
(`rgba(3,11,33,...)`) — never neutral grey. The tint carries brand
atmosphere, not just depth.

- **Level 0** — flat, page background.
- **Level 1** — `rgba(3,11,33,0.06) 0px 2px 8px`. Hover hints.
- **Level 2** — `rgba(3,11,33,0.10) 0px 8px 24px`. Cards, panels.
- **Level 3** — `rgba(3,11,33,0.15) 0px 16px 40px -12px,
  rgba(0,0,0,0.08) 0px 8px 20px -8px`. Featured cards, dropdowns.
- **Level 4** — `rgba(3,11,33,0.20) 0px 24px 48px -16px,
  rgba(0,0,0,0.10) 0px 12px 24px -8px`. Modals, floating panels.
- **Focus Ring** — `0 0 0 2px rgba(14,54,165,0.3)`.

Negative spread keeps shadows vertical and controlled. Multi-layer
approach pairs a brand-tinted far shadow with a neutral close shadow.

## Shapes

Pill (24px) is the signature radius for interactive elements — buttons
and badges. Cards use 12–16px. Sharp corners and fully round (>24px)
are avoided on content surfaces.

## Components

Buttons are always pill-shaped (`rounded.xl` = 24px). The signature
Polystate hero pattern is the **dual CTA**: primary blue
(`button-primary`) paired with accent green (`button-accent`) side by
side.

Cards alternate between `card-light` (white surface on `#F9F9F9`) and
`card-dark` (translucent white over `#030B21`). Featured cards use the
larger `rounded.lg` radius.

Navigation is sticky with glass blur on both modes —
`backdrop-filter: blur(12px)` over a translucent background. The glass
effect is part of the brand identity; do not ship nav without it.

## Known Lint Warnings

Two warnings are intentional and accepted:

- `components.secondary-text-dark` contrast 1.63:1 — deliberate. The
  `neutral-dark-grey` on `bg-dark` pair is reserved for *decorative
  labels and peripheral metadata*, never for reading text. Flag is
  accurate: do not use this pair for primary copy.
- `colors.accent-green-shadow` orphaned — decorative drop-shadow only
  (e.g. `box-shadow: 0 1px 1px #a3f9b0` under success badges). Not
  consumed as a component fill or text color.

## Do's and Don'ts

### Do

- Use General Sans for every surface — including headings.
- Use the primary blue at exactly `#0E36A5` — not lighter, not darker.
- Ship buttons with 24px pill radius and the dual-CTA pattern on heroes.
- Apply progressive negative letter-spacing at display sizes.
- Keep body text on dark at `#EAEAEA`, body text on light at `#0A0F1E`.
- Alternate dark and light sections for cinematic section rhythm.
- Use brand-tinted shadows (`rgba(3,11,33,...)`).
- Use accent green `#D8F2DC` for badges, success, and dual-CTA pairing.
- Enable font smoothing (antialiased) on every page.

### Don't

- Don't use General Sans weight 600 or 700 — 400/500 only.
- Don't use large border-radius (>24px) on cards — 12–16px max.
- Don't use neutral grey shadows — always tint with dark blue.
- Don't use pure black text (`#000000`) — use `#0A0F1E`.
- Don't add colors outside this palette without approval.
- Don't ship navigation without the glass blur — it defines the brand.
- Don't use Inter for headings — Inter is data tables only.
- Don't center-align body text — left-align; only headlines may center.
- Don't use decorative gradients on buttons — gradient is for text only.
- Don't introduce rainbow colors or off-brand decorative SVGs.
