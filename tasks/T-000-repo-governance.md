# Task ID

`T-000`

## Title

Repository governance and agent workflow

## Status

`done`

## Owner

Codex

## Summary

Define the repository operating model so Git remains the project source of truth while multiple AI agents and humans contribute.

## Scope

- [`CONTRIBUTING.md`](../CONTRIBUTING.md)
- [`AGENTS.md`](../AGENTS.md)
- [`tasks/TEMPLATE.md`](./TEMPLATE.md)
- [`README.md`](../README.md)

## Out Of Scope

- Branch protection automation
- CI setup
- Unity project creation

## Dependencies

- [`docs/game-pillars.md`](../docs/game-pillars.md)
- [`tasks/roadmap.md`](./roadmap.md)

## Acceptance Criteria

- Repo-level git workflow rules are documented.
- Agent-specific workflow rules are documented.
- A reusable task template exists.
- The repo README points contributors at the governance docs.

## Notes

- The sync policy is "always before starting and before merging, otherwise as needed."
