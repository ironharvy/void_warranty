# Contributing

This repo is the source of truth for the project. If a decision, task, design change, or implementation plan is not reflected in Git, it is not authoritative.

## Core Rules

1. Do not treat chat history as the canonical record. Commit docs, tasks, and code to the repo.
2. Do not work directly on `main` for non-trivial changes.
3. One task per branch.
4. Keep branches short-lived and scoped.
5. Rebase onto the latest `main` before starting and again before merging.
6. Do not mix unrelated changes in one branch.
7. Update docs when behavior, scope, or process changes.

## Branch Naming

Use one of these formats:

- `feat/<task-id>-short-name`
- `fix/<task-id>-short-name`
- `docs/<task-id>-short-name`
- `chore/<task-id>-short-name`

Examples:

- `feat/T-012-runner-controller`
- `docs/T-005-agent-workflow`

## Pull And Sync Policy

Do not `git pull` constantly in the middle of active work. That creates churn and unnecessary conflict risk.

Instead:

### Before starting a task

Run:

```bash
git checkout main
git pull --rebase
```

Then create the task branch from updated `main`.

### While working

If your task is short and isolated, keep working without pulling.

If `main` has moved and your branch may conflict, run:

```bash
git fetch origin
git rebase origin/main
```

### Before merging

Always sync again:

```bash
git fetch origin
git rebase origin/main
```

If the branch no longer rebases cleanly, stop and resolve the conflict intentionally. Do not force through it blindly.

## Commit Policy

Each commit should do one coherent thing.

Good examples:

- `docs: define agent workflow and git rules`
- `feat: add runner movement controller`
- `fix: prevent extraction trigger from firing without objective`

Bad examples:

- `stuff`
- `wip`
- `changes`

## Task Ownership

Every non-trivial branch should map to a task file in [`tasks/`](./tasks).

The task should state:

- Task ID
- Goal
- Owner
- Status
- Files expected to change
- Acceptance criteria
- Dependencies or blockers

## Merge Criteria

A branch is ready to merge only when:

- The task file is updated.
- Relevant docs are updated.
- The implementation matches the task scope.
- Known limitations are documented.
- The branch is rebased onto current `main`.

## Avoid

- Long-lived branches with mixed work
- Silent scope changes
- Editing the same system from multiple branches without coordination
- Treating generated AI output as automatically correct
