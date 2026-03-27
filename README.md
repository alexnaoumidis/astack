# Astack

Build better work. The same process discipline that lets one engineer ship like a team of twenty — for everything that isn't code.

Inspired by [Gstack](https://github.com/garrytan/gstack).

## What This Is

A set of Cowork skills that chain together to help you think sharper, create with quality, and ship with confidence. Whether you're building a board deck, a sales proposal, a financial report, or a Monday morning Slack message — the process is the same:

**Frame → Create → Review → Reflect**

Each skill feeds the next. `/frame` produces a brief that `/review` evaluates against. `/retro` tracks what shipped and whether the process helped. Nothing falls through the cracks because each step knows what came before.

## Skills

### Core Chain (v0.1)

| Skill | What It Does |
|-------|-------------|
| `/frame` | Forces clarity before you start creating. Six hard questions that most people skip. Produces a brief that makes everything downstream better. |
| `/review` | Systematic quality check before you send. Catches accuracy errors, inconsistencies, buried asks, and AI slop. Auto-fixes the obvious stuff, flags judgment calls. |
| `/retro` | Structured reflection after delivery. What shipped, what stalled, what patterns are emerging. Compounds over time as it compares across weeks. |

### Coming Next

| Skill | What It Does |
|-------|-------------|
| `/perspective` | Multi-angle review — evaluates your work from 3-4 relevant perspectives simultaneously (the strategist, the skeptic, the reader, the detail checker). Scores each dimension 0-10. |
| `/verify` | Fact-check gate. Traces every number to its source, audits every comparison, classifies every claim as verified/unverifiable/incorrect. |
| `/10star` | Pressure-tests your ambition. "What would the 10-star version of this look like?" Four modes: expand, focus, reduce, reframe. |
| `/structure` | Reviews the logical architecture before you build. Maps argument flow, surfaces hidden assumptions, catches gaps. |
| `/deliver` | Pre-flight checklist before sending. Right audience? Right format? Right timing? Right context? |
| `/diagnose` | Root-cause analysis when something goes wrong. "No fixes without investigation." |
| `/audience-lens` | Rewrites from the reader's perspective. "I just received this — my first three questions are..." |
| `/pre-mortem` | Before launching: "It's 3 months from now and this failed. What went wrong?" |
| `/decision-doc` | Structured decision framework. Recommendation first, reasoning second, alternatives third. |
| `/careful` | Guardrails before irreversible actions — all-company emails, external publishing, financial commitments. |
| `/full-review` | Auto-chains the relevant skills based on what you're making. One command, full pipeline. |

## Install

Add the marketplace and install:

```
/plugin marketplace add alexnaoumidis/astack
/plugin install astack
```

Then use any skill:

```
/astack:frame
/astack:review
/astack:retro
```

## The Philosophy

This borrows heavily from [Gstack](https://github.com/garrytan/gstack) by Garry Tan — a set of Claude Code skills that encode the workflow of a great engineering team. Gstack's insight is that quality comes from process: think before you build, review before you ship, reflect after you deliver, and chain each step so nothing gets lost between them.

That insight isn't specific to code. A marketer skips the brief and dives into the Google Doc. A founder drafts the investor update before deciding what story they're telling. A finance lead opens the spreadsheet before questioning the assumptions. Everyone does the same thing engineers used to do before Gstack — they reach for the tool before they've finished thinking.

Shipstack applies the same process discipline to everything that isn't code: decks, emails, reports, proposals, analyses, announcements, plans, and everything in between.

The skills adapt automatically based on what you're making. `/review` knows that a board deck needs accuracy and narrative checks while a Slack message needs tone and brevity checks. The process stays the same. The dimensions shift.

## Contributing

This is early. The first three skills are shipped. The next twelve are designed but not built. If you want to contribute a skill, the architecture is simple: each skill is a `SKILL.md` file in its own directory under `skills/`. Read the existing ones for the pattern.

## License

MIT
