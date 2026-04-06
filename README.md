# F.R.I.D.A.Y

```
███████╗██████╗ ██╗██████╗  █████╗ ██╗   ██╗
██╔════╝██╔══██╗██║██╔══██╗██╔══██╗╚██╗ ██╔╝
█████╗  ██████╔╝██║██║  ██║███████║ ╚████╔╝ 
██╔══╝  ██╔══██╗██║██║  ██║██╔══██║  ╚██╔╝  
██║     ██║  ██║██║██████╔╝██║  ██║   ██║   
╚═╝     ╚═╝  ╚═╝╚═╝╚═════╝ ╚═╝  ╚═╝   ╚═╝  
```

**First Responder Intelligence for Driving Ambitious Yearly-goals**

A Claude Code plugin that turns your terminal into a complete AI-powered product management operating system. **51 skills** covering every PM workflow — from strategy to execution, from PRDs to presentations, from user research to team hiring.

---

## Quick Start

### Install

```bash
claude plugin marketplace add maorkuriel/friday
claude plugin install friday
```

### Personalize (2 minutes)

On first launch, F.R.I.D.A.Y runs a 6-question personalization wizard:

- Your PM seniority level
- Your company type
- What kind of product you work on
- Your domain focus
- How you work with engineering
- Your biggest pain point right now

Just click your answers — no typing needed. F.R.I.D.A.Y uses your profile to recommend the right skills and tailor its output to your context.

### Set Up Your Product Knowledge Base

```
/pm-setup
```

Drop your company URL and F.R.I.D.A.Y researches everything. Takes 3 minutes. Creates a persistent `knowledge/` directory that every skill reads from and writes to.

### Start Working

```bash
/write-prd notification-system     # Write a full PRD
/product-strategy                   # Build your product strategy
/prioritize                         # Score and rank your backlog
/pm-briefing                        # Morning briefing
/launch-plan checkout-redesign      # Launch checklist
/growth-frameworks                  # Build a growth model
/finding-pmf                        # Assess product-market fit
/create-slide-deck quarterly-review # HTML slide deck
```

Or just describe what you need — F.R.I.D.A.Y routes to the right skill automatically.

---

## What's Inside

### 37 PM Workflow Skills

| Category | Skills |
|----------|--------|
| **Core** | friday (gateway), pm-setup, pm-dashboard, pm-briefing |
| **Discovery** | feedback-synthesis, competitive-intel, opportunity-assessment |
| **Strategy** | product-strategy, write-strategy, okr-writer, quarterly-plan, finding-pmf |
| **User Research** | user-research, persona-builder, interview-guide, journey-map |
| **Define** | write-prd, refine-spec, tech-feasibility |
| **Plan** | prioritize, roadmap-builder, sprint-scope |
| **Growth & Retention** | growth-frameworks, retention-engagement |
| **Deliver** | launch-plan, retro-facilitator, experimentation |
| **Communicate** | storytelling-influence, status-update, decision-record, meeting-prep |
| **Measure** | metrics-check, experiment-review |
| **Present** | create-slide-deck |
| **Career & Team** | pm-career-growth, team-and-hiring |

### 4 Jarvis-Powered Document Skills

Deep, source-grounded document creation with multi-agent review:

| Skill | What It Does |
|-------|-------------|
| `skills/jarvis/prd-writing` | PRD creation with automatic engineer + exec review |
| `skills/jarvis/prfaq-writing` | Amazon-style PR-FAQ writing |
| `skills/jarvis/stakeholder-update` | Multi-audience stakeholder updates |
| `skills/jarvis/strategy-doc` | Strategy documents with devil's advocate review |

### 14 Specialized Subagents

F.R.I.D.A.Y automatically delegates to expert subagents when reviewing documents:

| Subagent | When It Fires |
|----------|--------------|
| **Executive** | Strategic alignment, stakeholder clarity, business impact |
| **User Researcher** | User value, adoption risk, validation gaps |
| **Backend Engineer** | Technical feasibility, API design, data models |
| **Frontend Engineer** | UI complexity, component reuse, performance |
| **CTO** | Architecture decisions, tech debt, scalability |
| **Data Analyst** | Metrics definition, experiment design, SQL logic |
| **Data Engineer** | Data pipeline feasibility, schema design |
| **UX Designer** | Information architecture, accessibility, design systems |
| **Marketer** | Positioning, messaging, launch strategy |
| **Comms** | Communication clarity, narrative structure |
| **Devil's Advocate** | Pre-mortem, failure modes, contrarian analysis |
| **Prompt Assessor** | AI prompt quality, risk quantification |
| **Research Papers** | Academic research grounding |
| **DevOps** | Infrastructure, deployment, reliability |

### Auto-Delegation Triggers

| You Say | F.R.I.D.A.Y Spawns |
|---------|-------------------|
| "review PRD" | Engineer + Executive + User Researcher (parallel) |
| "review PRFAQ" | Executive + Engineer (parallel) |
| "validate feature" | User Researcher |
| "review strategy" | Executive + Engineer |
| "multi-perspective review" | All three (parallel) |
| "assess prompt" | Prompt Assessor |
| "devil's advocate on this" | Devil's Advocate |

---

## Strategic Depth

F.R.I.D.A.Y's strategic skills are grounded in named frameworks from real PM thought leaders:

| Skill | Frameworks |
|-------|-----------|
| **Product Strategy** | Shreyas Doshi, Gibson Biddle (DHM), Marty Cagan |
| **Prioritize** | Shreyas Doshi (LNO), Brandon Chu, Shishir Mehrotra (RICE) |
| **Growth Frameworks** | Brian Balfour, Casey Winters, Sarah Tavel, Sean Ellis |
| **Finding PMF** | Sean Ellis (40% rule), Mike Maples Jr, Dalton Caldwell |
| **User Research** | Bob Moesta (JTBD), Teresa Torres, Krithika Shankarraman |
| **Retention & Engagement** | Gibson Biddle, Naomi Gleit, Patrick Campbell |
| **Storytelling & Influence** | Nancy Duarte, Andy Raskin, Wes Kao |
| **Experimentation** | Ronny Kohavi, Gibson Biddle, Eric Ries |
| **PM Career Growth** | Jackie Bavaro, Ravi Mehta, Julie Zhuo |
| **Team & Hiring** | Gokul Rajaram, Claire Hughes Johnson, Emily Kramer |

---

## The Memory System (3-Layer)

F.R.I.D.A.Y maintains a 3-layer memory that persists across sessions:

```
memory/
  user-profile.md          ← Your PM profile (from personalization wizard)
  learnings.md             ← Patterns and corrections across sessions
  cross-project.md         ← Company and stakeholder context
  daily-notes/             ← Session summaries (last 3 days loaded on start)
  session-log.jsonl        ← Structured event log (decisions, blockers, actions)

knowledge/                 ← Product-specific context (per project)
  pm-context.md            ← Product, team, tools
  friday-profile.md        ← Your personalization answers
  [all other knowledge files...]

cache/                     ← Cached documents (Drive, Notion)
context/                   ← Project-level analysis outputs
```

### What Gets Logged Automatically

- Every **decision** made during a session
- Every **blocker** identified
- Every **action item** created
- Every **document fetched** (cached immediately)
- Session summaries at end of day

---

## The Knowledge System

Every skill reads from and writes to `knowledge/`:

```
knowledge/
  pm-context.md       ← Product, team, and tools
  friday-profile.md   ← Your personalization answers
  team.md / okrs.md / strategy.md
  competitors/        ← Battlecards (one per competitor)
  decisions/          ← Decision records with rationale
  specs/              ← PRDs and feature specs
  feedback/           ← Customer feedback syntheses
  priorities/         ← Feature rankings and scoring
  roadmap/            ← Quarterly roadmaps
  sprints/            ← Sprint plans
  launches/           ← Launch checklists
  updates/            ← Stakeholder updates
  meetings/           ← Meeting prep and notes
  metrics/            ← KPI reviews
  experiments/        ← A/B test analyses
  opportunities/      ← Opportunity assessments
  retros/             ← Retrospectives
  briefs/             ← Daily briefings
  personas/           ← User personas
  research/           ← Interview guides, journey maps
  feasibility/        ← Technical assessments
  decks/              ← HTML slide decks
  growth/             ← Growth models
  pmf/                ← PMF assessments
```

---

## Standalone Prompts (Any AI Tool)

The `prompts/` folder contains all strategic skill prompts as plain markdown — no Claude Code required:

```
prompts/
  prioritization.md
  product-strategy.md
  growth-frameworks.md
  finding-product-market-fit.md
  user-research.md
  retention-and-engagement.md
  experimentation.md
  storytelling-and-influence.md
  pm-career-growth.md
  team-and-hiring.md
```

Paste any of these into ChatGPT, Gemini, or any AI tool.

---

## Claude Desktop (Non-CLI Users)

If you use Claude Desktop instead of Claude Code CLI:

```
claude-desktop/pm-workspace-wizard.skill
```

Install this `.skill` file in Claude Desktop and say "set up my PM workspace" — it generates 38 files across 25 folders in under 5 minutes.

---

## Integrations (Optional)

F.R.I.D.A.Y works out of the box with zero integrations. Install these for live data:

| Integration | What It Unlocks |
|-------------|----------------|
| **GitHub** | PR data for status updates and feasibility checks |
| **Linear / Jira** | Sprint data, backlog, ticket status |
| **Slack** | Channel messages for feedback synthesis |
| **Notion** | Doc imports and wiki references |
| **Confluence** | Enterprise doc imports |
| **Amplitude / Mixpanel** | Live metrics for KPI reviews and experiment analysis |
| **Figma** | Design references for PRDs |
| **Google Drive** | Document caching and context loading |

---

## Quick Commands

```
/friday              → Gateway — routes any request to the right skill
/pm-setup            → Onboarding wizard
/write-prd           → Write a PRD
/product-strategy    → Build a strategy
/prioritize          → Score your backlog
/pm-briefing         → Morning briefing
/launch-plan         → Launch checklist
/create-slide-deck   → HTML presentation
/growth-frameworks   → Growth model
/finding-pmf         → PMF assessment
/pm-career-growth    → Career growth plan
/team-and-hiring     → Hiring scorecard
```

---

## Steering Wheel

Adjust F.R.I.D.A.Y's output style on-the-fly:

| Command | Effect |
|---------|--------|
| "make it more concrete" | Ground in specifics |
| "make it bolder" | More decisive |
| "expand on this" | More depth |
| "simplify" | Plain language |
| "be more exploratory" | More options |
| "lock it in" | Definitive answer |
| "devil's advocate" | Challenge the recommendation |

---

## Requirements

- [Claude Code](https://docs.anthropic.com/en/docs/claude-code) (CLI, desktop, or IDE extension)
- Claude Pro, Team, or Enterprise plan

## Security

Every skill is a plain markdown file you can read and audit. No compiled code, no obfuscated logic.

## Update

```bash
claude plugin update friday
```

## Uninstall

```bash
claude plugin uninstall friday
claude plugin marketplace remove friday-marketplace
```

Your `knowledge/` and `memory/` directories are not deleted.

## License

MIT. See [LICENSE](LICENSE).
