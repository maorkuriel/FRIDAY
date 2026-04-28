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

The ultimate AI-powered product management operating system, built as a [Claude Code](https://claude.ai/code) plugin. **39 PM skills** covering the full product lifecycle — from customer discovery to strategy, from PRDs to retrospectives, from career growth to capacity planning.

> **Live at:** [maorkuriel.github.io/FRIDAY](https://maorkuriel.github.io/FRIDAY)

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

Drop your company URL and F.R.I.D.A.Y researches everything. Takes 3 minutes. Creates a persistent `knowledge/` directory that every skill reads from and writes to — compounding your context over time.

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
/capacity-audit                     # Audit where your time is going
/pm-improvement                     # Build a 30-day skill growth plan
```

Or just describe what you need — F.R.I.D.A.Y routes to the right skill automatically.

---

## What's Inside

### 39 PM Workflow Skills

| Category | Skills |
|----------|--------|
| **Core** | `friday` (gateway), `pm-setup`, `pm-dashboard`, `pm-briefing` |
| **Discovery** | `feedback-synthesis`, `competitive-intel`, `opportunity-assessment` |
| **Strategy** | `product-strategy`, `write-strategy`, `okr-writer`, `quarterly-plan`, `finding-pmf` |
| **User Research** | `user-research`, `persona-builder`, `interview-guide`, `journey-map` |
| **Define** | `write-prd`, `refine-spec`, `tech-feasibility` |
| **Plan** | `prioritize`, `roadmap-builder`, `sprint-scope` |
| **Growth & Retention** | `growth-frameworks`, `retention-engagement` |
| **Deliver** | `launch-plan`, `retro-facilitator`, `experimentation` |
| **Communicate** | `storytelling-influence`, `status-update`, `decision-record`, `meeting-prep` |
| **Measure** | `metrics-check`, `experiment-review` |
| **Present** | `create-slide-deck` |
| **Career & Team** | `pm-career-growth`, `team-and-hiring` |
| **Manage Yourself** | `capacity-audit`, `pm-improvement` |

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
| "devil's advocate on this strategy" | Devil's Advocate subagent |
| "multi-perspective review" | All three perspectives simultaneously |
| "is this technically feasible?" | Backend Engineer + CTO |
| "prepare for exec presentation" | Executive + Comms |

---

## Skill Highlights

### `/write-prd` — Guided PRD Creation
Discovery-based PRD generation. F.R.I.D.A.Y asks the right questions first, then writes a full PRD with Gherkin acceptance criteria, success metrics, and a launch plan. Reads your codebase for technical context if available.

### `/product-strategy` — Battle-Tested Strategy
Frameworks from Shreyas Doshi, Gibson Biddle, and Marty Cagan. Builds or critiques a product strategy with explicit bets, positioning, and what you're choosing NOT to do.

### `/prioritize` — Ruthless Prioritization
RICE and ICE scoring with OKR multipliers. Ranks your backlog with rationale. Draws from Shreyas Doshi's LNO framework and Brandon Chu's opportunity sizing.

### `/decision-record` — Full Decision Documentation
Captures decisions with Type 1/Type 2 classification (Bezos one-way/two-way door model), alternatives considered, rationale, accepted trade-offs, and explicit revisit conditions. Auto-links to related PRDs, strategy docs, and OKRs.

### `/capacity-audit` — Time and Energy Optimization
Audits how you actually spend your time versus your declared priorities. Identifies energy leaks, misaligned time investments, and produces a weekly calendar template that protects your high-leverage work. Draws from Paul Graham's Maker/Manager schedule and Shreyas Doshi's LNO framework.

### `/pm-improvement` — 30-Day Skill Growth Plan
Honest PM competency assessment across customer discovery, strategy, execution, data, influence, and self-management. Identifies your single highest-leverage gap, diagnoses the root cause, and builds a week-by-week 30-day plan with a measurable success signal. Draws from Ravi Mehta, Jackie Bavaro, and Shreyas Doshi.

### `/pm-briefing` — Daily Operating System
Reads everything — knowledge files, Jira/Linear sprint status, OKR progress, upcoming launches, open decisions, experiment results — and tells you exactly what matters today and what to focus on first.

### `/competitive-intel` — Research to Battlecard in Minutes
Give F.R.I.D.A.Y a competitor URL or name. It fetches their website, pricing, features, and recent news, then generates a full battlecard with positioning, strengths, weaknesses, and strategic implications.

### `/growth-frameworks` — Growth Loop Modeling
Growth loops, viral coefficients, acquisition channels, and retention analysis. Frameworks from Brian Balfour, Casey Winters, Sarah Tavel, and Sean Ellis.

### `/create-slide-deck` — HTML Presentations
Generates beautiful, self-contained HTML slide decks with keyboard navigation, print support, and brand colors extracted from your website. Runs in any browser with no dependencies.

---

## The Knowledge System

F.R.I.D.A.Y stores all product knowledge in `knowledge/`:

```
knowledge/
├── pm-context.md       # Product, team, tools, and strategic context
├── friday-profile.md   # Your personalization answers
├── strategy.md         # Current product strategy
├── okrs.md             # Goals and key results
├── team.md             # Team structure and capacity
├── competitors/        # Competitive battlecards
├── decisions/          # Decision records with revisit dates
├── specs/              # PRDs and product specs
├── feedback/           # Customer feedback syntheses
├── priorities/         # Feature rankings and scoring
├── roadmap/            # Roadmap commitments
├── sprints/            # Sprint plans and capacity
├── launches/           # Launch checklists and retrospectives
├── updates/            # Stakeholder updates
├── meetings/           # Meeting notes and action items
├── metrics/            # KPI reviews and anomaly logs
├── experiments/        # A/B test designs and results
├── opportunities/      # Opportunity assessments
├── retros/             # Retrospectives and open actions
├── briefs/             # Daily briefing history
├── personas/           # User personas
├── research/           # User research and interview notes
├── feasibility/        # Technical feasibility assessments
├── decks/              # Presentations
├── growth/             # Growth models and loop analyses
└── pmf/                # Product-market fit assessments
```

Every skill reads from and writes to this directory. The knowledge compounds — your competitive battlecards inform your PRDs, your OKRs inform your prioritization, your retros inform your next sprint scope.

---

## Frameworks and Sources

F.R.I.D.A.Y grounds its skills in frameworks from the best practitioners in product:

**Strategy**: Shreyas Doshi, Gibson Biddle, Marty Cagan, Hamilton Helmer  
**Growth**: Brian Balfour, Casey Winters, Sarah Tavel, Sean Ellis  
**User Research**: Bob Moesta (JTBD), Teresa Torres, Krithika Shankarraman  
**Prioritization**: Shreyas Doshi (LNO), Brandon Chu, Shishir Mehrotra  
**Communication**: Nancy Duarte, Andy Raskin, Kim Scott, Wes Kao  
**Experimentation**: Ronny Kohavi, Albert Cheng, Eric Ries  
**PMF**: Sean Ellis, Rahul Vohra, Mike Maples Jr, Dalton Caldwell  
**Career**: Ravi Mehta, Jackie Bavaro, Julie Zhuo  
**Teams**: Gokul Rajaram, Claire Hughes Johnson, Emily Kramer  
**Retention**: Gibson Biddle, Naomi Gleit  
**Decisions**: Jeff Bezos (Type 1/Type 2), Jeff Gothelf  
**Self-Management**: Paul Graham (Maker/Manager), Ericsson (Deliberate Practice)

All grounded in real published frameworks — never generic advice.

---

## Requirements

- [Claude Code](https://claude.ai/code) (CLI, desktop, or IDE extension)
- Claude Pro, Team, or Enterprise subscription
- ~3 minutes for initial setup

---

## Installation

### Option 1: Plugin Marketplace (Recommended)

```bash
claude plugin marketplace add maorkuriel/friday
claude plugin install friday
```

### Option 2: Manual Install

```bash
git clone https://github.com/maorkuriel/FRIDAY.git
cd FRIDAY
./install.sh
```

See [GETTING-STARTED.md](GETTING-STARTED.md) for full setup instructions.

---

## Documentation

| Guide | What It Covers |
|-------|---------------|
| [GETTING-STARTED.md](GETTING-STARTED.md) | Full setup walkthrough |
| [docs/QUICK-START.md](docs/QUICK-START.md) | Essential commands reference |
| [docs/CUSTOMIZATION.md](docs/CUSTOMIZATION.md) | Adding skills, customizing behavior |
| [docs/SKILL-REGISTRATION.md](docs/SKILL-REGISTRATION.md) | Building your own skills |
| [docs/JARVIS-GUIDE.md](docs/JARVIS-GUIDE.md) | Jarvis OS deep-dive |
| [docs/TROUBLESHOOTING.md](docs/TROUBLESHOOTING.md) | Common issues and fixes |

---

## License

MIT — see [LICENSE](LICENSE).

Built by [Maor Kuriel](https://github.com/maorkuriel).
