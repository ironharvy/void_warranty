# Agent Workflow

This file defines how human contributors and AI agents should operate in this repo.

## Repository Authority

Git is the source of truth.

That means:

- Design direction lives in tracked markdown files.
- Tasks live in tracked task files.
- Code changes must point back to a task.
- If a conversation changes scope, the repo must be updated to reflect it.

## Required Workflow For Agents

1. Read the relevant task file before making changes.
2. Read any referenced design docs before implementing.
3. Update from `main` before starting the branch.
4. Work in a task-scoped branch.
5. Change only files relevant to the assigned task.
6. If scope expands, update docs and task definition in the same branch.
7. Before merge, rebase onto latest `main`.

## When To Sync With Git

Agents should sync at these points:

### Always

- Before starting a new task
- Before opening or requesting merge

### As needed

- When the assigned files were modified on `main`
- When another task changed shared systems
- When conflict risk is high

Agents should not interrupt focused implementation every few minutes just to pull.

## Conflict Minimization

To reduce merge conflicts:

- Keep task ownership narrow.
- Assign distinct file sets where possible.
- Prefer additive docs over editing the same planning file repeatedly.
- Split large features into separate tasks with clear boundaries.

## Task Requirement

Each task should have its own markdown file in [`tasks/`](./tasks).

Suggested naming:

- `tasks/T-001-project-setup.md`
- `tasks/T-002-runner-controller.md`

## Status Values

Use one of:

- `todo`
- `in_progress`
- `blocked`
- `review`
- `done`

## Human Review Rules

Agents can draft code and docs, but the following should receive explicit human review before becoming the new baseline:

- Scope changes
- Architecture changes
- Asset pipeline changes
- Tooling or process changes
- Anything that alters the game pillars

## Documentation Priority

Update these when relevant:

- [`docs/game-pillars.md`](./docs/game-pillars.md)
- [`docs/one-page-gdd.md`](./docs/one-page-gdd.md)
- [`docs/vertical-slice.md`](./docs/vertical-slice.md)
- [`tasks/roadmap.md`](./tasks/roadmap.md)

## Rule Of Thumb

If an agent had to make a decision that another contributor will need later, that decision belongs in Git.
