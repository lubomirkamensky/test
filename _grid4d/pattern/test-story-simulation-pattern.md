# Test Story Simulation Pattern

> How simulation stories are framed in the test epic: every story is a live
> probe of the Evolucean story machinery, and its output is evidence, not
> features.

**Epic:** [TEST](TEST)
**Pattern scope:** story framing in the test epic

## Purpose

Stories in the test epic do not build a product. They run real activity through
the CLI's story lifecycle so that friction, defects, and surprises surface
while the stakes are low. This pattern fixes the frame so every simulation
produces comparable evidence.

## Rules

### R1: Every simulation story states what it probes

The Goal names the mechanism under test (a CLI command, a lifecycle stage, a
pattern rule), not a feature to build. Sibling stories may probe the same
mechanism from different angles (epic level vs. subepic level).

**Checkable rule:** the Goal section of a test story contains at least one
reference to a mechanism (command name, lifecycle stage, or pattern rule).

### R2: Defects flow to the owning epic

A defect found while running a test story is captured where the defect lives:
issue occurrences or new issues in the Evolucean epic for CLI problems; the
test epic only records the observation. A change to any Evolucean file requires
an Evolucean story — including issue edits (the change guard enforces this; the
first live proof was the SANDBOX-42 occurrence recorded under EVOLUCEAN-0280).

**Checkable rule:** every defect mentioned in a test story's Notes has a
pointer to an Evolucean issue or story, or states explicitly that none was
created and why.

### R3: Manual minting is a defect, not a shortcut

Story IDs are minted only through `story create`. A story file written by hand
bypasses prefix validation, counter reservation, and pool registration — the
SANDBOX-42 leftover proved all three at once (wrong prefix, wrong location,
stuck in_progress forever).

**Checkable rule:** a test story document that could not be produced by
`story create` (foreign prefix, wrong directory, missing pool entry) is
treated as an error and pruned after recording the occurrence.

### R4: Evidence over convenience in completion

A simulation story completes through the full pipeline (tests yaml, knowledge
map, verified transitions) even when the work itself is documentation. The
pipeline running on a docs-only story is itself the experiment: it proves the
machinery works for the cheapest possible story.

**Checkable rule:** the story's tests yaml runs green and the completion
transitions report verified pushes (ls-remote equal to local HEAD).

## Related

- [test-parallel-session-protocol](test-parallel-session-protocol) — running two simulation stories at once
- [implementation-story-blueprint](implementation-story-blueprint) — the Evolucean blueprint every story follows
