# Claap — AI agents for revenue teams

Ready-to-run Claude skills that work on your real **Claap** call recordings.
Each agent reads your calls, deals and emails through the Claap MCP server (AI
fields, saved views and tagged transcript search included) and turns meetings into action: win/loss readouts, battlecards, onboarding decks, customer
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
| 🧭 `account-brief-builder` | Walk into every call knowing what the account already told you. Account Brief Builder reads every call, email and deal on the account in Claap and sends you a one-page brief in Slack before the meeting: who's in the room, what they said, what's still open, and what to get out of this call. |
| 🥊 `battlecard-generator` | Create competitor battlecards on demand — grounded in real prospect quotes from Claap recordings and verified against your product docs + the competitor's. |
| 🎓 `customer-onboarding-deck-builder` | Turn every closed-won deal into persona-specific onboarding decks — IC sales, managers, CSMs, product, execs — grounded in real CRM data and Claap transcripts. |
| ✍️ `customer-story-writer` | Generate a cinematic customer story page from every won deal — hero, quotes carousel, ROI metrics, deal timeline — and publish directly to your CMS. |
| 🚨 `deal-risk-detector` | Stop losing deals you could see coming. Deal Risk Detector reads every call, transcript and email attached to every open deal in Claap, scores the risk with the evidence behind it, and posts one structured digest to Slack every morning. |
| 🎯 `keyword-researcher` | Turn what buyers actually say in sales calls into the SEO keywords you should own. Keyword Researcher mines the terms, topics and competitors from your Claap calls, then ranks them by search demand versus difficulty with Ahrefs. |
| 📈 `objection-dashboard-builder` | Turn scattered objection data into an interactive monthly dashboard — verbatim quotes, category trends, and coaching insights, branded to your design system. |
| 🎭 `ramp-trainer` | Cut ramp time. Ramp Trainer mines your closed deals in Claap, turns them into voice roleplays where an ElevenLabs AI plays the buyers your team actually faces, scores every drill, and tells you when a new rep is ready for a live call. |
| 🤝 `sales-cs-handover` | Automatic one-page handover for every closed deal — stakeholders, commitments, success criteria, and risks pulled from every sales recording in the cycle. |
| 🧑‍🏫 `sales-deck-builder` | Build a fully branded, prospect-specific sales deck in 1 minute — pulling pain points, quotes, and pricing context from every Claap call. |
| 🎯 `sales-meetings-daily-recap` | Get a structured Slack recap every morning of yesterday's sales calls — objections, competitor mentions, and product signals, each deep-linked to the exact moment in the recording. |
| 📊 `win-loss-analyzer` | Set up AI fields on your deals, then run a weekly win/loss readout — compares won vs lost qualification scores, ranks the reasons, and posts the digest to Slack. |

## What you'll need

- A **Claap** account with call recordings (bundled MCP, authorized on first use).
- For some agents, additional MCP servers you connect yourself — e.g. your CRM
  (HubSpot / Salesforce), Slack, Notion, or Google Drive. Each skill states which.

## Usage

Ask Claude to run an agent by name, e.g. *"Run the weekly win/loss analysis"*.
Replace any `[PLACEHOLDER]` values the first time. If no workspace is set, the
agent lists your Claap workspaces and asks which one to use. To run on a cadence, save the agent as a Scheduled agent in Claude.
