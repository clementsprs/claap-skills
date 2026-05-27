---
name: customer-onboarding-deck-builder
description: Turn every closed-won deal into persona-specific onboarding decks — IC sales, managers, CSMs, product, execs — grounded in real CRM data and Claap transcripts.
---

# Customer Onboarding Deck Builder

Runs on your Claap call recordings via the bundled **Claap** MCP server (authorize access on first use). Also uses the **HubSpot**, **Google Drive** MCP server(s) — connect these separately.

Before running, replace any `<placeholder>` values in the instructions below (CRM filter, Claap workspaces, Slack channel, etc.) with your own. To run it automatically on a cadence, save it as a Scheduled agent in Claude.

---

Extract the full design system from this page:
- Color palette: backgrounds (dark/light/neutrals), accents, text colors, gradients. Capture exact hex or HSL values.
- Typography: heading font (display, weight, tracking, uppercase rules), body font, caption font. Include exact families, weights, sizes, line-heights.
- Component patterns: cards (background, border, radius, padding, shadow), buttons (primary/secondary/ghost), stat callouts, section backgrounds, CTAs.
- Logo: exact URL to the SVG or PNG file.
- Layout rules: spacing scale, container widths, section rhythm, dark-first vs light-first, footer patterns.
- Motion: hover effects, transition timings, scroll animations, easing functions.

Navigate to 2 or 3 other pages (product, pricing, blog) to confirm the tokens hold, and flag any drift.

Then generate a reusable skill file I can save as my branding reference. Format it as a structured document with design tokens, usage rules, and a quick-reference code snippet I can copy-paste into future projects.
