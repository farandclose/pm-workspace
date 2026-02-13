# Self-Organizing PM Workspace

A ready-to-use workspace template for Product Managers who use [Claude Code](https://docs.anthropic.com/en/docs/claude-code) as their AI assistant. Drop files in, ask questions, and let the system stay organized on its own.

## What This Solves

PMs accumulate tasks and knowledge from meetings, Slack, email, research — scattered across tools and folders. This workspace gives you:

1. **A single TODO** — one file where every task lives, with a trace of what was delivered when it's done.
2. **A semantic directory index** — a keyword-to-file map so you (and the AI) can find anything by concept, not by folder path.
3. **Auto-reconciliation** — drop files into `temp/`, run `/reconcile`, and the system classifies, moves, and indexes them for you.

## Quick Start

1. Clone this repo (or copy the contents into a new project).
2. Install [Claude Code](https://docs.anthropic.com/en/docs/claude-code) if you haven't already.
3. Open the project directory in your terminal and run `claude`.
4. Start working — add tasks, drop files into `temp/`, ask questions about your content.

## How It Works

### TODO.md

Your single task tracker. Tasks flow through **Open → In Progress → Done**. Completed tasks keep a summary of what was delivered, so you have a searchable log months later.

### DIRECTORY_INDEX.md

A keyword-to-file map. When you or the AI need to find something, this index enables concept-based retrieval — search for "churn" or "onboarding" and the right files surface.

### Skills

| Command | What it does |
|---------|-------------|
| `/reconcile` | Scans `temp/`, classifies each file, moves it to the right directory, and updates the index. |
| `/save-it` | Paste article content directly and the system saves it with proper naming and index entry. |

### Directory Structure

```
strategy/            ← Roadmaps, vision docs, positioning, go-to-market
competitive-intel/   ← Competitor analysis, market landscape, battlecards
customer-insights/   ← User research, feedback, interview notes, NPS
specs/               ← PRDs, feature specs, requirements, design briefs
meeting-notes/       ← Standups, syncs, 1:1s, retrospectives
research/            ← Industry trends, papers, articles, frameworks
temp/                ← Drop zone for new files awaiting classification
```

## Customization

- **Add directories** — e.g., `partnerships/`, `launch-plans/` — just update `CLAUDE.md` and the reconcile skill to recognize them.
- **Add skills** — create new `.claude/skills/<name>/SKILL.md` files for repeating workflows.
- **Change the domain** — this pattern works for any role that accumulates tasks and knowledge artifacts. Rename the folders to match your work.

## License

MIT — use it however you like.
