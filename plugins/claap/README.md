# Claap — AI agents for revenue teams

Ready-to-run Claude skills that work on your real **Claap** call recordings.
Each agent pulls transcripts and deal context via the Claap MCP server and turns
meetings into action: win/loss readouts, battlecards, onboarding decks, customer
stories, daily recaps and more.

Mirrors the live [Claap Agent Gallery](https://claap.io/agent-gallery).

## Install

```
/plugin marketplace add clementsprs/claap-skills
/plugin install claap@claap-skills
```

On first use each agent authorizes the **Claap** MCP server
(`https://api.claap.io/mcp`, OAuth) against your Claap workspace.

## Agents

| Skill | What it does |
|---|---|
| 🥊 `battlecard-generator` | Create competitor battlecards on demand — grounded in real prospect quotes from Claap recordings and verified against your product docs + the competitor's. |
| 🎓 `customer-onboarding-deck-builder` | Turn every closed-won deal into persona-specific onboarding decks — IC sales, managers, CSMs, product, execs — grounded in real CRM data and Claap transcripts. |
| ✍️ `customer-story-writer` | Generate a cinematic customer story page from every won deal — hero, quotes carousel, ROI metrics, deal timeline — and publish directly to your CMS. |
| 📈 `objection-dashboard-builder` | Turn scattered objection data into an interactive monthly dashboard — verbatim quotes, category trends, and coaching insights, branded to your design system. |
| 🧑‍🏫 `sales-deck-builder` | Build a fully branded, prospect-specific sales deck in 10 minutes — pulling pain points, quotes, and pricing context from every Claap call. |
| 🎯 `sales-meetings-daily-recap` | Get a structured Slack recap every morning of yesterday's sales calls — objections, competitor mentions, and product signals, each deep-linked to the exact moment in the recording. |
| 🤝 `sales-cs-handover` | Automatic one-page handover for every closed deal — stakeholders, commitments, success criteria, and risks pulled from every sales recording in the cycle. |
| 📊 `win-loss-analyzer` | Run a weekly win/loss readout — pulls closed deals from your CRM, mines reasons from Claap transcripts, ranks themes, and posts the digest to Slack. |

## What you'll need

- A **Claap** account with call recordings (bundled MCP, authorized on first use).
- For some agents, additional MCP servers you connect yourself — e.g. your CRM
  (HubSpot / Salesforce), Slack, Notion, or Google Drive. Each skill states which.

## Usage

Ask Claude to run an agent by name, e.g. *"Run the weekly win/loss analysis"*.
Replace any `<placeholder>` values (CRM filter, workspaces, channels) the first
time. To run on a cadence, save the agent as a Scheduled agent in Claude.
