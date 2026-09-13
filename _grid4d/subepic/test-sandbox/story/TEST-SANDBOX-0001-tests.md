# TEST-SANDBOX-0001-tests

> Test definition for TEST-SANDBOX-0001 with one test per requirement.

## Design

Pattern-resolution sandbox story run from the subepic worktree. R1 asserts
the knowledge map records both epic-level pattern documents consumed during
the run. R2 asserts story files live in the subepic story folder and never
leaked into the epic-level story folder. R3 asserts the story Notes carry
the shared-state observation section with the counters statement and the
Evolucean capture pointer. Paths are relative to the Epic root (this
worktree).

## Definition

```yaml
tests:
  - name: R1_patterns_consumed_in_knowledge_map
    description: knowledge map records both epic-level pattern documents
    command: grep -q "test-parallel-session-protocol" _grid4d/subepic/test-sandbox/story/TEST-SANDBOX-0001-knowledge-map.md && grep -q "test-story-simulation-pattern" _grid4d/subepic/test-sandbox/story/TEST-SANDBOX-0001-knowledge-map.md
    expect:
      exit_code: 0
  - name: R2_subepic_story_file_resolution
    description: story files resolve in the subepic folder with no epic-level leak
    command: test -f _grid4d/subepic/test-sandbox/story/TEST-SANDBOX-0001.md && test -f _grid4d/subepic/test-sandbox/story/TEST-SANDBOX-0001-tests.md && test ! -e _grid4d/story/TEST-SANDBOX-0001.md
    expect:
      exit_code: 0
  - name: R3_shared_state_observations_recorded
    description: Notes carry the observation section with counters statement and capture pointer
    command: grep -q "Shared-state observations" _grid4d/subepic/test-sandbox/story/TEST-SANDBOX-0001.md && grep -q "race happened" _grid4d/subepic/test-sandbox/story/TEST-SANDBOX-0001.md && grep -q "EVOLUCEAN-0283" _grid4d/subepic/test-sandbox/story/TEST-SANDBOX-0001.md
    expect:
      exit_code: 0
```

## Execution

| Test | Result | Date |
|------|--------|------|
| R1_patterns_consumed_in_knowledge_map | ✅ | 2026-09-13 |
| R2_subepic_story_file_resolution | ✅ | 2026-09-13 |
| R3_shared_state_observations_recorded | ✅ | 2026-09-13 |

## Related

- [TEST-SANDBOX-0001](TEST-SANDBOX-0001) - Parent story

---
## _behavior

validation:
  required_sections: [Design, Definition, Execution]
  definition_format: yaml_code_block
