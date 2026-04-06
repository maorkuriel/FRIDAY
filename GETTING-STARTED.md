# Getting Started with F.R.I.D.A.Y

## Step 1: Install

```bash
claude plugin marketplace add maorkuriel/friday
claude plugin install friday
```

## Step 2: Personalize (2 minutes)

On first launch, F.R.I.D.A.Y shows the personalization wizard. Click your answers to 6 questions:

1. **Your PM level** — associate, PM, senior, principal, lead, or VP
2. **Company type** — startup, growth, enterprise, agency, etc.
3. **Product type** — B2B SaaS, B2C, dev tools, marketplace, mobile, etc.
4. **Domain focus** — core product, growth, monetization, UX, data, etc.
5. **Engineering relationship** — embedded squad, cross-team, solo PM, etc.
6. **Biggest pain point** — PRDs, prioritization, strategy, users, metrics, etc.

F.R.I.D.A.Y uses your profile to personalize skill recommendations and tone.

## Step 3: Set Up Your Knowledge Base

```
/pm-setup
```

Answer 6 steps about your company and product. Drop your company URL and F.R.I.D.A.Y researches it automatically. This creates your `knowledge/` directory — the foundation every skill uses.

## Step 4: Try Your First Skill

Based on your pain point, F.R.I.D.A.Y recommends where to start. Common first skills:

```bash
/write-prd <feature-name>      # If you need to spec something
/product-strategy              # If you need to think about direction
/prioritize                    # If you have a backlog to rank
/pm-briefing                   # If you want an overview of everything
```

## Step 5: Let It Compound

The more you use F.R.I.D.A.Y, the smarter it gets. Every skill reads from and writes to `knowledge/`. After a month:

- Your competitive battlecards inform your PRDs
- Your OKRs inform your prioritization
- Your retros inform your next sprint scope
- Your daily briefing shows everything at once

---

## Core Commands Reference

| What You Want | Command |
|---------------|---------|
| Route any request | `/friday` |
| Set up your product | `/pm-setup` |
| Write a PRD | `/write-prd <feature>` |
| Build a strategy | `/product-strategy` |
| Score your backlog | `/prioritize` |
| Morning briefing | `/pm-briefing` |
| See everything | `/pm-dashboard` |
| Research a competitor | Say "research [competitor]" |
| Analyze feedback | Say "here's some customer feedback: ..." |
| Launch checklist | `/launch-plan <feature>` |
| Build a presentation | `/create-slide-deck <topic>` |

---

## Getting Multi-Agent Reviews

F.R.I.D.A.Y automatically spawns expert subagents when you ask:

- "Review this PRD" → Engineer + Executive + User Researcher review in parallel
- "Devil's advocate on this strategy" → Devil's Advocate subagent
- "Multi-perspective review" → All three perspectives simultaneously

Each subagent gives you a risk-rated review with specific, actionable recommendations.

---

## Memory System

F.R.I.D.A.Y remembers across sessions:

- **Decisions** you make are logged automatically
- **Blockers** are tracked and surfaced in your briefing
- **Action items** carry over between sessions
- **Daily notes** capture what you worked on

Run `jarvis status` to see recent events, or `jarvis actions` for pending action items.

---

## Standalone Prompts

Don't want to use Claude Code? Every strategic skill is available as a standalone prompt in `prompts/`. Just paste into any AI tool.

---

## Troubleshooting

See `docs/TROUBLESHOOTING.md` for common issues and fixes.
