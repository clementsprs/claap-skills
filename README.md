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

  ## Using a skill

  Download the `.skill` file, upload it to Claude.ai as a personal skill (or drop it into your local skills folder), then describe your task. Claude auto-loads it when triggers match.

  ## Contributing

  1. Add a new folder at the repo root with a `SKILL.md` inside.
  2. Write the frontmatter `description` as a trigger spec — the clearer it is, the better auto-activation works.
  3. Put scripts under `scripts/`, reference docs under `references/`.
  4. Open a PR.

  ## Roadmap

  - [x] `extract-branding-theme`
  - [ ] `claap-sales-deck`
  - [ ] `claap-icp`
