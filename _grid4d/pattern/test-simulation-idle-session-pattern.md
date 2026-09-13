# test Simulation Idle Session

> What a Player does between stories in the test Epic, when no story is
> active. The idle frame for an Epic whose stories are probes: every
> proposal is a next experiment, not a next feature.

**Pattern type:** Player procedure (how to probe), not a document template
**Epic:** [TEST](TEST)
**Pattern scope:** idle sessions in the test Epic
**Trigger:** stop hook idle state (no active story in the test Epic)
**Frame:** [test-story-simulation-pattern](test-story-simulation-pattern)

## Purpose

The test Epic has no product backlog, no ontology to refine, and no shaping
gradients — its stories run the Evolucean story machinery and collect
evidence. An idle moment here is an invitation to pick the next mechanism to
probe. This pattern fixes that choice procedure so idle sessions stay
comparable and their output stays evidence.

## Sequence

1. **Sync** — `knowledge-usage sync` (pulls remote and regenerates all
   projections for every Epic in the instance).
2. **Frame memory** — read [test-story-simulation-pattern](test-story-simulation-pattern)
   and [test-parallel-session-protocol](test-parallel-session-protocol).
3. **Read the probes** — the story documents of this Epic and its subepics
   (including `story/history/`): what was probed, what it surfaced, what
   stayed open.
4. **Read the instruments** — this Epic's generated projections
   (`_grid4d/_generated/epic/`, the subepics' `_generated/subepic/`): after
   EVOLUCEAN-0287 the set contains only knowledge-based projections;
   a CLI-dependent projection appearing here is a defect (report to the
   owning epic, [evolucean](../evolucean)).
5. **Pick the next mechanism** — from steps 3-4, name the CLI mechanism
   (command, lifecycle stage, pattern rule) whose behavior is least
   verified for a non-evolucean Epic or for parallel sessions.
6. **Propose** — present the probe candidate (mechanism, expected evidence,
   pass/fail signal) to the Human; the Human chooses. A Human-approved probe
   becomes a story via the standard lifecycle; a defect found on the way is
   captured in the epic that owns the defect.

## Rules

- **Every proposal is a probe** — a mechanism under test, not a feature
  ([test-story-simulation-pattern](test-story-simulation-pattern) R1).
- **Evidence over status** — the session reports what the machinery did,
  not what it accomplished.
- **Defects flow to the owning epic** — the test Epic records the
  occurrence; the fix story lives where the code lives
  ([test-story-simulation-pattern](test-story-simulation-pattern) R2).
- **No story without Human choice** — the session proposes, the Human
  decides.

## Related

- [test-story-simulation-pattern](test-story-simulation-pattern) — the frame every test story follows
- [test-parallel-session-protocol](test-parallel-session-protocol) — running several probe sessions at once
- [EVOLUCEAN-0287](EVOLUCEAN-0287) — the projection applicability and per-Epic idle resolution this pattern exercises
- [TEST](TEST) — the Epic this pattern belongs to

---
