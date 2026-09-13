# TEST-0001-tests

> Test definition for TEST-0001 with one test per requirement.

## Design

TEST-0001 is a sandbox story: it validates story/subepic machinery live and
files its findings as issues/ideas in the evolucean Epic. The deterministic
contract is narrow - the sandbox artifacts exist and the filed knowledge
documents are resolvable by name from this Epic.

## Definition

```yaml
tests:
  - name: R1_sandbox_artifacts_exist
    description: sandbox artifacts created by the experiments are on disk
    command: 'test -f _grid4d/story/SANDBOX-42.md && test -d _grid4d/subepic/test-jira/story && test -f _grid4d/subepic/test-jira/story/TEST-JIRA-0001.md && echo "R1: artifacts verified"'
    expect:
      exit_code: 0
      stdout_contains: "R1: artifacts verified"
  - name: R1_findings_filed_cross_epic
    description: the issue and idea filed in evolucean by this story exist
    command: 'test -f ../evolucean/_grid4d/issue/subepic-story-pattern-resolution-broken.md && test -f ../evolucean/_grid4d/idea/jira-generated-story-ids.md && echo "R1: findings filed"'
    expect:
      exit_code: 0
      stdout_contains: "R1: findings filed"
    expect:
      exit_code: 0
      stdout_contains: "R1: findings filed"
```

## Execution

| Test | Result | Date |
|------|--------|------|
| R1_sandbox_artifacts_exist | ✅ | 2026-09-11 |
| R1_findings_filed_cross_epic | ✅ | 2026-09-11 |

## Related

- [TEST-0001](TEST-0001) - Parent story

---
## _behavior

validation:
  required_sections: [Design, Definition, Execution]
  definition_format: yaml_code_block
