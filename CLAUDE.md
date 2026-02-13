# CLAUDE.md

## Repository Purpose

This is a self-organizing PM workspace. It uses AI-assisted workflows to manage tasks, organize knowledge artifacts, and enable concept-based retrieval across everything a Product Manager accumulates day-to-day.

## Repository Notes

This is a content/knowledge repository. There are no build steps, test suites, or deployment commands.

## Directory Structure

| Directory | Purpose |
|-----------|---------|
| `strategy/` | Roadmaps, vision docs, positioning, go-to-market plans, strategic analysis |
| `competitive-intel/` | Competitor analysis, market landscape, battlecards, win/loss analysis |
| `customer-insights/` | User research, feedback synthesis, interview notes, NPS analysis, support themes |
| `specs/` | PRDs, feature specs, requirements docs, design briefs |
| `meeting-notes/` | Standups, syncs, 1:1s, retrospectives, brainstorm sessions |
| `research/` | Industry trends, papers, articles, frameworks, reading notes |
| `temp/` | Drop zone for new files awaiting classification |

## Naming Conventions

- **Content files**: `kebab-case.md` (e.g., `q1-roadmap.md`, `competitor-x-teardown.md`)
- **System files**: `UPPERCASE.md` (e.g., `CLAUDE.md`, `TODO.md`, `DIRECTORY_INDEX.md`)

## DIRECTORY_INDEX.md Update Protocol

- When adding or moving a content file, update `DIRECTORY_INDEX.md` with the new path and keywords.
- Keywords should cover the main concepts in the file to enable semantic retrieval.
- Every content file must have an entry in the index.

## TODO.md Workflow

- Tasks move through stages: **Open** → **In Progress** → **Done**.
- Completed tasks retain their output trace (summary of what was done) under the Done section.
- Do not delete completed tasks — they serve as a log.

## temp/ Reconciliation Workflow

- New files land in `temp/` as a staging area.
- On reconciliation: classify each file, move it to the appropriate directory, and update `DIRECTORY_INDEX.md`.
- `temp/` should be empty after reconciliation (only `.gitkeep` remains).
- Use `/reconcile` to run the full procedure.
