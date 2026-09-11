# SANDBOX-42: Jira-imported story live test

> Simulated Jira-imported story (project SANDBOX, ticket 42) to test the lifecycle of a story whose ID was minted outside the CLI, created here manually because `story create` has no `--id` option yet.

**Type:** default
**Epic:** [TEST](TEST)
**Status:** in_progress
**Blueprint:** [implementation-story-blueprint](implementation-story-blueprint)

## Goal

Validate that a story with a foreign (Jira-style) ID participates in the story lifecycle: resolution, pause/resume, status rendering, branch derivation, and version computation.

## Requirements

### R1: Foreign-ID story lifecycle

The story file exists, resolves through pattern/type machinery, and can be paused/resumed; branch and version derivation produce sane values for a non-epic-prefix ID.

**Acceptance Criterion:** SANDBOX-42 can be paused and resumed; derived branch matches feature/SANDBOX-42-*; no crash in status or version computation.

## Notes

Created manually 2026-09-11 as part of TEST-0001 live testing (Jira story IDs candidate validation).

## References

---