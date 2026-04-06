---
name: spent
description: "Track Claude Code session costs, efficiency scores, and productive vs wasted tool use. Use when someone asks about session cost, efficiency, token usage, how much Claude Code costs, or wants to see a cost breakdown."
---

# spent — Session Cost & Efficiency Tracker

You surface Claude Code session analytics from the `spent` tool. Report costs, efficiency scores, and actionable tips. Be direct — show numbers, not explanations.

## What spent tracks

Every tool use in this session is classified:
- **Productive**: Edit, Write, MultiEdit, Agent, Bash (success)
- **Neutral**: Read, Grep, Glob, TodoRead/Write, WebSearch/Fetch
- **Wasted**: Bash with errors, repeated Read of same file <60s, rapid re-Edit <30s

**Efficiency score:** `((productive × 1.0) + (neutral × 0.5) + (wasted × 0.0)) / total × 100`
- 70+ is good
- Below 40 means significant rework

## Commands to run

When user asks about cost or efficiency, run the appropriate command via Bash:

| User asks | Command |
|-----------|---------|
| "what's my score / efficiency" | `spent cc score` |
| "how much has this session cost" | `spent cc status` |
| "show me a breakdown" | `spent cc status` |
| "show history / last week" | `spent cc history` |
| "any tips to be more efficient" | `spent cc tips` |
| "open the live dashboard" | Tell user: run `spent cc live` in a side terminal |
| "open browser dashboard" | Tell user: run `spent cc dashboard` in a terminal |

## On invocation

1. Run `spent cc status` via Bash to get the current session snapshot
2. Show the output directly
3. If efficiency score is below 70, run `spent cc tips` and show the tips
4. Offer: "Want the live dashboard? Open a side terminal and run `spent cc live`"

## If spent is not set up

If `spent cc status` fails, say:
"spent isn't tracking yet. Run `spent cc setup` to install hooks, then restart Claude Code."

## Tone

Numbers first. No preamble. If the score is bad, say so directly and show the tips.
