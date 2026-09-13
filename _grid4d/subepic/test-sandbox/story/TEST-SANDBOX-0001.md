# TEST-SANDBOX-0001: Validate pattern resolution from subepic: sandbox simulation story consuming epic-level patterns

> Validate pattern resolution from subepic: sandbox simulation story consuming epic-level patterns

**Type:** default
**Epic:** [TEST-SANDBOX](../TEST-SANDBOX)
**Status:** in_progress
**Blueprint:** [implementation-story-blueprint](implementation-story-blueprint)

## Goal

Run a simulation story entirely from inside subepic test-sandbox while a sibling
session (TEST-0002, epic level) seeds `test/_grid4d/pattern/`. This story is the
consumer side of the pattern-resolution experiment: it should discover, read, and
apply epic-level patterns from a subepic workspace, and record how resolution
actually behaved.

## Requirements

### R1: Epic-level pattern discovery from a subepic workspace

**Acceptance Criterion:** The story execution consults epic-level patterns
(`test/_grid4d/pattern/`, seeded by the sibling TEST-0002 session) while running in
subepic test-sandbox, and the knowledge map records which pattern documents were
consumed and from which path.

### R2: Subepic story lifecycle end-to-end

**Acceptance Criterion:** The subepic story (this one) goes through the full
lifecycle — create, execute, tests, complete — from the worktree, and every command
resolves files in `subepic/test-sandbox/story/` (not epic-level `story/`); any
mis-resolution is captured as an issue occurrence.

### R3: Parallel-session shared-state observations

**Acceptance Criterion:** Notes record what happened to shared instance state
(active_story in `_data/evolucean/state.json`, counters branch, `git worktree list`)
while both sessions were live — including any active-story clobbering, counter
races, or hook mismatches, captured as defects for the Evolucean epic.

## Acceptance Criteria

- [ ] Epic-level patterns consumed and recorded in the knowledge map from the subepic workspace
- [ ] Full subepic story lifecycle executed from the worktree with correct file resolution
- [ ] Shared-state observations recorded; defects captured as issues or Evolucean stories

## Notes

Created: 2026-09-13
CLI invocation for this session: prepend the shared CLI venv to PATH first —
`export PATH="/Users/lubomirkamensky/ahabase/evolucean/knowledge-usage-cli/.venv/bin:$PATH"`.
Executed from worktree `/Users/lubomirkamensky/ahabase/_worktrees/test/test-sandbox/TEST-SANDBOX-0001`
(branch `feature/TEST-SANDBOX-0001-validate-pattern-resolution`) in a dedicated
Claude session. Sibling: TEST-0002 (epic level, main test tree). Discovery note:
`story create --subepic` minted the ID as `TEST-SANDBOX-0001` — subepics carry
their own prefix and counter; the manual mint `SANDBOX-42` (pruned earlier today)
was wrong in both prefix and location.

### File territory (protocol R4)

This story owns `_grid4d/subepic/test-sandbox/**` in worktree
`_worktrees/test/test-sandbox/TEST-SANDBOX-0001`. It commits nothing outside
that prefix except read-only consumption elsewhere.

### R1: epic-level pattern consumption from a subepic workspace

- Resolution attempt order from this subepic worktree: subepic-local
  `_grid4d/subepic/test-sandbox/pattern/` — absent (inherit root, correct);
  epic-level `_grid4d/pattern/` in this worktree — **empty** (branch predates
  the sibling's seed); projection `_generated/epic/TEST-Patterns.md`
  (generated 14:34 from the main tree) — "*No patterns found for this Epic.*"
- The seeded patterns (`test-parallel-session-protocol`,
  `test-story-simulation-pattern`) existed only in the sibling worktree
  `_worktrees/test/TEST-0002/_grid4d/pattern/` on the unmerged branch
  `feature/TEST-0002-establish-story-patterns-in`; the main tree
  `~/ahabase/test/_grid4d/pattern/` stayed empty through this run.
- Both documents were consumed from that sibling worktree path (cross-worktree
  read; the knowledge map records them under Consumed). Both were applied:
  this Notes section follows protocol R5's observation-section requirement and
  the simulation pattern's R2 defect-pointer requirement.
- Classification: this is **not** a subepic pattern-resolution defect (that
  class is resolved — see Evolucean issue
  `subepic-story-pattern-resolution-broken`, fixed by EVOLUCEAN-0245). It is
  unmerged-work invisibility: pattern files on a sibling branch are invisible
  to every other tree, exactly as git intends. The parallel-session protocol
  (R3/R4) is the mitigation; a merged main would have resolved fine. Recorded
  as observation, no Evolucean issue needed.

### Shared-state observations (protocol R5)

All times 2026-09-13 CEST. Baseline before resume (≈15:00): `state.json`
`active_story: TEST-0002`, `active_epic: test`, pool of 5; counters branch
`origin/counters` at `1d2a88e` ("counter: TEST-SANDBOX -> 0001", 14:46:48);
worktree list: test@main `6e2926e`, TEST-0002, TEST-SANDBOX-0001.

1. **Active-story clobbering (defect, captured).** `knowledge-usage resume
   TEST-SANDBOX-0001` flipped the single global `active_story` from the
   sibling's `TEST-0002` to this story with **no warning** that another live
   session held it. `active-story` and `status` from this worktree report the
   story correctly, and the collaboration listing shows both worktrees
   (visibility is good — the silent steal is the problem). The sibling
   session independently observed the same steal from its side (TEST-0002
   watchpoint O1) — two-writer confirmation.
2. **The run was three live sessions, not two.** Between inspections
   (≈15:02–15:20) the TEST-0002 worktree HEAD moved `d4d26b2` → `82909e0`
   (watchpoints), and a third session surfaced in the evolucean epic:
   EVOLUCEAN-0282 with its own worktree `_worktrees/evolucean/EVOLUCEAN-0282`
   (its KM lists this very story and TEST-0002 as consumed). No file
   conflicts at any point — disjoint territory held across three sessions.
3. **Counters branch: race happened, machinery held.** The last counter
   entries are `fad9da4 counter: EVOLUCEAN -> 0282` then `ee8d01f counter:
   EVOLUCEAN -> 0283` — 0282 was minted concurrently with this session's
   activity window, and this story's capture mint then correctly received
   0283 (no collision, no lost update). A predicted ID written into these
   notes before minting ("0282") turned out wrong for exactly this reason;
   the real mint superseded it.
4. **KM hook validation false alarm at story start.** The PostToolUse hook
   created this story's knowledge map (15:06, correct subepic path ✓) and on
   the next read flagged it "Missing required sections: Created" — the
   top-level `## Created` section only appears once this story creates its
   first knowledge document. Self-inconsistent output at story start
   (hook-generated file failing hook validation), resolves itself once real
   documents exist.
5. **`status` banner mismatch.** `knowledge-usage status` run from this test
   worktree prints the banner `=== evolucean ===` (namespace, not the active
   epic) and `Wiki not found: test` — the test epic has no wiki configured.
   Cosmetic; active story/epic fields below the banner are correct.
6. **Cross-epic capture perturbs the observed state (recursion, confirmed
   live).** Minting the capture story flipped `active_story`/`active_epic`
   from this story to EVOLUCEAN-0283 — the capture mechanism reproduced the
   defect it captures (also seen from the sibling side, TEST-0002 O3).
7. **Stale bound tree residue (captured into the existing issue).** The
   evolucean primary tree briefly held a stray
   `EVOLUCEAN-0282-knowledge-map.md` (create-time tree binding + resume fast
   path never rebinding; TEST-0002 watchpoint diagnosis), visually merged
   into this story's capture scope until the 0282 session relocated it into
   its worktree at 15:16. Recorded as post-resolution occurrences on
   `km-logger-writes-wrong-tree`.
8. **Story-file resolution (R2) held on every command.** `resume`,
   `active-story`, `status` all resolved into
   `subepic/test-sandbox/story/`; epic-level `story/` (TEST-0001 archive +
   TEST.md) untouched throughout. Hook KM attribution followed the global
   active slot correctly at every step (my knowledge reads landed in this
   story's KM; capture-session reads landed in 0283's).
9. **`pause` leaves the global slot pointing at a paused story.** `pause` of
   EVOLUCEAN-0283 printed "Paused … remains in pool" yet `state.json` kept
   `active_story: EVOLUCEAN-0283` — the global pointer and the pool state
   disagree until the next resume. Minor facet of the same single-slot
   design as (1); recorded here, folded into the active-story issue's
   pause-related facet note.

### Defect capture pointers

- Defects (1), (4), (5) plus the stale-bound-tree residue (7) are CLI defects
  → captured under Evolucean story **EVOLUCEAN-0283** (issues
  `active-story-global-across-parallel-sessions` and
  `km-blueprint-check-false-alarm-on-fresh-knowledge-map`; occurrence added
  to `story-create-invalid-branch-name-from-description` for the
  `capture-parallelsession` slug mangling; post-resolution occurrences added
  to `km-logger-writes-wrong-tree`).
- Observations (2), (3), (6) are experiment data, not defects — recorded here
  only, no issue (by design; per simulation pattern R2 the test epic records
  the observation).
