# Test Parallel Session Protocol

> How two parallel Claude sessions run two stories in the test epic without
> stepping on each other. Field convention born from the first live run
> (2026-09-13, TEST-0002 + TEST-SANDBOX-0001).

**Epic:** [TEST](TEST)
**Pattern scope:** story execution in parallel sessions

## Purpose

The test epic exists to exercise story patterns through real activity. Its
signature experiment is two stories running at once in two sessions. This
pattern states the rules that make the experiment produce signal instead of
collisions.

## Rules

### R1: One story, one worktree, one session

Each parallel story runs in its own git worktree in its own session. Sessions
never share a tree: a checkout made by one session must not switch under the
other.

**Checkable rule:** `git worktree list` shows exactly one worktree per active
parallel story, and no two sessions report the same worktree as their cwd.

### R2: Worktree layout is hierarchical by epic and subepic

Worktrees live under `~/ahabase/_worktrees/<epic>/<STORY>` for epic-level
stories and `~/ahabase/_worktrees/<epic>/<subepic>/<STORY>` for subepic
stories. The story directory is named by the story ID exactly.

```
_worktrees/
└── test/
    ├── TEST-0002/                              # epic-level story
    └── test-sandbox/
        └── TEST-SANDBOX-0001/                  # subepic story
```

**Checkable rule:** for every active parallel story there exists a worktree
path matching the layout above; a flat path like `_worktrees/test-0003` is a
violation (it happened once, before this rule was written).

### R3: Story files are minted where the work happens

`story create` runs from the worktree that will host the story, so story files
never land in a tree where no work will happen. If the story ID already exists
on a branch before the worktree does (the current CLI mints the ID and leaves
files in the calling tree), the files are committed onto the story branch and
the worktree is created from that branch — the bootstrap dance recorded in the
Evolucean issue `story-create-worktree-bootstrap-manual`.

**Checkable rule:** after bootstrap, `_grid4d/**` story files for the story
exist in its worktree; the main checkout carries none of them untracked.

### R4: File territory is disjoint between parallel stories

Sibling stories declare disjoint ownership in their Notes (which directories
they own) before either starts writing. Epic-level story owns epic-level
folders; subepic story owns `subepic/<name>/` folders.

**Checkable rule:** the set of non-`_generated` files each session commits has
no intersection while both stories are open.

### R5: Shared instance state is a watchpoint, not a given

`_data/evolucean/state.json` (active_story), the counters branch, the git
remote, and DuckDB/Kuzu are shared across sessions. Every parallel run records
observations about them: who held active_story at which moment, whether any
command mis-resolved, what clobbered what. Defects become issue occurrences or
Evolucean stories — that capture is the output of the experiment.

**Checkable rule:** each parallel-run story carries a shared-state observation
section; a run that noticed nothing anomalous says so explicitly.

## Related

- [test-story-simulation-pattern](test-story-simulation-pattern) — how simulation stories are framed
- [worktree-aware-story-tooling](worktree-aware-story-tooling) — the Evolucean capability this protocol leans on
- [story-create-worktree-bootstrap-manual](story-create-worktree-bootstrap-manual) — the Evolucean issue for automating R3
