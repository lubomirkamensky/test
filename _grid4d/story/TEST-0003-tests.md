# TEST-0003-tests

> Test definition for TEST-0003 with one test per requirement.

## Design

Test requirements for TEST-0003. One test per requirement. Commands run from
the epic root (the story worktree) in POSIX sh. R1 checks the pattern file
and the live stop-handler idle resolution. R2 counts the stale projection
files after the regeneration this story runs. R3 checks the live story
discovery for the epic and the test-sandbox subepic.

## Definition

```yaml
tests:
  - name: R1_idle_pattern_exists_and_resolved
    description: the test epic has its own idle-session pattern and the live idle instruction names it from this worktree
    command: |-
      ls _grid4d/pattern/test-simulation-idle-session-pattern.md > /dev/null && PYTHONPATH="/Users/lubomirkamensky/ahabase/evolucean/knowledge-usage-cli/src" python3 -c "
      import os, re
      from knowledge_usage_cli import hooks
      os.chdir('/Users/lubomirkamensky/ahabase/_worktrees/test/TEST-0003')
      out = re.search(r'LLM: (.*)', hooks._format_idle_status()).group(1)
      assert 'test-simulation-idle-session-pattern' in out, out
      print('OK')
      "
    expect:
      exit_code: 0
      stdout_contains: OK
  - name: R2_stale_projections_gone
    description: none of the fifteen CLI-dependent projection files exist in this tree after the story's regeneration
    command: |-
      found=$(find _grid4d -path "*_generated*" \( -name "TEST-Artifacts.md" -o -name "TEST-Capabilities.md" -o -name "TEST-Complexity.md" -o -name "TEST-Design-Patterns.md" -o -name "TEST-Orphans.md" -o -name "TEST-SANDBOX-Artifacts.md" -o -name "TEST-SANDBOX-Capabilities.md" -o -name "TEST-SANDBOX-Complexity.md" -o -name "TEST-SANDBOX-Design-Patterns.md" -o -name "TEST-SANDBOX-Orphans.md" -o -name "TEST-JIRA-Artifacts.md" -o -name "TEST-JIRA-Capabilities.md" -o -name "TEST-JIRA-Complexity.md" -o -name "TEST-JIRA-Design-Patterns.md" -o -name "TEST-JIRA-Orphans.md" \) | wc -l | tr -d ' ')
      [ "$found" = "0" ] && echo OK
    expect:
      exit_code: 0
      stdout_contains: OK
  - name: R3_story_and_subepic_discovery_work
    description: the landed discovery finds this epic story and the subepic story with correct epic attribution
    command: |-
      PYTHONPATH="/Users/lubomirkamensky/ahabase/evolucean/knowledge-usage-cli/src" python3 -c "
      from knowledge_usage_cli.discovery import find_story
      f, epic, sub = find_story('TEST-0003')
      assert epic == 'test' and sub is None, (epic, sub)
      f2, epic2, sub2 = find_story('TEST-SANDBOX-0001')
      assert epic2 == 'test' and sub2 == 'test-sandbox', (epic2, sub2)
      print('OK')
      "
    expect:
      exit_code: 0
      stdout_contains: OK
```

## Execution

| Test | Result | Date |
|------|--------|------|
| R1_idle_pattern_exists_and_resolved | ✅ | 2026-09-13 |
| R2_stale_projections_gone | ✅ | 2026-09-13 |
| R3_story_and_subepic_discovery_work | ✅ | 2026-09-13 |

## Related

- [TEST-0003](TEST-0003) - Parent story

---
## _behavior

validation:
  required_sections: [Design, Definition, Execution]
  definition_format: yaml_code_block
