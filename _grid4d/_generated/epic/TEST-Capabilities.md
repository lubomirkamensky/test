# test Capabilities

> Generated: 2026-09-11 19:17

## Summary

| Metric | Count |
|--------|-------|
| Capabilities | 43 |
| OK (indexed + blueprinted) | 0 |
| Unindexed | 43 |
| Blueprint gaps | 0 |
| Dead index entries | 0 |
| Untested (advisory) | 43 |

Answers per capability: indexed in the ontology, declared in which modules, blueprint coverage of those modules, standalone test evidence.

## Capability Coverage

| Capability | Ontology index | Code modules | Blueprint | Tests | Status |
|------------|----------------|--------------|-----------|-------|--------|
| claude-cli | ✗ | `claude_cli_commands` | 0/1 | ✗ | unindexed |
| claude-config | ✗ | `claude_claude_config` | 0/1 | ✗ | unindexed |
| claude-model-selection | ✗ | `claude_model_selection` | 0/1 | ✗ | unindexed |
| claude-provider-registry | ✗ | `claude_provider_registry` | 0/1 | ✗ | unindexed |
| claude-provider-sync | ✗ | `claude_provider_sync` | 0/1 | ✗ | unindexed |
| cli-command | ✗ | `cli` | 0/1 | ✗ | unindexed |
| config-management | ✗ | `bootstrap`, `check_executor`, `cli`, `config`, `dbt_export`, `git_utils`, `km_logger`, `projections_base`, `projections_registry`, `rule_extractor`, `test_runner` | 0/11 | ✗ | unindexed |
| data-persistence | ✗ | `cli`, `db`, `parser`, `sync` | 0/4 | ✗ | unindexed |
| dbt-export | ✗ | `cli`, `dbt_export` | 0/2 | ✗ | unindexed |
| document-validation | ✗ | `capability_extractor`, `check_executor`, `cli`, `ontology`, `parser`, `snapshot`, `verify` | 0/7 | ✗ | unindexed |
| epic-bootstrap | ✗ | `bootstrap` | 0/1 | ✗ | unindexed |
| export-generation | ✗ | `capability_extractor`, `cli`, `karma_export`, `km_logger`, `parser`, `rule_extractor`, `sync`, `test_runner` | 0/8 | ✗ | unindexed |
| git-operations | ✗ | `bootstrap`, `counters`, `git_utils`, `hooks` | 0/4 | ✗ | unindexed |
| gradient-check | ✗ | `cli`, `gradient` | 0/2 | ✗ | unindexed |
| hook-handling | ✗ | `hooks` | 0/1 | ✗ | unindexed |
| instance-state | ✗ | `snapshot` | 0/1 | ✗ | unindexed |
| issue-matching | ✗ | `issue_matcher`, `verify` | 0/2 | ✗ | unindexed |
| knowledge-map-logging | ✗ | `km_logger` | 0/1 | ✗ | unindexed |
| link-management | ✗ | `cli` | 0/1 | ✗ | unindexed |
| llm-agent | ✗ | `llm_agent` | 0/1 | ✗ | unindexed |
| llm-configuration | ✗ | `cli`, `llm_config` | 0/2 | ✗ | unindexed |
| llm-lmstudio | ✗ | `cli`, `llm_lmstudio` | 0/2 | ✗ | unindexed |
| llm-model-config | ✗ | `llm_model_config` | 0/1 | ✗ | unindexed |
| llm-openrouter | ✗ | `llm_openrouter` | 0/1 | ✗ | unindexed |
| llm-paths | ✗ | `cli`, `llm_paths` | 0/2 | ✗ | unindexed |
| llm-proxy | ✗ | `llm_proxy` | 0/1 | ✗ | unindexed |
| llm-selection | ✗ | `cli`, `llm_selection` | 0/2 | ✗ | unindexed |
| llm-service | ✗ | `cli`, `llm_service` | 0/2 | ✗ | unindexed |
| llm-telemetry | ✗ | `llm_telemetry` | 0/1 | ✗ | unindexed |
| naming | ✗ | `bootstrap` | 0/1 | ✗ | unindexed |
| parsing | ✗ | `bootstrap`, `capability_extractor`, `check_executor`, `cli`, `hooks`, `km_logger`, `links`, `ontology`, `parser`, `patterns`, `rule_extractor`, `scope_role`, `status`, `test_runner` | 0/14 | ✗ | unindexed |
| pattern-driven | ✗ | `hooks` | 0/1 | ✗ | unindexed |
| pattern-inference | ✗ | `pattern_inference` | 0/1 | ✗ | unindexed |
| pattern-lookup | ✗ | `km_logger` | 0/1 | ✗ | unindexed |
| pattern-management | ✗ | `patterns` | 0/1 | ✗ | unindexed |
| pattern-resolver | ✗ | `cli`, `pattern_resolver` | 0/2 | ✗ | unindexed |
| projection-generation | ✗ | `cli`, `projections_base`, `projections_epic_artifacts`, `projections_epic_capabilities`, `projections_epic_complexity`, `projections_epic_concepts`, `projections_epic_design_patterns`, `projections_epic_gradients`, `projections_epic_graph`, `projections_epic_issues`, `projections_epic_llm_status`, `projections_epic_orphans`, `projections_epic_patterns`, `projections_epic_pool_views`, `projections_epic_shaping`, `projections_epic_stories`, `projections_epic_story_views`, `projections_epic_subepics`, `projections_epic_trace`, `projections_epic_usage`, `projections_epic_viewlib`, `projections_fragments`, `projections_namespace_base`, `projections_namespace_instance`, `projections_namespace_issues`, `projections_namespace_patterns`, `projections_registry`, `projections_utility_inheritance`, `projections_utility_validation` | 0/29 | ✗ | unindexed |
| sensor-read | ✗ | `cli`, `sensors` | 0/2 | ✗ | unindexed |
| story-tracking | ✗ | `config`, `counters`, `hooks`, `karma`, `status`, `story` | 0/6 | ✗ | unindexed |
| template-rendering | ✗ | `bootstrap` | 0/1 | ✗ | unindexed |
| test-execution | ✗ | `hooks`, `test_runner` | 0/2 | ✗ | unindexed |
| wiki-sync | ✗ | `wiki` | 0/1 | ✗ | unindexed |
| wiki-validation | ✗ | `wiki` | 0/1 | ✗ | unindexed |

## Gaps

| Capability | Status | Action |
|------------|--------|--------|
| claude-cli | unindexed | Add index entry |
| claude-config | unindexed | Add index entry |
| claude-model-selection | unindexed | Add index entry |
| claude-provider-registry | unindexed | Add index entry |
| claude-provider-sync | unindexed | Add index entry |
| cli-command | unindexed | Add index entry |
| config-management | unindexed | Add index entry |
| data-persistence | unindexed | Add index entry |
| dbt-export | unindexed | Add index entry |
| document-validation | unindexed | Add index entry |
| epic-bootstrap | unindexed | Add index entry |
| export-generation | unindexed | Add index entry |
| git-operations | unindexed | Add index entry |
| gradient-check | unindexed | Add index entry |
| hook-handling | unindexed | Add index entry |
| instance-state | unindexed | Add index entry |
| issue-matching | unindexed | Add index entry |
| knowledge-map-logging | unindexed | Add index entry |
| link-management | unindexed | Add index entry |
| llm-agent | unindexed | Add index entry |
| llm-configuration | unindexed | Add index entry |
| llm-lmstudio | unindexed | Add index entry |
| llm-model-config | unindexed | Add index entry |
| llm-openrouter | unindexed | Add index entry |
| llm-paths | unindexed | Add index entry |
| llm-proxy | unindexed | Add index entry |
| llm-selection | unindexed | Add index entry |
| llm-service | unindexed | Add index entry |
| llm-telemetry | unindexed | Add index entry |
| naming | unindexed | Add index entry |
| parsing | unindexed | Add index entry |
| pattern-driven | unindexed | Add index entry |
| pattern-inference | unindexed | Add index entry |
| pattern-lookup | unindexed | Add index entry |
| pattern-management | unindexed | Add index entry |
| pattern-resolver | unindexed | Add index entry |
| projection-generation | unindexed | Add index entry |
| sensor-read | unindexed | Add index entry |
| story-tracking | unindexed | Add index entry |
| template-rendering | unindexed | Add index entry |
| test-execution | unindexed | Add index entry |
| wiki-sync | unindexed | Add index entry |
| wiki-validation | unindexed | Add index entry |

## Untested (advisory)

No standalone test script mentions the capability. Advisory only: yaml story tests assert by stdout strings and are not counted here.

- claude-cli
- claude-config
- claude-model-selection
- claude-provider-registry
- claude-provider-sync
- cli-command
- config-management
- data-persistence
- dbt-export
- document-validation
- epic-bootstrap
- export-generation
- git-operations
- gradient-check
- hook-handling
- instance-state
- issue-matching
- knowledge-map-logging
- link-management
- llm-agent
- llm-configuration
- llm-lmstudio
- llm-model-config
- llm-openrouter
- llm-paths
- llm-proxy
- llm-selection
- llm-service
- llm-telemetry
- naming
- parsing
- pattern-driven
- pattern-inference
- pattern-lookup
- pattern-management
- pattern-resolver
- projection-generation
- sensor-read
- story-tracking
- template-rendering
- test-execution
- wiki-sync
- wiki-validation