# Claap skills

  A collection of [Claude skills](https://docs.claude.com/en/docs/agents-and-tools/claude-code/skills) used by the Claap team. Drop one into Claude and it loads on demand
  when the task matches.

  ## Available skills

  ### extract-branding-theme

  Reverse-engineers any `.pptx` file into a structured JSON design system and saves every logo and image to disk. Point Claude at a deck, get back the colors, fonts, layouts, and
  assets it's built from.

  Pipeline: theme colors, typography, layout grid, masters and layouts, asset extraction and classification, component patterns, metadata.

  Output:
  - `branding_template.json` — full design system
  - `assets/` — every image, brand assets flagged

  Triggers on any `.pptx` upload plus phrases like "extract the branding", "reverse-engineer this template", "what fonts and colors does this deck use".

  ### claap-design-system

  The Claap design system as a Tailwind-first reference: dark-first UI, Inter font, blue primary, full gray scale and accent palette, component recipes (cards, buttons, flashcards, stat callouts, accordions, nav), motion language. Drop into a Claude project to produce artifacts and HTML/React prototypes that feel like an extension of Claap, not just "styled with brand colors".

  Triggers on phrases like "claap design", "claap UI", "claap artifact", "claap prototype", "build claap interface".

  ### design-system-extractor

  Extracts a full design system from a live product — website (via Claude Chrome extension or WebFetch) or Figma file (via Dev Mode MCP) — and returns a drop-in design-system skill matching the `claap-design-system` format: tokens, component recipes, motion, interaction states. Bootstrap step for teams that want a `<product>-design-system` skill without writing one from scratch.

  Triggers on phrases like "extract design system", "design system from website", "design system from figma", "build a design-system skill", "reverse-engineer product UI".

  ## Using a skill

  Download the `.skill` file, upload it to Claude.ai as a personal skill (or drop it into your local skills folder), then describe your task. Claude auto-loads it when triggers match.

  ## Contributing

  1. Add a new folder at the repo root with a `SKILL.md` inside.
  2. Write the frontmatter `description` as a trigger spec — the clearer it is, the better auto-activation works.
  3. Put scripts under `scripts/`, reference docs under `references/`.
  4. Open a PR.

  ## Roadmap

  - [x] `extract-branding-theme`
  - [x] `claap-design-system`
  - [x] `design-system-extractor`
  - [ ] `claap-sales-deck`
  - [ ] `claap-icp`
