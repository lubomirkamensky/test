# test CLI Artifacts

> Generated: 2026-09-11 19:17

## Summary

| Metric | Value | Coverage |
|--------|-------|----------|
| Modules | 75 | - |
| Blueprints | 72/75 | 96% |
| Test Files | 32/75 | 42% |
| Functions | 931 | - |
| With Capability | 838/931 | 90% |
| Commands | 96 | - |
| Capabilities | 43 | - |
| Tests Passed | 89/89 | 100% |

## Test Coverage

Modules directly exercised by the regression tree (`Module_TestCov` sensor: at least one `EVOLUCEAN-*-tests.py` suite imports the module):

*No test coverage measured (no CLI modules found).*

## Modules Overview

| Module | Blueprint | Tests | Functions | Capabilities |
|--------|-----------|-------|-----------|--------------|
| [bootstrap](#bootstrap) | ✓ | - | 12 | 12/12 |
| [capability_extractor](#capability-extractor) | ✓ | 2/2 | 7 | 7/7 |
| [check_executor](#check-executor) | ✓ | 7/7 | 13 | 13/13 |
| [claude_claude_config](#claude-claude-config) | ✓ | 0/0 | 11 | 11/11 |
| [claude_cli_commands](#claude-cli-commands) | ✓ | 11/11 | 17 | 17/17 |
| [claude_model_selection](#claude-model-selection) | ✓ | 0/0 | 10 | 10/10 |
| [claude_provider_registry](#claude-provider-registry) | ✓ | 0/0 | 20 | 20/20 |
| [claude_provider_sync](#claude-provider-sync) | ✓ | 0/0 | 6 | 6/6 |
| [cli](#cli) | ✓ | 8/8 | 109 | 106/109 |
| [config](#config) | ✓ | 7/7 | 63 | 61/63 |
| [counters](#counters) | ✓ | - | 8 | 8/8 |
| [db](#db) | ✓ | 6/6 | 12 | 12/12 |
| [dbt_export](#dbt-export) | ✓ | - | 9 | 9/9 |
| [discovery](#discovery) | ✓ | - | 12 | 0/12 |
| [git_utils](#git-utils) | ✓ | 5/5 | 12 | 12/12 |
| [gradient](#gradient) | ✓ | - | 3 | 3/3 |
| [hooks](#hooks) | ✓ | 7/7 | 32 | 32/32 |
| [issue_matcher](#issue-matcher) | ✓ | 2/2 | 4 | 4/4 |
| [karma](#karma) | ✓ | 2/2 | 2 | 2/2 |
| [karma_export](#karma-export) | ✓ | - | 4 | 4/4 |
| [km_logger](#km-logger) | ✓ | 6/6 | 8 | 8/8 |
| [links](#links) | ✓ | 2/2 | 3 | 3/3 |
| [llm_agent](#llm-agent) | ✓ | - | 8 | 8/8 |
| [llm_config](#llm-config) | ✓ | - | 9 | 9/9 |
| [llm_lmstudio](#llm-lmstudio) | ✓ | 0/0 | 16 | 16/16 |
| [llm_model_config](#llm-model-config) | ✓ | 0/0 | 22 | 22/22 |
| [llm_openrouter](#llm-openrouter) | ✓ | 0/0 | 9 | 9/9 |
| [llm_paths](#llm-paths) | ✓ | - | 11 | 11/11 |
| [llm_proxy](#llm-proxy) | ✓ | 0/0 | 19 | 19/19 |
| [llm_selection](#llm-selection) | ✓ | - | 5 | 5/5 |
| [llm_service](#llm-service) | ✓ | 0/0 | 27 | 27/27 |
| [llm_telemetry](#llm-telemetry) | ✓ | - | 22 | 18/22 |
| [ontology](#ontology) | ✓ | 2/2 | 5 | 5/5 |
| [parser](#parser) | ✓ | 0/0 | 14 | 14/14 |
| [pattern_inference](#pattern-inference) | ✓ | - | 5 | 5/5 |
| [pattern_resolver](#pattern-resolver) | ✓ | - | 6 | 6/6 |
| [patterns](#patterns) | ✓ | 0/0 | 7 | 7/7 |
| [projections_base](#projections-base) | ✓ | - | 11 | 11/11 |
| [projections_epic_artifacts](#projections-epic-artifacts) | ✓ | - | 7 | 7/7 |
| [projections_epic_capabilities](#projections-epic-capabilities) | ✓ | - | 8 | 8/8 |
| [projections_epic_complexity](#projections-epic-complexity) | ✓ | - | 10 | 10/10 |
| [projections_epic_concepts](#projections-epic-concepts) | ✓ | - | 8 | 8/8 |
| [projections_epic_design_patterns](#projections-epic-design-patterns) | ✓ | - | 10 | 10/10 |
| [projections_epic_gradients](#projections-epic-gradients) | ✓ | - | 11 | 3/11 |
| [projections_epic_graph](#projections-epic-graph) | ✓ | - | 6 | 5/6 |
| [projections_epic_issues](#projections-epic-issues) | ✓ | - | 3 | 3/3 |
| [projections_epic_llm_status](#projections-epic-llm-status) | ✓ | - | 8 | 8/8 |
| [projections_epic_orphans](#projections-epic-orphans) | ✓ | - | 13 | 13/13 |
| [projections_epic_patterns](#projections-epic-patterns) | ✓ | - | 4 | 4/4 |
| [projections_epic_pool_views](#projections-epic-pool-views) | - | - | 15 | 4/15 |
| [projections_epic_shaping](#projections-epic-shaping) | ✓ | - | 7 | 7/7 |
| [projections_epic_stories](#projections-epic-stories) | ✓ | - | 5 | 5/5 |
| [projections_epic_story_views](#projections-epic-story-views) | - | - | 14 | 4/14 |
| [projections_epic_subepics](#projections-epic-subepics) | ✓ | - | 3 | 3/3 |
| [projections_epic_trace](#projections-epic-trace) | ✓ | - | 21 | 4/21 |
| [projections_epic_usage](#projections-epic-usage) | ✓ | - | 5 | 3/5 |
| [projections_epic_viewlib](#projections-epic-viewlib) | - | - | 5 | 5/5 |
| [projections_fragments](#projections-fragments) | ✓ | - | 3 | 3/3 |
| [projections_namespace_base](#projections-namespace-base) | ✓ | - | 3 | 3/3 |
| [projections_namespace_instance](#projections-namespace-instance) | ✓ | - | 26 | 25/26 |
| [projections_namespace_issues](#projections-namespace-issues) | ✓ | - | 10 | 10/10 |
| [projections_namespace_patterns](#projections-namespace-patterns) | ✓ | - | 4 | 4/4 |
| [projections_registry](#projections-registry) | ✓ | - | 7 | 7/7 |
| [projections_utility_inheritance](#projections-utility-inheritance) | ✓ | - | 7 | 7/7 |
| [projections_utility_validation](#projections-utility-validation) | ✓ | - | 10 | 9/10 |
| [rule_extractor](#rule-extractor) | ✓ | 4/4 | 8 | 8/8 |
| [scope_role](#scope-role) | ✓ | 2/2 | 3 | 3/3 |
| [sensors](#sensors) | ✓ | - | 33 | 29/33 |
| [snapshot](#snapshot) | ✓ | 5/5 | 20 | 20/20 |
| [status](#status) | ✓ | 5/5 | 4 | 4/4 |
| [story](#story) | ✓ | 0/0 | 28 | 12/28 |
| [sync](#sync) | ✓ | 0/0 | 6 | 5/6 |
| [test_runner](#test-runner) | ✓ | 6/6 | 7 | 7/7 |
| [verify](#verify) | ✓ | 0/0 | 7 | 7/7 |
| [wiki](#wiki) | ✓ | - | 9 | 9/9 |

---

## Module Details

### bootstrap

> Epic bootstrap: turn the startup ritual into validated commands.

**Blueprint:** [implementation-cli-bootstrap-blueprint](implementation-cli-bootstrap-blueprint)
**Tests:** -
**Functions:** 12 (12 with Capability)

#### config-management

| Function | Description |
|----------|-------------|
| `load_registry` | Parse the ahabase registry. |
| `register_epic` | Add the epic and its story prefix to the config dict; rai... |
| `register_subepic` | Add a subepic under its epic in the config dict; raise on... |
| `write_registry` | Write the registry atomically, header preserved, re-valid... |

#### epic-bootstrap

| Function | Description |
|----------|-------------|
| `epic_init` | Scaffold the Epic skeleton and register it; return the ac... |
| `subepic_init` | Scaffold a minimal SubEpic inside an initialized Epic; re... |

#### git-operations

| Function | Description |
|----------|-------------|
| `read_remote` | Credential-free origin remote URL of the prepared clone. |

#### naming

| Function | Description |
|----------|-------------|
| `canonical_subepic` | SubEpic name carries the epic prefix (evolucean-timbrcli ... |

#### parsing

| Function | Description |
|----------|-------------|
| `clean_remote_url` | Strip credentials from an https remote URL. |
| `remote_owner` | GitHub account owning the remote, when discoverable. |

#### template-rendering

| Function | Description |
|----------|-------------|
| `epic_identity` | Identity document for a fresh Epic (EVOLUCEAN shape, no g... |
| `subepic_identity` | Identity document for a fresh SubEpic (EVOLUCEAN-TIMBRCLI... |

### capability_extractor

> Extract Capabilities from CLI modules.

**Blueprint:** [implementation-cli-capability_extractor-blueprint](implementation-cli-capability_extractor-blueprint)
**Tests:** 2/2 (pass)
**Functions:** 7 (7 with Capability)

#### document-validation

| Function | Description |
|----------|-------------|
| `validate_module_capabilities` | Validate all functions in module have Capability declared. |

#### export-generation

| Function | Description |
|----------|-------------|
| `_extract_function_info` | Extract function info from AST node. |
| `extract_capabilities_by_module` | Extract Capabilities grouped by capability name. |
| `extract_cli_commands` | Extract CLI commands from @cli.command decorators. |
| `extract_module_functions` | Extract top-level functions and class methods with their ... |
| `get_valid_capabilities` | Get list of Capabilities from CLI code. |

#### parsing

| Function | Description |
|----------|-------------|
| `extract_capability_from_docstring` | Extract Capability tag from docstring. |

### check_executor

> Execute validation checks from document-rules.yml.

**Blueprint:** [implementation-cli-check_executor-blueprint](implementation-cli-check_executor-blueprint)
**Tests:** 7/7 (pass)
**Functions:** 13 (13 with Capability)

#### config-management

| Function | Description |
|----------|-------------|
| `load_document_rules` | Load document-rules.yml. |

#### document-validation

| Function | Description |
|----------|-------------|
| `check_at_least_one` | Check that at least one of the listed sections exists. |
| `check_has_subsection` | Check that parent sections have required child subsections. |
| `check_list_format` | Check that sections use list format: - `[doc](link)`. |
| `check_not_empty` | Check that sections contain at least one item. |
| `check_unique_across` | Check that document links don't appear in multiple sections. |
| `execute_checks` | Execute all checks against content. |
| `validate_document` | Validate document content against rules for its type. |
| `validate_type_blueprint` | Validate type-blueprint: Template must pass its own Valid... |

#### parsing

| Function | Description |
|----------|-------------|
| `extract_links_from_section` | Extract markdown links from a section (## or ###). |
| `extract_template_content` | Extract content from ## Template section's markdown code ... |
| `find_sections` | Find ## headings, ignoring code blocks. |
| `find_subsections` | Find ### headings under a ## parent section. |

### claude_claude_config

> Claude Code configuration management with context-aware provider discovery.

**Blueprint:** [implementation-cli-claude_claude_config-blueprint](implementation-cli-claude_claude_config-blueprint)
**Tests:** 0/0 (not_run)
**Functions:** 11 (11 with Capability)

#### claude-config

| Function | Description |
|----------|-------------|
| `__post_init__` | Initialize default values. |
| `__post_init__` | Initialize default values. |
| `detect_environment_context` | Detect environment context (personal vs enterprise). |
| `discover_providers` | Discover available providers based on current environment. |
| `get_current_provider` | Get currently configured provider type from Claude Code s... |
| `get_machine_id` | Get unique machine identifier. |
| `get_settings_path` | Get Claude Code settings.json path. |
| `read_settings` | Read Claude Code settings.json. |
| `select_best_provider` | Select best provider from available options. |
| `test_provider_availability` | Test if provider is available on current machine. |
| `write_settings` | Write Claude Code settings.json atomically. |

### claude_cli_commands

> CLI commands for Claude Code configuration management.

**Blueprint:** [implementation-cli-claude_cli_commands-blueprint](implementation-cli-claude_cli_commands-blueprint)
**Tests:** 11/11 (pass)
**Functions:** 17 (17 with Capability)

#### claude-cli

| Function | Description |
|----------|-------------|
| `_create_backup` | Create backup of settings file. |
| `_get_last_known_good_path` | Get path to last-known-good settings file. |
| `_save_last_known_good` | Save current settings as last-known-good. |
| `_validate_provider_switch` | Validate that new provider is accessible. |
| `_write_settings_atomic` | Write settings file atomically (temp file + rename). |
| `get_current_provider_and_model` | Get current provider and model information. |
| `get_model_history` | Get model usage history. |
| `list_backups` | List available backup files. |
| `list_provider_models` | List available models for a provider. |
| `list_providers` | List all providers with local availability. |
| `restore_backup` | Restore settings from backup. |
| `rollback_last_known_good` | Rollback to last known good configuration. |
| `set_model_preference` | Set user preference for a model. |
| `show_status` | Show current Claude Code configuration status. |
| `switch_model_only` | Switch to a different model of the current provider. |
| `switch_provider` | Switch to a different provider with automatic rollback on... |
| `switch_provider_with_model` | Switch to a provider with model selection. |

### claude_model_selection

> Model selection and management for Claude Code providers.

**Blueprint:** [implementation-cli-claude_model_selection-blueprint](implementation-cli-claude_model_selection-blueprint)
**Tests:** 0/0 (not_run)
**Functions:** 10 (10 with Capability)

#### claude-model-selection

| Function | Description |
|----------|-------------|
| `__post_init__` | Convert category string to enum. |
| `format_provider_models_for_registry` | Format ProviderModels for registry YAML. |
| `get_available_models` | Get list of available model IDs. |
| `get_model_info` | Get info for a specific model. |
| `get_model_stats` | Get stats for a model, create if not exists. |
| `parse_provider_models` | Parse provider models from registry data. |
| `recommend_models` | Recommend alternative models based on usage and preferences. |
| `record_usage` | Record model usage. |
| `select_best_model` | Select best model based on preferences and stats. |
| `set_user_preference` | Set user preference for a model. |

### claude_provider_registry

> Provider registry with per-machine availability tracking.

**Blueprint:** [implementation-cli-claude_provider_registry-blueprint](implementation-cli-claude_provider_registry-blueprint)
**Tests:** 0/0 (not_run)
**Functions:** 20 (20 with Capability)

#### claude-provider-registry

| Function | Description |
|----------|-------------|
| `from_dict` | Create from YAML data. |
| `from_dict` | Create from YAML data. |
| `from_dict` | Create from YAML data. |
| `from_dict` | Create from YAML data. |
| `get_available_providers` | Get providers available on local machine. |
| `get_default_model` | Get default model from models dict. |
| `get_default_registry_path` | Get the shipped default (seed) registry path. |
| `get_local_availability` | Get availability info for local machine. |
| `get_provider_by_type` | Get provider config by type. |
| `get_registry_path` | Get the live provider registry YAML path. |
| `import_provider_from_discovery` | Import discovered provider into registry. |
| `is_experimental` | Check if this provider is marked as experimental. |
| `load_registry` | Load provider registry from YAML file. |
| `save_registry` | Save provider registry to YAML file atomically. |
| `to_dict` | Convert to YAML-serializable dict. |
| `to_dict` | Convert to YAML-serializable dict. |
| `to_dict` | Convert to YAML-serializable dict. |
| `to_dict` | Convert to YAML-serializable dict. |
| `update_local_availability` | Update availability for local machine. |
| `update_local_context` | Update context metadata for local machine. |

### claude_provider_sync

> Multi-machine sync for provider registry with context-preserving merge.

**Blueprint:** [implementation-cli-claude_provider_sync-blueprint](implementation-cli-claude_provider_sync-blueprint)
**Tests:** 0/0 (not_run)
**Functions:** 6 (6 with Capability)

#### claude-provider-sync

| Function | Description |
|----------|-------------|
| `_is_newer` | Check if remote timestamp is newer than local. |
| `_merge_providers` | Merge two provider configs with conflict resolution. |
| `get_registry_sync_status` | Get current sync status of provider registry. |
| `merge_registries` | Merge remote registry into local registry with context-pr... |
| `simulate_sync` | Simulate sync without making changes (dry-run). |
| `sync_provider_registry` | Sync provider registry from remote to local. |

### cli

> CLI entry point.

**Blueprint:** [implementation-cli-cli-blueprint](implementation-cli-cli-blueprint)
**Tests:** 8/8 (pass)
**Functions:** 109 (106 with Capability)

#### cli-command

| Function | Description |
|----------|-------------|
| `_is_story_file` | Check if file is a story file (TICKET-*.md pattern). |
| `_verify_file_internal` | Internal verify-file logic. Returns output string or None. |
| `active_story` | Show current active story and model (debug command). |
| `claude` | Claude Code configuration management. |
| `claude_current` | Show current provider and model with recommendations. |
| `claude_doctor` | Audit Claude Code hook events: OK / DRIFT / DEAD + opport... |
| `claude_list` | List all providers with local availability. |
| `claude_list_backups` | List available backup files. |
| `claude_list_models` | List available models for a provider. |
| `claude_model_history` | Show model usage history. |
| `claude_prefer_model` | Set preference for a model (preferred/avoid). |
| `claude_restore` | Restore settings from backup. |
| `claude_rollback` | Rollback to last known good configuration (FASTEST recove... |
| `claude_status` | Show current Claude Code configuration with context. |
| `claude_switch` | Switch to a different Claude Code provider with automatic... |
| `claude_switch_model` | Switch to a different model of the current provider. |
| `claude_sync` | Sync provider registry from remote source. |
| `claude_sync_simulate` | Simulate provider registry sync without making changes. |
| `claude_sync_status` | Show provider registry sync status. |
| `config` | Configuration management. |
| `config` | Configuration management commands. |
| `config_check_token` | Check if GitHub token(s) are valid. |
| `config_show` | Show current configuration. |
| `config_update_token` | Update GitHub PAT token for an organization. |
| `doctor` | Check installation and dependencies. |
| `extract_rules` | Extract validation rules from type-blueprints. |
| `fork` | Create a new version (fork) of a document. |
| `hook_handler` | Handle PostToolUse hooks from Claude Code. |
| `karma` | Show karma metrics. |
| `llm` | LLM and LiteLLM proxy management. |
| `llm_check` | Check LLM configuration and dependencies. |
| `llm_init` | Initialize LLM module configuration. |
| `llm_proxy_configure` | Configure Claude Code to use LiteLLM proxy. |
| `llm_proxy_generate_config` | Generate LiteLLM proxy configuration file. |
| `llm_proxy_start` | Start LiteLLM proxy for Claude Code integration. |
| `llm_proxy_status` | Check LiteLLM proxy status. |
| `llm_proxy_stop` | Stop LiteLLM proxy server. |
| `llm_telemetry_env` | Show (default) or install the telemetry env block. |
| `llm_telemetry_start` | Start the agent telemetry OTLP collector. |
| `llm_telemetry_status` | Show collector status, last activity and env-block state. |
| `llm_telemetry_stop` | Stop the agent telemetry OTLP collector. |
| `llm_update` | Update OpenRouter free models list from API. |
| `ontology` | Ontology management commands. |
| `pattern` | Pattern management and debugging commands. |
| `pattern_list` | List available patterns for a context. |
| `pattern_show` | Show effective pattern with lineage info. |
| `pattern_validate` | Validate all documents against their patterns. |
| `pause_story` | Pause active story - keeps it in pool but stops tracking. |
| `resume_story` | Resume a story from pool (or show pool if no argument). |
| `snapshot` | Instance State management via snapshots. |
| `snapshot_baseline` | Tag current snapshot as baseline for Story. |
| `snapshot_completion` | Tag current snapshot as completion for Story. |
| `snapshot_create` | Create new snapshot of Instance. |
| `snapshot_diff` | Show diff between snapshots. |
| `snapshot_list` | List recent snapshots. |
| `status` | Show game status - active story, open stories, debt. |
| `stop_handler` | Game Master - show game status and guide next move. |
| `test` | Execute tests from a -tests.md file. |
| `test_role` | Test role determination (for testing). |
| `test_scope` | Test scope determination (for testing). |
| `verify_file_cmd` | Verify single file structure against its blueprint. |
| `verify_stdin_cmd` | Verify content from stdin against document type rules. |

#### config-management

| Function | Description |
|----------|-------------|
| `cli` | Knowledge Usage CLI - local processing of knowledge usage... |
| `init` | Setup complete Evolucean game board. |

#### data-persistence

| Function | Description |
|----------|-------------|
| `sync` | Pull + parse + load + verify + export (if changes). |
| `verify` | Check consistency (MD == JSON == DBs + Capabilities). |

#### dbt-export

| Function | Description |
|----------|-------------|
| `export_dbt` | Generate dbt project exports for an epic. |

#### document-validation

| Function | Description |
|----------|-------------|
| `ontology_validate` | Validate ontology/ folder structure and cross-references. |
| `verify_capabilities` | Verify Capability declarations in CLI module(s). |

#### export-generation

| Function | Description |
|----------|-------------|
| `export_karma` | Generate Karma-Report.md to all Epics. |
| `extract_functions` | Extract functions with Capabilities from CLI module. |

#### gradient-check

| Function | Description |
|----------|-------------|
| `export_gradient` | Generate gradient report comparing blueprints to code. |

#### link-management

| Function | Description |
|----------|-------------|
| `link` | Link management commands. |
| `link_fix` | Fix path_in_link issues by converting to filename-only. |

#### llm-configuration

| Function | Description |
|----------|-------------|
| `llm_config_status` | Show which LLM hook instructions come from the pattern vs... |

#### llm-lmstudio

| Function | Description |
|----------|-------------|
| `llm_lmstudio_auto_setup` | Complete automated LM Studio setup. |
| `llm_lmstudio_download_model` | Download and load model to LM Studio. |
| `llm_lmstudio_install` | Check/install LM Studio application. |

#### llm-paths

| Function | Description |
|----------|-------------|
| `llm_path_list` | List known LLM access paths and which one is current. |
| `llm_path_switch` | Switch Claude Code to a verified access path (preflight f... |
| `llm_path_verify` | Preflight-verify an access path with a minimal messages r... |
| `llm_recover` | Revive the LiteLLM proxy offline (run outside Claude Code). |

#### llm-selection

| Function | Description |
|----------|-------------|
| `llm_step_map` | Show step profiles and the selection proposal for a task ... |

#### llm-service

| Function | Description |
|----------|-------------|
| `llm_discover_models` | Discover currently working free models from OpenRouter. |
| `llm_free_models_update` | Update OpenRouter free models in config.yaml. |
| `llm_lmstudio_daemon_logs` | Show LM Studio daemon logs. |
| `llm_lmstudio_daemon_restart` | Restart LM Studio daemon. |
| `llm_lmstudio_daemon_start` | Start LM Studio daemon. |
| `llm_lmstudio_daemon_status` | Check LM Studio daemon status. |
| `llm_lmstudio_daemon_stop` | Stop LM Studio daemon. |
| `llm_lmstudio_status` | Check LM Studio status and loaded model. |
| `llm_lmstudio_test` | Test LM Studio completion. |
| `llm_lmstudio_watchdog` | LM Studio watchdog - check and auto-restart. |
| `llm_recommend_config` | Generate recommended LiteLLM config based on working models. |
| `llm_service_doctor` | Run LiteLLM service diagnostics. |
| `llm_service_install` | Install and start LiteLLM as launchd service. |
| `llm_service_logs` | Show LiteLLM service logs. |
| `llm_service_restart` | Restart LiteLLM launchd service. |
| `llm_service_status` | Show LiteLLM launchd service status. |
| `llm_service_uninstall` | Uninstall LiteLLM launchd service. |

#### parsing

| Function | Description |
|----------|-------------|
| `query` | Run ad-hoc query. |

#### pattern-resolver

| Function | Description |
|----------|-------------|
| `pattern_fix` | Rename patterns to use epic/subepic prefix. |

#### projection-generation

| Function | Description |
|----------|-------------|
| `projection` | Generate Epic-level projections to _generated/epic/. |

#### sensor-read

| Function | Description |
|----------|-------------|
| `sensor` | Internal sensor registry (implementation-cli-sensors-blue... |
| `sensor_list` | List registered sensors and their gradient metrics. |
| `sensor_read` | Measure all implemented sensors and store readings to Duc... |

#### unassigned

| Function | Description |
|----------|-------------|
| `epic` | Epic bootstrap: init a new Epic or SubEpic from a prepare... |
| `epic_init_cmd` | Scaffold NAME inside its prepared clone and register it i... |
| `epic_init_subepic_cmd` | Scaffold a minimal SubEpic NAME inside an initialized EPI... |

### config

> Configuration management.

**Blueprint:** [implementation-cli-config-blueprint](implementation-cli-config-blueprint)
**Tests:** 7/7 (pass)
**Functions:** 63 (61 with Capability)

#### config-management

| Function | Description |
|----------|-------------|
| `_expand_path` | Expand ~ and return Path. |
| `_get_settings_path` | Find settings file in order of precedence. |
| `_get_subepic_for_story` | Get subepic name for a story based on prefix. |
| `check_github_token` | Check if GitHub token for an org is valid. |
| `ensure_gh_account` | Ensure correct GitHub account is active for Epic. |
| `get_all_repositories` | Get all configured repositories. |
| `get_all_story_prefixes` | Get all story prefixes for an Epic including subepics. |
| `get_claude_hooks` | Get Claude Code hooks configuration with CLI path substit... |
| `get_cli_src_dir` | Get CLI source code directory. |
| `get_clone_url` | Get authenticated clone URL for repository. |
| `get_config_dir` | Get the config directory. |
| `get_configured_epics` | Get Epic paths using filesystem discovery. |
| `get_configured_epics_knowledge` | Get Epic knowledge paths (_grid4d folders). |
| `get_configured_knowledge_paths` | Get Epic knowledge paths (_grid4d folders). |
| `get_data_dir` | Get the data directory, creating if needed. |
| `get_document_types` | Get document type to blueprint mapping from settings. |
| `get_epic_branch` | Get merge target branch for an Epic or SubEpic. |
| `get_epic_from_knowledge_path` | Get Epic path from a knowledge path. |
| `get_epic_gh_account` | Get GitHub account for an Epic. |
| `get_epic_git_operations` | Get whether to perform git operations (commit/merge/push)... |
| `get_epic_knowledge_path` | Get knowledge path for an Epic (e.g., evolucean/_grid4d). |
| `get_epic_merge` | Get whether to merge to target branch for an Epic or SubE... |
| `get_epic_names` | All epic names to iterate: discovered on disk + legacy-co... |
| `get_epic_release` | Get whether to create release for an Epic or SubEpic. |
| `get_epic_snapshot_on_complete` | Get whether to create ahabase snapshot on story completion. |
| `get_epic_story_history_keep` | Get number of stories to keep in story root (others go to... |
| `get_epic_story_lifecycle` | Get story lifecycle config for an Epic. |
| `get_github_token_orgs` | Get list of GitHub orgs that use token authentication via... |
| `get_idle_stop_cooldown_seconds` | Get stop handler cooldown in seconds when no story is act... |
| `get_json_dir` | Get JSON cache directory for parsed stories. |
| `get_primary_epic` | Get primary Epic name from settings. |
| `get_primary_wiki` | Get primary Epic name from settings. |
| `get_project_root` | Get the project root directory. |
| `get_queries_dir` | Get SQL/Cypher queries directory. |
| `get_repo_path` | Get full path to repository. |
| `get_repository_config` | Get repository config by name. |
| `get_schema_dir` | Get database schema directory. |
| `get_state_path` | Get the state file path (inside data_dir). |
| `get_stop_cooldown_seconds` | Get stop handler cooldown in seconds. |
| `get_story_lifecycle` | Get story lifecycle validation rules for a wiki. |
| `get_story_pattern` | Get story pattern name for a wiki or specific story. |
| `get_story_type_config` | Get configuration for a specific story type. |
| `get_story_type_requirements` | Get requirements for a story type with defaults. |
| `get_story_types` | Get story types configuration for an Epic. |
| `get_templates_dir` | Get Jinja templates directory. |
| `get_wiki_path` | Get path to Epic knowledge folder by name. |
| `get_wikis_dir` | Get wikis directory from settings. |
| `get_workspace_dir` | Get workspace directory from settings (optional). |
| `is_local_epic` | Check if Epic is local (no pull needed). |
| `is_local_repo` | Check if repo is local (no pull needed). |
| `load_ahabase_config` | Load ahabase.yaml configuration. |
| `load_secrets` | Load secrets from config/secrets.yml (git-ignored). |
| `load_settings` | Load settings from config file. |
| `load_state` | Load sync state with migration from wiki to epic terminol... |
| `save_state` | Save sync state. |
| `update_github_token` | Update GitHub PAT token for an organization. |

#### story-tracking

| Function | Description |
|----------|-------------|
| `_check_definition_for_prefix` | Check definition file in story_dir for matching StoryPrefix. |
| `get_active_story` | Get active story and epic. Returns (story, epic) or (None... |
| `get_epic_for_story` | Get epic name for a story ID using prefix mapping. |
| `get_story_pool` | Get story pool (MRU order). |
| `set_active_story` | Set active story and update pool (MRU order, max 5). |

#### unassigned

| Function | Description |
|----------|-------------|
| `get_configured_wikis` | Deprecated: Use get_configured_knowledge_paths instead. |
| `is_local_wiki` | Deprecated: Use is_local_epic instead. |

### counters

> Story ID counters on a git orphan branch.

**Blueprint:** [implementation-cli-counters-blueprint](implementation-cli-counters-blueprint)
**Tests:** -
**Functions:** 8 (8 with Capability)

#### git-operations

| Function | Description |
|----------|-------------|
| `_git` | Run a git command in the repo and return stripped stdout. |
| `_push_counters` | Commit counters.json via plumbing and push it by SHA. |
| `_read_remote_counters` | Fetch the counters branch and parse counters.json as {key... |
| `_remote_branch_exists` | True when origin carries the counters branch (raises when... |
| `allocate` | Claim the next number for a key on the counters branch. |
| `has_remote` | True when the repo has an origin remote configured. |

#### story-tracking

| Function | Description |
|----------|-------------|
| `allocate_story_id` | Return (story_id, strategy_used) for the next story. |
| `seed_from_stories` | Max story number across story/ and story/history/ (0 when... |

### db

> Database layer for DuckDB and Kuzu.

**Blueprint:** [implementation-cli-db-blueprint](implementation-cli-db-blueprint)
**Tests:** 6/6 (pass)
**Functions:** 12 (12 with Capability)

#### data-persistence

| Function | Description |
|----------|-------------|
| `__init__` | Initialize DuckDB and Kuzu connections. |
| `_init_schema` | Initialize database schemas. |
| `delete_stories` | Delete stories from both databases. |
| `ensure_schema` | Reset derived stores when on-disk schema is older than SC... |
| `get_kuzu_story_ids` | Get all story IDs from Kuzu. |
| `get_stored_doc_author` | Get last known author for a document. |
| `get_story_ids` | Get all story IDs from DuckDB. |
| `get_usage_epics` | Get epic names present in the databases. |
| `insert_many` | Insert stories into both databases. |
| `query_cypher` | Run Cypher query and return results as list of dicts. |
| `query_sql` | Run SQL query and return results as list of dicts. |
| `upsert_story_status` | Insert or update story status. |

### dbt_export

> DBT project export module.

**Blueprint:** [implementation-cli-dbt_export-blueprint](implementation-cli-dbt_export-blueprint)
**Tests:** -
**Functions:** 9 (9 with Capability)

#### config-management

| Function | Description |
|----------|-------------|
| `get_dbt_export_config` | Get dbt export configuration for an epic. |

#### dbt-export

| Function | Description |
|----------|-------------|
| `export_dbt` | Run dbt export for an epic. |
| `generate_dbt_index` | Generate DBT-Index.md overview. |
| `generate_mart_export` | Generate markdown export for a single mart model. |
| `get_model_layer` | Determine L2.1/L2.2 layer from model path. |
| `get_source_dependencies` | Get source dependencies for a model. |
| `get_upstream_chain` | Get upstream dependency chain for a model. |
| `parse_manifest` | Parse dbt manifest.json. |
| `run_dbt_setup` | Run dbt setup sequence. |

### discovery

> Filesystem-based discovery for Evolucean CLI.

**Blueprint:** [implementation-cli-discovery-blueprint](implementation-cli-discovery-blueprint)
**Tests:** -
**Functions:** 12 (0 with Capability)

#### unassigned

| Function | Description |
|----------|-------------|
| `_is_auxiliary` | Check if file is auxiliary (tests, knowledge-map, etc.). |
| `find_blueprint` | Find blueprint/implementation file. |
| `find_file` | Find file in any epic or subepic. |
| `find_issue` | Find issue file. |
| `find_ontology` | Find ontology file. |
| `find_pattern` | Find pattern file. |
| `find_story` | Find story file and extract epic/subepic info. |
| `find_story_in_epic` | Find story file within a specific epic using filesystem g... |
| `get_story_dir` | Get story directory relative to _grid4d for a story. |
| `get_workspace` | Get workspace root path. |
| `list_epics` | List all epics in workspace. |
| `list_subepics` | List all subepics for an epic. |

### git_utils

> Git utilities.

**Blueprint:** [implementation-cli-git_utils-blueprint](implementation-cli-git_utils-blueprint)
**Tests:** 5/5 (pass)
**Functions:** 12 (12 with Capability)

#### config-management

| Function | Description |
|----------|-------------|
| `update_settings_to_local` | Update settings.yml to change repository type from remote... |

#### git-operations

| Function | Description |
|----------|-------------|
| `_get_repo_root` | Get repo root from knowledge path. |
| `get_doc_author` | Get author email for a document. |
| `git_diff_status` | Get changed files since commit, including uncommitted ones. |
| `git_file_info` | Get git log info for a file. |
| `git_head` | Get current HEAD commit hash. |
| `git_pull` | Pull latest changes from remote. |
| `git_revert_to_author` | Revert file to last commit by target author. |
| `has_uncommitted` | Check for uncommitted changes matching pattern. |
| `init_git_repo` | Initialize git repository with .gitignore. |
| `is_git_repo` | Check if directory is a git repository. |
| `is_remote_accessible` | Check if remote repository is accessible via git ls-remote. |

### gradient

> Gradient measurement between blueprints and code.

**Blueprint:** [implementation-cli-gradient-blueprint](implementation-cli-gradient-blueprint)
**Tests:** -
**Functions:** 3 (3 with Capability)

#### gradient-check

| Function | Description |
|----------|-------------|
| `calculate_gradient` | Calculate gradient between blueprint and code for a module. |
| `generate_gradient_report` | Generate markdown gradient report. |
| `get_all_cli_modules` | Get list of all CLI modules with blueprints. |

### hooks

> Hook handlers for Claude Code integration.

**Blueprint:** [implementation-cli-hooks-blueprint](implementation-cli-hooks-blueprint)
**Tests:** 7/7 (pass)
**Functions:** 32 (32 with Capability)

#### git-operations

| Function | Description |
|----------|-------------|
| `_get_git_changes` | Get uncommitted changes from git status. |
| `_get_recent_commits` | Get recent commits related to story. |
| `get_wiki_git_status` | Check git status for wiki directory. |
| `needs_sync` | Check if sync needed after story completion. |

#### hook-handling

| Function | Description |
|----------|-------------|
| `_format_no_story_enforcement` | Format enforcement message when Edit/Write without active... |
| `audit_hook_registration` | Classify Claude Code hook events against the hooks module. |
| `handle_post_tool_use` | Handle PostToolUse hooks from Claude Code. |
| `handle_stop` | Game Master - show game status and guide next move. |

#### parsing

| Function | Description |
|----------|-------------|
| `_get_story_type_from_content` | Extract story type from content. |
| `_parse_test_results_per_requirement` | Parse test results grouped by requirement ID. |
| `parse_acceptance_criteria` | Parse Acceptance Criteria section from story content. |
| `parse_execution_table` | Parse Execution table from tests file. |
| `update_execution_table` | Update Execution table with new test results. |

#### pattern-driven

| Function | Description |
|----------|-------------|
| `get_story_behavior` | Get effective behavior config for a story. |

#### story-tracking

| Function | Description |
|----------|-------------|
| `_check_concept_coverage` | Check if concepts have ontology coverage using Trace. |
| `_find_story_file` | Find story file using filesystem-based discovery. |
| `_find_tracked_requirement` | Find requirement with **Tracked in:** link. |
| `_format_ac_status` | Format stop-handler output based on Acceptance Criteria. |
| `_format_checkpoint_status` | Fallback: format stop-handler output based on checkpoints. |
| `_format_idle_status` | Format stop-handler output when no story is active. |
| `_format_pattern_status` | Format stop-handler output based on pattern configuration. |
| `_format_requirements_status` | Format stop-handler output based on Requirements. |
| `_format_tracked_status` | Format stop-handler output with tracked requirement showi... |
| `_generate_story_context` | Generate story context file for LLM. |
| `_get_done_story_instructions` | Get git/sync instructions for DONE story if needed. |
| `_parse_phase_from_status` | Parse phase info from status file. |
| `_parse_requirements` | Parse Requirements (R1, R2, ...) from story content. |
| `get_active_story_info` | Get active story and pool info for display. |
| `pause_active_story` | Pause active story - keeps it in pool but stops tracking. |
| `resume_story_from_pool` | Resume a story from pool. |

#### test-execution

| Function | Description |
|----------|-------------|
| `handle_tests_file_auto` | Auto-run tests for -tests.md file if needed. |
| `needs_test_run` | Check if tests need to run based on Execution table. |

### issue_matcher

> Issue pattern matching for CLI.

**Blueprint:** [implementation-cli-issue_matcher-blueprint](implementation-cli-issue_matcher-blueprint)
**Tests:** 2/2 (pass)
**Functions:** 4 (4 with Capability)

#### issue-matching

| Function | Description |
|----------|-------------|
| `get_entropy_warnings` | Get entropy warnings for content. |
| `get_error_suggestion` | Get suggestion message for error. |
| `match_entropy_pattern` | Match content against known entropy patterns. |
| `match_error_pattern` | Match exit code and stderr against known error patterns. |

### karma

> Karma metrics computation.

**Blueprint:** [implementation-cli-karma-blueprint](implementation-cli-karma-blueprint)
**Tests:** 2/2 (pass)
**Functions:** 2 (2 with Capability)

#### story-tracking

| Function | Description |
|----------|-------------|
| `get_karma_per_author` | Get karma metrics per author. |
| `get_top_documents` | Get top documents by usage count. |

### karma_export

> Karma export module - generates Karma-Report.md.

**Blueprint:** [implementation-cli-karma_export-blueprint](implementation-cli-karma_export-blueprint)
**Tests:** -
**Functions:** 4 (4 with Capability)

#### export-generation

| Function | Description |
|----------|-------------|
| `_build_file_index` | Build index of all file names in ahabase namespace. |
| `_get_epic_name` | Extract Epic name from wiki/knowledge path. |
| `_is_valid_doc_name` | Check if document name is valid (exists in namespace). |
| `export_karma_report` | Export karma report to all Epics. |

### km_logger

> Knowledge-map logging - write entries directly to knowledge-map file.

**Blueprint:** [implementation-cli-km_logger-blueprint](implementation-cli-km_logger-blueprint)
**Tests:** 6/6 (pass)
**Functions:** 8 (8 with Capability)

#### config-management

| Function | Description |
|----------|-------------|
| `get_km_path` | Get path to knowledge-map file for a story. |

#### export-generation

| Function | Description |
|----------|-------------|
| `ensure_km_structure` | Ensure knowledge-map file exists with basic structure. |

#### knowledge-map-logging

| Function | Description |
|----------|-------------|
| `add_entry` | Add entry to knowledge-map. |
| `log_file_access` | Log file access to knowledge-map. |

#### parsing

| Function | Description |
|----------|-------------|
| `entry_exists` | Check if document already exists in knowledge-map. |
| `find_or_create_section` | Find or create section for action (flat structure). |
| `normalize_km` | Normalize knowledge-map formatting. |

#### pattern-lookup

| Function | Description |
|----------|-------------|
| `_find_pattern_template` | Find pattern template for a document type. |

### links

> Links module - on-demand markdown link extraction.

**Blueprint:** [implementation-cli-links-blueprint](implementation-cli-links-blueprint)
**Tests:** 2/2 (pass)
**Functions:** 3 (3 with Capability)

#### parsing

| Function | Description |
|----------|-------------|
| `extract_links` | Extract link targets from markdown content. |
| `get_all_links` | Get all outgoing links from wiki: {source: [targets]}. |
| `get_incoming_links` | Get all incoming links to wiki docs: {target: [sources]}. |

### llm_agent

> Agent layer model resolution for Claude Code.

**Blueprint:** [implementation-cli-llm_agent-blueprint](implementation-cli-llm_agent-blueprint)
**Tests:** -
**Functions:** 8 (8 with Capability)

#### llm-agent

| Function | Description |
|----------|-------------|
| `_proxy_routing` | Map proxy model_name entries to their provider endpoints. |
| `_resolve_bedrock_direct` | Resolve the Bedrock-direct agent path (no proxy involved). |
| `agent_indicator` | One-line indicator of the agent's real model. |
| `agent_models` | Distinct agent model names from a resolution, sorted. |
| `json_loads` | Parse JSON text, returning None on failure. |
| `resolve_agent_model` | Resolve the agent's model routing from environment and pr... |
| `resolve_inference_profile` | Resolve a Bedrock inference profile via AWS CLI (evidence... |
| `strip_profile_prefix` | Strip an AWS cross-region profile prefix to the foundatio... |

### llm_config

> Pattern-driven LLM configuration loader (EVOLUCEAN-0190).

**Blueprint:** [implementation-cli-llm_config-blueprint](implementation-cli-llm_config-blueprint)
**Tests:** -
**Functions:** 9 (9 with Capability)

#### llm-configuration

| Function | Description |
|----------|-------------|
| `config_layer` | Read the pattern's whole ``llm_config`` mapping. |
| `config_status` | Render where each hook LLM instruction comes from (patter... |
| `config_value` | Resolve one llm_config value: instance, pattern, typed de... |
| `hook_instruction` | Resolve one hook LLM instruction: pattern first, default ... |
| `hook_instructions_layer` | Read the pattern's ``hook_instructions`` mapping. |
| `instance_config_layer` | Read this instance's ``_config`` LLM mapping (empty when ... |
| `instance_config_path` | Locate the instance-level LLM config for this machine. |
| `parse_pattern_config` | Extract the llm_config YAML block from a pattern document. |
| `pattern_path` | Locate the LLM configuration pattern for an Epic. |

### llm_lmstudio

> LM Studio integration module.

**Blueprint:** [implementation-cli-llm_lmstudio-blueprint](implementation-cli-llm_lmstudio-blueprint)
**Tests:** 0/0 (not_run)
**Functions:** 16 (16 with Capability)

#### llm-lmstudio

| Function | Description |
|----------|-------------|
| `_find_llama_server` | Find path to llama-server binary. |
| `_install_lmstudio_linux` | Install LM Studio on Linux. |
| `_install_lmstudio_macos` | Install LM Studio on macOS. |
| `_install_lmstudio_windows` | Install LM Studio on Windows. |
| `check_lmstudio_installed` | Check if LM Studio is installed. |
| `create_daemon_scripts` | Create daemon scripts for LM Studio server. |
| `download_model` | Download model from HuggingFace to LM Studio models direc... |
| `from_dict` | Create LMStudioConfig from dict. |
| `get_alternative_models` | Return alternative models. |
| `get_default_model_config` | Return default model configuration. |
| `get_lmstudio_config` | Load LM Studio configuration from config/lmstudio.yml. |
| `get_project_root` | Get project root directory. |
| `install_lmstudio` | Install LM Studio by platform. |
| `list_available_models` | Return list of available models from config. |
| `start_daemon` | Start LM Studio daemon via launchctl. |
| `verify_setup` | Verify complete LM Studio setup. |

### llm_model_config

> Model configuration management for OpenRouter free models.

**Blueprint:** [implementation-cli-llm_model_config-blueprint](implementation-cli-llm_model_config-blueprint)
**Tests:** 0/0 (not_run)
**Functions:** 22 (22 with Capability)

#### llm-model-config

| Function | Description |
|----------|-------------|
| `__init__` | Load model configuration from YAML file. |
| `_categorize_model` | Categorize model based on name and description. |
| `_generate_config` | Generate fresh config from OpenRouter API. |
| `_generate_selection_criteria` | Generate selection criteria. |
| `_generate_task_mapping` | Generate task type mapping. |
| `_generate_yaml_from_models` | Generate YAML structure from OpenRouter models. |
| `_is_config_old` | Check if config file is older than max_age_days. |
| `_load_config` | Load and parse YAML configuration. |
| `_sort_by_scores` | Sort models by quality_score, then performance_score. |
| `_update_from_api` | Update configuration from OpenRouter API. |
| `filter_by_category` | Get models by category. |
| `filter_by_min_quality` | Get models with minimum quality score. |
| `filter_by_task_type` | Get models that support given task type. |
| `from_dict` | Create ModelInfo from dict. Capability: llm-model-config |
| `get_all_models` | Get all models as list. |
| `get_auto_selected_model` | Get auto-selected model ID for general use. |
| `get_model` | Get model info by key. |
| `get_model_config` | Get global model configuration instance. |
| `get_project_root` | Get project root directory. |
| `select_best_for_task_type` | Select best model for given task type. |
| `supports_task_type` | Check if model supports given task type. |
| `update_models` | Manually trigger model list update from OpenRouter API. |

### llm_openrouter

> OpenRouter backend for LLM module.

**Blueprint:** [implementation-cli-llm_openrouter-blueprint](implementation-cli-llm_openrouter-blueprint)
**Tests:** 0/0 (not_run)
**Functions:** 9 (9 with Capability)

#### llm-openrouter

| Function | Description |
|----------|-------------|
| `_defensive_update` | Defensive update: refresh model list and try again. |
| `_get_api_key` | Get OpenRouter API key from environment. |
| `_is_model_available` | Check if model exists in current available models. |
| `complete` | Complete a prompt using OpenRouter. |
| `discover_working_free_models` | Discover which free models are currently working. |
| `get_free_models` | Get list of free models from OpenRouter. |
| `get_recommended_config` | Get recommended LiteLLM config based on currently working... |
| `test_model` | Test if a specific model works. |
| `verify_api_key` | Verify OpenRouter API key and get detailed status. |

### llm_paths

> LLM access paths - switching between providers with preflight verification.

**Blueprint:** [implementation-cli-llm_paths-blueprint](implementation-cli-llm_paths-blueprint)
**Tests:** -
**Functions:** 11 (11 with Capability)

#### llm-paths

| Function | Description |
|----------|-------------|
| `_probe_suffixes` | Cheap probe endpoints: pattern override, code default sec... |
| `_settings_env` | Read the env section of the Claude Code settings (empty w... |
| `current_path` | Identify which access path the Claude Code env currently ... |
| `known_paths` | Return the built-in access path definitions. |
| `path_sensors` | Light reachability sensor per known path (no token cost). |
| `recover_service` | Revive the LiteLLM proxy offline (launchd restart + healt... |
| `recover_with_fallback` | Full safe-restart orchestration: fallback first, restart,... |
| `resolve_auth` | Resolve an auth spec ("env:NAME" or a literal token). |
| `switch_path` | Point Claude Code at an access path - only after a verifi... |
| `validate_proxy_config` | Validate the LiteLLM config offline (parse + model_list p... |
| `verify_path` | Preflight a path with a real minimal messages request. |

### llm_proxy

> LiteLLM Proxy for Claude Code integration.

**Blueprint:** [implementation-cli-llm_proxy-blueprint](implementation-cli-llm_proxy-blueprint)
**Tests:** 0/0 (not_run)
**Functions:** 19 (19 with Capability)

#### llm-proxy

| Function | Description |
|----------|-------------|
| `_asked_alias` | Read the alias the request carried from a success callbac... |
| `_fallback_depth` | Read the router's fallback depth from a success callback ... |
| `_format_from_health` | Fallback: format model status directly from /health endpo... |
| `check_litellm_installed` | Check if litellm is installed. |
| `check_openrouter_api_key` | Check if OpenRouter API key is set. |
| `ensure_config` | Ensure config file exists, generate if missing. |
| `format_model_status` | Format current model status for terminal display. |
| `generate_config` | Generate LiteLLM proxy configuration file. |
| `get_claude_code_config` | Get current Claude Code configuration. |
| `get_default_config` | Get default LiteLLM proxy configuration. |
| `get_last_used_model` | Get the last model used by LiteLLM proxy. |
| `get_proxy_health` | Get LiteLLM proxy health status. |
| `ingest_usage_history` | Ingest usage_history.jsonl into the DuckDB llm_usage table. |
| `is_proxy_running` | Check if proxy is running on given port. |
| `log_success_event` | LiteLLM success callback - records asked-versus-answered ... |
| `record_model_usage` | Record which model was actually used by LiteLLM proxy. |
| `restore_claude_code_config` | Restore Claude Code configuration from backup. |
| `set_claude_code_proxy_config` | Configure Claude Code to use LiteLLM proxy. |
| `start_proxy` | Start LiteLLM proxy server. |

### llm_selection

> Step model selection - mapping task types to step profiles (EVOLUCEAN-0180).

**Blueprint:** [implementation-cli-llm_selection-blueprint](implementation-cli-llm_selection-blueprint)
**Tests:** -
**Functions:** 5 (5 with Capability)

#### llm-selection

| Function | Description |
|----------|-------------|
| `format_proposal` | Render a selection proposal as terminal text. |
| `is_paid_model` | A model is treated as paid unless it carries an explicit ... |
| `resolve_step_profile` | Resolve a task type to its step profile. |
| `select_step_model` | Build a selection proposal for a task type. |
| `usage_evidence` | Per-model traffic counts from DuckDB llm_usage (real evid... |

### llm_service

> LiteLLM service management for Claude Code integration.

**Blueprint:** [implementation-cli-llm_service-blueprint](implementation-cli-llm_service-blueprint)
**Tests:** 0/0 (not_run)
**Functions:** 27 (27 with Capability)

#### llm-service

| Function | Description |
|----------|-------------|
| `check_claude_settings_conflict` | Check if Claude Code settings.json is configured for Lite... |
| `check_lmstudio` | Check if LM Studio is running and get loaded model info. |
| `check_lmstudio_daemon_installed` | Check if LM Studio daemon script is installed. |
| `check_openrouter_free_models_quick` | Quick check of OpenRouter free models status. |
| `create_launchd_service` | Create macOS launchd service. |
| `default` | Get default paths. |
| `detect_environment` | Detect current environment type. |
| `ensure_directories` | Create required directories. |
| `generate_config` | Generate LiteLLM config from template. |
| `get_lmstudio_daemon_logs` | Get LM Studio daemon logs. |
| `get_lmstudio_daemon_script` | Get path to LM Studio daemon script. |
| `get_lmstudio_daemon_status` | Get LM Studio daemon status from launchd and script. |
| `get_lmstudio_models` | Get list of available models from LM Studio. |
| `get_logs` | Get recent log content. |
| `get_service_status` | Get current LiteLLM service status. |
| `install_litellm` | Install LiteLLM in venv using uv. |
| `lmstudio_daemon_restart` | Restart LM Studio daemon using lm-server-daemon.sh. |
| `lmstudio_daemon_start` | Start LM Studio daemon using lm-server-daemon.sh. |
| `lmstudio_daemon_stop` | Stop LM Studio daemon using lm-server-daemon.sh. |
| `lmstudio_watchdog_check` | LM Studio watchdog check and optional auto-restart. |
| `load_service` | Load launchd service. |
| `run_doctor` | Run diagnostic checks. |
| `test_lmstudio_completion` | Test LM Studio completion endpoint. |
| `uninstall_service` | Uninstall LiteLLM service completely. |
| `unload_service` | Unload launchd service. |
| `update_config_with_free_models` | Update config.yaml with currently working free models. |
| `validate_prerequisites` | Validate prerequisites for given environment. |

### llm_telemetry

> Agent telemetry sensor - local OTLP collector (EVOLUCEAN-0200).

**Blueprint:** [implementation-cli-llm_telemetry-blueprint](implementation-cli-llm_telemetry-blueprint)
**Tests:** -
**Functions:** 22 (18 with Capability)

#### llm-telemetry

| Function | Description |
|----------|-------------|
| `_attr_value` | Extract a python value from one OTLP AnyValue mapping. |
| `_decode_attributes` | Decode an OTLP attribute list into a plain dict. |
| `_load_settings` | Read the Claude Code settings file (empty dict when absen... |
| `_log_collector_line` | Append one diagnostics line to the collector log. |
| `_record_event_name` | Resolve the event name of one OTLP log record. |
| `_record_timestamp` | Derive seconds-since-epoch from an OTLP log record. |
| `_usage_history_path` | The shared evidence file (lazy import keeps the proxy mod... |
| `append_agent_telemetry` | Append agent api_request events as asked-model usage reco... |
| `collector_stats` | Return the last collector log line (empty when none). |
| `handle_otlp_logs` | Process one OTLP logs payload end to end. |
| `install_telemetry_env` | Merge the telemetry env block into Claude Code settings. |
| `is_collector_running` | Check whether something answers on the collector port. |
| `main` | Foreground entry point for the background collector process. |
| `parse_api_requests` | Extract agent api_request events from one OTLP logs payload. |
| `run_collector` | Run the collector HTTP server in the foreground. |
| `show_telemetry_env` | Report the current five-var state against Claude settings. |
| `start_collector` | Start the collector as a background process. |
| `stop_collector` | Stop any process listening on the collector port. |

#### unassigned

| Function | Description |
|----------|-------------|
| `_respond` | - |
| `do_GET` | - |
| `do_POST` | - |
| `log_message` | - |

### ontology

> Ontology validation for new ontology structure.

**Blueprint:** [implementation-cli-ontology-blueprint](implementation-cli-ontology-blueprint)
**Tests:** 2/2 (pass)
**Functions:** 5 (5 with Capability)

#### document-validation

| Function | Description |
|----------|-------------|
| `check_index_completeness` | Check that index Vocabulary matches actual files. |
| `check_required_sections` | Check that each ontology blueprint has required sections. |
| `validate_ontology` | Run all ontology validation checks. |

#### parsing

| Function | Description |
|----------|-------------|
| `extract_vocabulary_links` | Extract document names from Vocabulary section. |
| `get_ontology_files` | Get all ontology blueprint files (without .md extension). |

### parser

> Knowledge map parser.

**Blueprint:** [implementation-cli-parser-blueprint](implementation-cli-parser-blueprint)
**Tests:** 0/0 (not_run)
**Functions:** 14 (14 with Capability)

#### data-persistence

| Function | Description |
|----------|-------------|
| `parse_and_save_json` | Parse MD to dict and save as JSON. |

#### document-validation

| Function | Description |
|----------|-------------|
| `_validate_doc_exists` | Check if referenced document exists. |
| `_validate_one_doc_one_place` | Validate that each document appears in exactly one Action. |

#### export-generation

| Function | Description |
|----------|-------------|
| `clear_json_dir` | Clear all JSON files for full reload. |
| `delete_json` | Delete JSON file for a story. |

#### parsing

| Function | Description |
|----------|-------------|
| `_check_deploy_to_test` | Check if story status page has Deploy to Test merged. |
| `_check_tests_pass` | Check if story has tests and all pass. |
| `clear_validation_errors` | Clear validation errors. |
| `extract_doc_reference` | Extract document reference and role from markdown link line. |
| `extract_story_id` | Extract story ID from filename. |
| `get_epic_and_subepic` | Extract (epic, subepic) ownership from a path inside a kn... |
| `get_validation_errors` | Get collected validation errors. |
| `parse_knowledge_sections` | Extract Scope/Action/Documents hierarchy from MD content. |
| `parse_story_success` | Parse story success status based on configured check type. |

### pattern_inference

> Pattern inference engine for extracting validation rules from templates.

**Blueprint:** [implementation-cli-pattern_inference-blueprint](implementation-cli-pattern_inference-blueprint)
**Tests:** -
**Functions:** 5 (5 with Capability)

#### pattern-inference

| Function | Description |
|----------|-------------|
| `_deep_merge` | Deep merge two dicts, override wins on conflicts. |
| `_parse_behavior` | Parse _behavior section as YAML. |
| `extract_rules` | Extract validation rules from pattern template + _behavio... |
| `get_behavior_config` | Get effective behavior config from pattern and optional d... |
| `validate_document` | Validate document against rules. |

### pattern_resolver

> Pattern lineage lookup following taxonomic hierarchy.

**Blueprint:** [implementation-cli-pattern_resolver-blueprint](implementation-cli-pattern_resolver-blueprint)
**Tests:** -
**Functions:** 6 (6 with Capability)

#### pattern-resolver

| Function | Description |
|----------|-------------|
| `_convert_value` | Convert string value to appropriate type. |
| `_parse_epic_definition` | Parse epic/subepic definition markdown to dict. |
| `get_context` | Detect epic/subepic from path. |
| `list_patterns` | List all available patterns for a context. |
| `lookup` | Find pattern following lineage (first found wins). |
| `lookup_epic_config` | Load effective epic/subepic config following inheritance. |

### patterns

> Pattern loading and parsing for Story and Workflow Loop.

**Blueprint:** [implementation-cli-patterns-blueprint](implementation-cli-patterns-blueprint)
**Tests:** 0/0 (not_run)
**Functions:** 7 (7 with Capability)

#### parsing

| Function | Description |
|----------|-------------|
| `parse_pattern` | Parse pattern markdown into structured data. |

#### pattern-management

| Function | Description |
|----------|-------------|
| `check_exit_condition` | Check if phase exit condition is met. |
| `determine_phase_state` | Determine current state of a phase. |
| `format_phase_status` | Format current phase status for display. |
| `get_current_phase` | Determine current active phase based on story state. |
| `get_pattern_path` | Find pattern file using filesystem-based discovery. |
| `load_pattern` | Load and parse pattern blueprint. |

### projections_base

> Base class for projections using Template Method pattern.

**Blueprint:** [implementation-cli-projections_base-blueprint](implementation-cli-projections_base-blueprint)
**Tests:** -
**Functions:** 11 (11 with Capability)

#### config-management

| Function | Description |
|----------|-------------|
| `grid4d_path` | Path to _grid4d folder (or subepic root for subepics). |
| `has_ontology` | Check if Epic has own ontology folder. |
| `implementation_path` | Path to implementation folder. |
| `ontology_path` | Path to ontology folder. |
| `story_path` | Path to story folder. |

#### projection-generation

| Function | Description |
|----------|-------------|
| `extract` | Extract raw data from Epic. Override in subclass. |
| `generate` | Template Method - orchestrates projection generation. |
| `get_timestamp` | Get current timestamp for generated header. |
| `render` | Render data to markdown. Override in subclass. |
| `transform` | Transform extracted data. Override if needed. |
| `write` | Write content to output file. |

### projections_epic_artifacts

> Artifacts projection - generates EPIC-Artifacts.md (CLI metrics).

**Blueprint:** [implementation-cli-projections_epic_artifacts-blueprint](implementation-cli-projections_epic_artifacts-blueprint)
**Tests:** -
**Functions:** 7 (7 with Capability)

#### projection-generation

| Function | Description |
|----------|-------------|
| `_escape_markdown_links` | Escape markdown links in description text. |
| `_extract_module_docstring` | Extract module-level docstring. |
| `_parse_test_results` | Parse test results from -tests.md file. |
| `_render_test_coverage` | Per-module regression-tree evidence from the Module_TestC... |
| `extract` | Extract CLI artifact metrics. |
| `render` | Render artifacts to markdown. |
| `transform` | Calculate summary metrics. |

### projections_epic_capabilities

> Capabilities projection - generates EPIC-Capabilities.md.

**Blueprint:** [implementation-cli-projections_epic_capabilities-blueprint](implementation-cli-projections_epic_capabilities-blueprint)
**Tests:** -
**Functions:** 8 (8 with Capability)

#### projection-generation

| Function | Description |
|----------|-------------|
| `_collect_blueprint_files` | Module names that have a conventional blueprint file. |
| `_read_index` | Capability names defined in the ontology index. |
| `_read_tests` | Read standalone test scripts once for mention checks. |
| `_scan_modules` | Scan every python module for capability and blueprint |
| `extract` | Extract capability evidence from code, ontology and tests. |
| `render` | Render the capability coverage report. |
| `resolve_blueprint` | Resolve the blueprint covering one module, or None. |
| `transform` | Build one row per capability and the summary. |

### projections_epic_complexity

> Epic complexity projection - EPIC-Complexity.md for the Epic.

**Blueprint:** [implementation-cli-projections_epic_complexity-blueprint](implementation-cli-projections_epic_complexity-blueprint)
**Tests:** -
**Functions:** 10 (10 with Capability)

#### projection-generation

| Function | Description |
|----------|-------------|
| `ast_entropy` | Shannon entropy of the AST node-type distribution (EVOLUC... |
| `cyclomatic_complexity` | Cyclomatic complexity per the formula in the gradient met... |
| `detect_symptoms` | Map metric values to manual symptoms; each report names v... |
| `extract` | Measure the Epic's knowledge-usage-cli modules. |
| `find_manual` | Locate the refactoring manual in the Epic's implementatio... |
| `module_metrics` | Complexity metrics of one Python module (ast only). |
| `param_count` | Total parameter count including vararg/kwarg. |
| `parse_manual` | Parse the "When to Refactor" table: symptom -> (first try... |
| `render` | Render Summary, Thresholds, Modules and Findings sections. |
| `transform` | Totals, per-symptom counts and baseline distribution stats. |

### projections_epic_concepts

> Concepts projection - generates EPIC-Concepts.md.

**Blueprint:** [implementation-cli-projections_epic_concepts-blueprint](implementation-cli-projections_epic_concepts-blueprint)
**Tests:** -
**Functions:** 8 (8 with Capability)

#### projection-generation

| Function | Description |
|----------|-------------|
| `_module_exists` | Does the module behind a conventional blueprint name exist? |
| `_parse_concept` | Parse one ontological concept blueprint. |
| `_scan_code_grounding` | Blueprint stems a code module links to. |
| `_scan_implementations` | Scan implementation blueprints for Implements declarations. |
| `_strip_concept_name` | Strip the ontology- prefix / -blueprint suffix EXACTLY once. |
| `extract` | Extract concepts and the reference chain from the Epic. |
| `render` | Render the concepts report. |
| `transform` | Join the reference chain onto the concepts. |

### projections_epic_design_patterns

> Epic design patterns projection - EPIC-Design-Patterns.md for the Epic.

**Blueprint:** [implementation-cli-projections_epic_design_patterns-blueprint](implementation-cli-projections_epic_design_patterns-blueprint)
**Tests:** -
**Functions:** 10 (10 with Capability)

#### projection-generation

| Function | Description |
|----------|-------------|
| `_header` | H1 title and first blockquote line of a document. |
| `_render_applied` | Patterns applied in CLI code with their evidence files. |
| `_render_referenced` | Patterns referenced from implementation knowledge via wik... |
| `_render_unapplied` | Gap list per family - input for Sustain-mode refactoring. |
| `extract` | Scan the Epic's design concepts, code declarations, knowl... |
| `parse_declarations` | ``- Name (Family): ...`` declarations from a ``Design pat... |
| `parse_design_pattern` | Parse a design pattern concept; None when it carries no C... |
| `parse_pattern_links` | Design pattern concept stems targeted by wiki links in a ... |
| `render` | Render design pattern usage overview to markdown. |
| `transform` | Match declarations and knowledge links to concepts, compu... |

### projections_epic_gradients

> Gradients projection - generates EPIC-Gradients.md.

**Blueprint:** [implementation-cli-projections_epic_gradients-blueprint](implementation-cli-projections_epic_gradients-blueprint)
**Tests:** -
**Functions:** 11 (3 with Capability)

#### projection-generation

| Function | Description |
|----------|-------------|
| `extract` | Measure all implemented sensors for the Epic. |
| `render` | Render gradients to markdown. |
| `transform` | Aggregate readings into one value per metric column. |

#### unassigned

| Function | Description |
|----------|-------------|
| `__init__` | - |
| `_aggregate` | Aggregate sensor readings into one catalog row value. |
| `_aggregate_bpfunc` | Sum module counts into the epic-level code traceability r... |
| `_aggregate_codeent` | Clean-share of per-module Code Entropy readings (CodeEnt). |
| `_aggregate_fresh` | Fresh-share of per-document freshness readings (KnowUseFr... |
| `_aggregate_karma` | Sum per-document counts into the epic-level karma. |
| `_aggregate_modtestcov` | Tested-share of per-module Test Coverage readings (ModTes... |
| `_aggregate_testcov` | Tested-share of per-concept test coverage readings (TestC... |

### projections_epic_graph

> Graph projection - generates EPIC-Graph.md using Kuzu queries.

**Blueprint:** [implementation-cli-projections_epic_graph-blueprint](implementation-cli-projections_epic_graph-blueprint)
**Tests:** -
**Functions:** 6 (5 with Capability)

#### projection-generation

| Function | Description |
|----------|-------------|
| `_build_file_index` | Build index of all file names in ahabase namespace. |
| `_is_valid_doc_name` | Check if document name is valid (exists in namespace). |
| `extract` | Extract graph metrics from Kuzu database. |
| `render` | Render graph data to markdown. |
| `transform` | Filter out invalid document references. |

#### unassigned

| Function | Description |
|----------|-------------|
| `__init__` | - |

### projections_epic_issues

> Issues projection - generates EPIC-Issues.md.

**Blueprint:** [implementation-cli-projections_epic_issues-blueprint](implementation-cli-projections_epic_issues-blueprint)
**Tests:** -
**Functions:** 3 (3 with Capability)

#### projection-generation

| Function | Description |
|----------|-------------|
| `extract` | Scan the epic's issue documents. |
| `render` | Render the issues report. |
| `transform` | Derive open/recurring counts; sort recurring issues first. |

### projections_epic_llm_status

> LLM status projection - generates EPIC-Llm-Status.md.

**Blueprint:** [implementation-cli-projections_epic_llm_status-blueprint](implementation-cli-projections_epic_llm_status-blueprint)
**Tests:** -
**Functions:** 8 (8 with Capability)

#### projection-generation

| Function | Description |
|----------|-------------|
| `_agent_usage` | Read the most recent agent-telemetry completions. |
| `_endpoint_models` | Extract model names from health endpoint entries. |
| `_human_age` | Format an age in seconds for display. |
| `_recent_usage` | Read the most recent usage events from the append-only JS... |
| `_recovery_rows` | Symptom → first-action rows: pattern override, default se... |
| `extract` | Extract live LLM state for the instance hosting this Epic. |
| `render` | Render the markdown document. |
| `transform` | Derive display rows from raw state. |

### projections_epic_orphans

> Orphans projection - generates EPIC-Orphans.md.

**Blueprint:** [implementation-cli-projections_epic_orphans-blueprint](implementation-cli-projections_epic_orphans-blueprint)
**Tests:** -
**Functions:** 13 (13 with Capability)

#### projection-generation

| Function | Description |
|----------|-------------|
| `_calc_coverage` | Calculate blueprint coverage percentage. |
| `_collect_blueprints` | Collect implementation blueprints. |
| `_collect_code_modules` | Collect Python code modules. |
| `_collect_tests` | Collect implementation tests. |
| `_extract_module_from_blueprint` | Extract module name from blueprint filename. |
| `_extract_module_from_tests` | Extract module name from tests filename. |
| `_find_missing_blueprints` | Find code modules without corresponding blueprint. |
| `_find_orphan_blueprints` | Find blueprints without corresponding code. |
| `_find_orphan_tests` | Find tests without corresponding blueprint. |
| `_module_to_code_path` | Convert module name to expected code path. |
| `extract` | Extract orphan information from Epic. |
| `render` | Render orphans report to markdown. |
| `transform` | Calculate summary metrics. |

### projections_epic_patterns

> Patterns projection - generates EPIC-Patterns.md.

**Blueprint:** [implementation-cli-projections_epic_patterns-blueprint](implementation-cli-projections_epic_patterns-blueprint)
**Tests:** -
**Functions:** 4 (4 with Capability)

#### projection-generation

| Function | Description |
|----------|-------------|
| `_parse_pattern` | Parse pattern file metadata. |
| `extract` | Extract patterns from Epic. |
| `render` | Render patterns to markdown. |
| `transform` | Calculate summary. |

### projections_epic_pool_views

> Pool views projection - per-entry views for issues, ideas and metrics.

**Blueprint:** Missing
**Tests:** -
**Functions:** 15 (4 with Capability)

#### projection-generation

| Function | Description |
|----------|-------------|
| `_entries` | (stem, source text) per pool entry. |
| `extract` | Current view context. |
| `generate` | Render one view per entry for each pool. |
| `render` | Render the current view, sections in the pool's pattern o... |

#### unassigned

| Function | Description |
|----------|-------------|
| `__init__` | - |
| `_generate_pool` | - |
| `_issue_row` | - |
| `_load_readings` | - |
| `_pool_activity` | - |
| `_pool_attributes` | - |
| `_pool_links` | - |
| `_pool_occurrences` | - |
| `_pool_overview` | - |
| `_pool_reading` | - |
| `_read` | - |

### projections_epic_shaping

> Shaping projection - generates EPIC-Shaping.md.

**Blueprint:** [implementation-cli-projections_epic_shaping-blueprint](implementation-cli-projections_epic_shaping-blueprint)
**Tests:** -
**Functions:** 7 (7 with Capability)

#### projection-generation

| Function | Description |
|----------|-------------|
| `_analyze_blueprint_traceability` | Analyze which blueprints link to ontology. |
| `_analyze_ontology_coverage` | Analyze which ontology concepts have implementation bluep... |
| `_collect_implementation_blueprints` | Collect implementation blueprints. |
| `_collect_ontology_concepts` | Collect ontology concept blueprints. |
| `extract` | Extract shaping metrics from Epic. |
| `render` | Render shaping report to markdown. |
| `transform` | Calculate summary metrics. |

### projections_epic_stories

> Stories projection - generates EPIC-Stories.md.

**Blueprint:** [implementation-cli-projections_epic_stories-blueprint](implementation-cli-projections_epic_stories-blueprint)
**Tests:** -
**Functions:** 5 (5 with Capability)

#### projection-generation

| Function | Description |
|----------|-------------|
| `_parse_story` | Parse story file to extract metadata. |
| `_parse_test_status` | Parse test results from -tests.md file. |
| `extract` | Extract stories from Epic (story/ + story/history/). |
| `render` | Render stories to markdown. |
| `transform` | Sort stories by number, newest first. |

### projections_epic_story_views

> Story views projection - one big-picture document per completed story.

**Blueprint:** Missing
**Tests:** -
**Functions:** 14 (4 with Capability)

#### projection-generation

| Function | Description |
|----------|-------------|
| `_completed_stories` | Story documents whose status marks completion, story/ first. |
| `extract` | Current view context and pattern sections. |
| `generate` | Render a view for every completed story. |
| `render` | Render the current view, sections in pattern order. |

#### unassigned

| Function | Description |
|----------|-------------|
| `__init__` | - |
| `_load_readings` | - |
| `_read` | - |
| `_sec_activity` | - |
| `_sec_knowledge` | - |
| `_sec_measured` | - |
| `_sec_outcome` | - |
| `_sec_overview` | - |
| `_sec_related` | - |
| `_sec_tests` | - |

### projections_epic_subepics

> SubEpics projection - generates EPIC-SubEpics.md.

**Blueprint:** [implementation-cli-projections_epic_subepics-blueprint](implementation-cli-projections_epic_subepics-blueprint)
**Tests:** -
**Functions:** 3 (3 with Capability)

#### projection-generation

| Function | Description |
|----------|-------------|
| `_parse_subepic` | Parse SubEpic directory to extract metadata. |
| `extract` | Extract SubEpics from Epic. |
| `render` | Render SubEpics to markdown. |

### projections_epic_trace

> Area trace projection - end-to-end coverage of one knowledge area.

**Blueprint:** [implementation-cli-projections_epic_trace-blueprint](implementation-cli-projections_epic_trace-blueprint)
**Tests:** -
**Functions:** 21 (4 with Capability)

#### projection-generation

| Function | Description |
|----------|-------------|
| `extract` | Locate area artifacts per layer. |
| `generate` | Set the area stem, then run the template method. |
| `render` | Render the coverage report. |
| `transform` | Assign per-layer status per the blueprint status rules. |

#### unassigned

| Function | Description |
|----------|-------------|
| `__init__` | - |
| `_implementation_roots` | - |
| `_issue_roots` | Epic issue folder plus subepic issue folders. |
| `_md_link` | Render a knowledge file as a wiki link, else inline code. |
| `_mentions` | - |
| `_ontology_roots` | Epic ontology plus subepic ontologies (subepics inherit t... |
| `_pattern_roots` | Epic pattern folder plus subepic pattern folders. |
| `_python_files` | - |
| `_stem_re` | Word-boundary pattern for the area stem. |
| `find_code_and_projections` | CLI modules (docstring/capability) and projection sources... |
| `find_data` | DuckDB tables, Kuzu labels and Document node names matchi... |
| `find_implementation` | Implementation docs by filename or content mention. |
| `find_infrastructure` | Infrastructure blueprints of the area (external-interface... |
| `find_issue` | Issue docs by filename or content mention. |
| `find_ontology` | Ontology blueprints matching the stem by naming convention. |
| `find_pattern` | Pattern templates by filename or content mention. |
| `find_tests` | Test files referencing area code modules or the stem. |

### projections_epic_usage

> Usage projection - generates EPIC-Usage.md (Prune evidence).

**Blueprint:** [implementation-cli-projections_epic_usage-blueprint](implementation-cli-projections_epic_usage-blueprint)
**Tests:** -
**Functions:** 5 (3 with Capability)

#### projection-generation

| Function | Description |
|----------|-------------|
| `extract` | Measure all sensors; keep the knowledge-document ones. |
| `render` | Render the usage report. |
| `transform` | Join sensor readings by document stem and derive signals. |

#### unassigned

| Function | Description |
|----------|-------------|
| `__init__` | - |
| `signal_of` | Signal from a KnowUseFresh reading (unused/stale/aging/fr... |

### projections_epic_viewlib

> Shared helpers for the big-picture view projections.

**Blueprint:** Missing
**Tests:** -
**Functions:** 5 (5 with Capability)

#### projection-generation

| Function | Description |
|----------|-------------|
| `git_activity_map` | Single-pass git log -> story and file activity. |
| `list_rows` | Non-empty rows of a section body, verbatim. |
| `load_pattern_sections` | Behavior mapping declared in ``pattern/<name>.md`` `## _b... |
| `parse_fields` | ``**Field:** value`` lines from a document header, in order. |
| `section_text` | Body of a ``## <heading>`` section, up to the next heading. |

### projections_fragments

> Generated marker sections inside definition documents.

**Blueprint:** [implementation-cli-projections_fragments-blueprint](implementation-cli-projections_fragments-blueprint)
**Tests:** -
**Functions:** 3 (3 with Capability)

#### projection-generation

| Function | Description |
|----------|-------------|
| `definition_document_path` | Path to the definition document of an Epic or SubEpic. |
| `update_definition_fragment` | Replace content between generated markers in a document. |
| `update_projections_fragment` | Update the ``projections`` fragment of an Epic's definiti... |

### projections_namespace_base

> Instance-level projection base - writes to <instance root>/_generated/.

**Blueprint:** [implementation-cli-projections_namespace_base-blueprint](implementation-cli-projections_namespace_base-blueprint)
**Tests:** -
**Functions:** 3 (3 with Capability)

#### projection-generation

| Function | Description |
|----------|-------------|
| `generate` | Template method; epic is unused for instance scope. |
| `instance_epic_dirs` | Epic dirs in the instance root (non-underscore, has _grid... |
| `write` | Write to <instance root>/_generated/{output_file}. |

### projections_namespace_instance

> Namespace projection - generates AHABASE-Instance.md for the whole instance.

**Blueprint:** [implementation-cli-projections_namespace_instance-blueprint](implementation-cli-projections_namespace_instance-blueprint)
**Tests:** -
**Functions:** 26 (25 with Capability)

#### projection-generation

| Function | Description |
|----------|-------------|
| `_conn` | Lazy Database() - one open per run, not per Epic. |
| `_cross_epic_usage` | Stories consuming documents owned by another Epic. |
| `_display_remote` | host/owner/repo with userinfo (credentials) stripped - to... |
| `_document_counts` | Document ownership from Kuzu Document nodes. |
| `_fmt` | Format a cell value: None/NaN/empty become '-'. |
| `_git_state` | Remote URL + branch via git; liveness per credential stra... |
| `_identity` | Epic identity doc (case-insensitive <epic>.md in story/) ... |
| `_is_git_repo` | Check if directory is a git repository. |
| `_open_issues` | Issue file stems carrying '**Status:** open'. |
| `_remote_is_live` | True when the remote resolves as live per the instance cr... |
| `_render_cross_epic` | Cross-epic knowledge usage view. |
| `_render_documents` | Document ownership pivot from DB. |
| `_render_epics` | Active Epics table (all three membership conditions hold). |
| `_render_incomplete` | Incomplete Epics table (on disk, failing the Active Epic ... |
| `_render_inventory` | Knowledge inventory per Epic (filesystem counts). |
| `_render_open_issues` | Open issues per Epic (filesystem). |
| `_render_stories` | Story ownership from DB. |
| `_render_structure_audit` | Structure Audit section - git repos and their structural ... |
| `_render_summary` | Instance summary. |
| `_scan_epic` | Folder counts + subepic rows + open issues + git/identity... |
| `_scan_structure_audit` | Scan all directories in instance root for structure compl... |
| `_story_status` | Story ownership from DuckDB story_status (schema v2). |
| `extract` | Extract instance data: disk scan with git/identity state,... |
| `render` | Render instance data to markdown. |
| `transform` | Evaluate the Active Epic test per cloned Epic, pivot docu... |

#### unassigned

| Function | Description |
|----------|-------------|
| `__init__` | - |

### projections_namespace_issues

> Namespace issues projection - generates AHABASE-Issues.md for the whole instance.

**Blueprint:** [implementation-cli-projections_namespace_issues-blueprint](implementation-cli-projections_namespace_issues-blueprint)
**Tests:** -
**Functions:** 10 (10 with Capability)

#### projection-generation

| Function | Description |
|----------|-------------|
| `_first_paragraph` | First non-empty paragraph below a section heading. |
| `_occurrence_rows` | Data rows of the Occurrences table as (date, symptom) tup... |
| `_render_lessons` | Resolved issues - the lessons-learned ledger. |
| `_render_open` | Open issues with their problem statements. |
| `_render_recurring` | Recurring issues - candidates for systematic solutions. |
| `_section` | Content between the first matching ``## <name>`` heading ... |
| `extract` | Scan issue documents across all cloned Epics. |
| `parse_issue` | Parse one issue document into a row; None when it carries... |
| `render` | Render issues overview to markdown. |
| `transform` | Order rows (recurring first), compute summary counts. |

### projections_namespace_patterns

> Namespace patterns projection - generates AHABASE-Patterns.md for the whole instance.

**Blueprint:** [implementation-cli-projections_namespace_patterns-blueprint](implementation-cli-projections_namespace_patterns-blueprint)
**Tests:** -
**Functions:** 4 (4 with Capability)

#### projection-generation

| Function | Description |
|----------|-------------|
| `extract` | Scan pattern template folders across cloned Epics. |
| `parse_template` | Parse a document template from a ``pattern/`` folder. |
| `render` | Render document template overview to markdown. |
| `transform` | Count templates per Epic. |

### projections_registry

> Registry for projection plugins.

**Blueprint:** [implementation-cli-projections_registry-blueprint](implementation-cli-projections_registry-blueprint)
**Tests:** -
**Functions:** 7 (7 with Capability)

#### config-management

| Function | Description |
|----------|-------------|
| `clear` | Clear all registered projections. For testing. |
| `create` | Create projection instance by name. |
| `list` | List registered projection names. |
| `names_for_scope` | Names of registered projections with the given scope. |
| `register` | Register a projection class. |

#### projection-generation

| Function | Description |
|----------|-------------|
| `generate_all` | Generate all projections for an Epic. |
| `generate_scope` | Generate each projection of a scope ONCE for the whole in... |

### projections_utility_inheritance

> Inheritance projection - generates EPIC-Inheritance.md.

**Blueprint:** [implementation-cli-projections_utility_inheritance-blueprint](implementation-cli-projections_utility_inheritance-blueprint)
**Tests:** -
**Functions:** 7 (7 with Capability)

#### projection-generation

| Function | Description |
|----------|-------------|
| `_build_node` | Build tree node with children. |
| `_build_tree` | Build inheritance tree structure. |
| `_find_epic_definition` | Find and parse Epic definition file. |
| `_parse_definition` | Parse Epic definition file. |
| `_render_node` | Render tree node recursively. |
| `extract` | Extract inheritance hierarchy. |
| `render` | Render inheritance tree to markdown. |

### projections_utility_validation

> Validation projection - generates Validation-Report.md.

**Blueprint:** [implementation-cli-projections_utility_validation-blueprint](implementation-cli-projections_utility_validation-blueprint)
**Tests:** -
**Functions:** 10 (9 with Capability)

#### projection-generation

| Function | Description |
|----------|-------------|
| `_build_file_index` | Build index of all files in ahabase namespace. |
| `_check_file` | Check single file for issues. |
| `_check_pattern_prefix` | Check if pattern file has correct epic/subepic prefix. |
| `_extract_filename` | Extract filename from link target. |
| `_get_scan_root` | Get the root path to scan for this epic/subepic. |
| `_should_include_file` | Check if file should be included in validation. |
| `_validate_link` | Validate a link against the file index. |
| `extract` | Extract validation issues from Epic. |
| `render` | Render validation report to markdown. |

#### unassigned

| Function | Description |
|----------|-------------|
| `__init__` | - |

### rule_extractor

> Extract validation rules from type-blueprints.

**Blueprint:** [implementation-cli-rule_extractor-blueprint](implementation-cli-rule_extractor-blueprint)
**Tests:** 4/4 (pass)
**Functions:** 8 (8 with Capability)

#### config-management

| Function | Description |
|----------|-------------|
| `get_type_blueprints` | Get type-blueprint mapping from knowledge-naming-blueprint. |

#### export-generation

| Function | Description |
|----------|-------------|
| `extract_all_rules` | Extract rules from all type-blueprints. |
| `generate_document_rules_yaml` | Generate YAML content for document-rules.yml. |
| `save_document_rules` | Save rules to config/document-rules.yml. |

#### parsing

| Function | Description |
|----------|-------------|
| `extract_rules_from_blueprint` | Extract validation rules from a single type-blueprint. |
| `find_sections_markdown_aware` | Find ## headings, ignoring those inside fenced code blocks. |
| `parse_structure_table` | Parse Structure table from blueprint content. |
| `parse_validation_checks` | Parse ## Validation section yaml block. |

### scope_role

> Scope and Role determination for knowledge-map entries.

**Blueprint:** [implementation-cli-scope_role-blueprint](implementation-cli-scope_role-blueprint)
**Tests:** 2/2 (pass)
**Functions:** 3 (3 with Capability)

#### parsing

| Function | Description |
|----------|-------------|
| `determine_action` | Determine action from tool name. |
| `determine_role` | Determine role from document suffix or path. |
| `determine_scope` | Determine scope for a file access. |

### sensors

> Internal Sensor layer: registry, measurement, persistence.

**Blueprint:** [implementation-cli-sensors-blueprint](implementation-cli-sensors-blueprint)
**Tests:** -
**Functions:** 33 (29 with Capability)

#### sensor-read

| Function | Description |
|----------|-------------|
| `_cli_source_modules` | CLI code modules: subject name -> file under the package ... |
| `_measure_execution_table` | Parse a story's tests.md execution table into one reading. |
| `_shaping_coverage` | Shared source computation for the Shaping metrics (OntCov... |
| `_suite_import_subjects` | Module subjects imported by the regression tree. |
| `get` | Get a sensor definition by id. |
| `knowledge_documents` | Active knowledge files: *.md under grid4d, underscore par... |
| `list` | List registered sensor definitions (sorted by id). |
| `load_readings` | Load persisted readings ordered by sensor, epic, subject. |
| `measure_all` | Measure every implemented sensor; skip declared-only ones. |
| `measure_and_store` | Measure all sensors for the epic and persist the readings. |
| `measure_bpcov` | Blueprint Coverage via the Orphans projection computation. |
| `measure_bpfunc` | Code Traceability per module: code functions named in the... |
| `measure_bptrace` | Blueprint Traceability via the Shaping projection computa... |
| `measure_codeent` | Code Entropy per module: symptom count against the refact... |
| `measure_concept_testcov` | Concept Test Coverage: which ontology concepts have tests. |
| `measure_depvalid` | Dependency Validity via the Validation projection computa... |
| `measure_epic_progress` | Epic Progress: completed / total stories in the story fol... |
| `measure_issue_rec` | Issue Recurrence: recurring issue types per epic. |
| `measure_karma` | Karma per document: usage counts from the DuckDB usage ta... |
| `measure_know_chg_fresh` | Knowledge Change Freshness: days since last change per do... |
| `measure_know_use_fresh` | Knowledge Usage Freshness: days since last usage record p... |
| `measure_module_testcov` | Test Coverage per module: regression-tree import evidence. |
| `measure_ontcov` | Ontology Coverage via the Shaping projection computation. |
| `measure_patcov` | Pattern Coverage via the design-patterns projection compu... |
| `measure_story_progress` | Story Progress: AC passing in the most recent story. |
| `measure_testpass` | Test Pass Rate across story test execution tables. |
| `register` | Register a sensor definition. |
| `scan_issue_documents` | Issue rows for the epic: stem, status, occurrence count. |
| `store_readings` | Upsert readings into the DuckDB sensor_reading table (lat... |

#### unassigned

| Function | Description |
|----------|-------------|
| `_cli_modules` | (module, blueprint path, code path) for implementation-cl... |
| `_no_data` | Readings list for a missing data source: empty (rendered ... |
| `_ratio_status` | ok / warning / critical for a higher-is-better ratio. |
| `_story_completed` | True when a story file marks the story completed. |

### snapshot

> Instance State management via snapshots.

**Blueprint:** [implementation-cli-snapshot-blueprint](implementation-cli-snapshot-blueprint)
**Tests:** 5/5 (pass)
**Functions:** 20 (20 with Capability)

#### document-validation

| Function | Description |
|----------|-------------|
| `validate_capabilities` | Validate that all code capabilities are defined in ontology. |

#### instance-state

| Function | Description |
|----------|-------------|
| `_ensure_snapshot_repo` | Ensure snapshot repo exists and is initialized. |
| `_get_authenticated_remote` | Get authenticated remote URL with token. |
| `check_blueprint_sync` | Check if modified .py modules have updated blueprints. |
| `check_cli_export_sync` | Check if CLI exports match actual command count. |
| `create_snapshot` | Create new snapshot of Instance. |
| `diff_for_story` | Generate diff for Story (baseline to current). |
| `diff_from_last` | Generate diff from last snapshot to current Instance state. |
| `diff_snapshots` | Generate diff between two snapshots. |
| `effective_push` | Effective push: the explicit param AND the instance confi... |
| `generate_artifact_map` | Generate Artifact Map from git diff output. |
| `get_credential_strategy` | Get the instance credential strategy for remote liveness. |
| `get_exclusions` | Get excluded patterns for snapshot. |
| `get_instance_config` | Get the global instance config from <root>/_config/instan... |
| `get_instance_id` | Get the stable Instance identity (8-hex id from the insta... |
| `get_instance_root` | Get Ahabase instance root path. |
| `get_last_snapshot` | Get most recent snapshot commit hash. |
| `get_snapshot_dir` | Get path to snapshot repository. |
| `get_story_baseline` | Get baseline snapshot for a Story. |
| `tag_snapshot` | Tag snapshot with Story identifier. |

### status

> Status and story detection logic.

**Blueprint:** [implementation-cli-status-blueprint](implementation-cli-status-blueprint)
**Tests:** 5/5 (pass)
**Functions:** 4 (4 with Capability)

#### parsing

| Function | Description |
|----------|-------------|
| `extract_goal` | Extract short description from story file. |
| `is_story_file` | Check if file is a story file (TICKET-*.md or EPIC-SUBEPI... |

#### story-tracking

| Function | Description |
|----------|-------------|
| `get_llm_instruction` | Get LLM instruction based on current state. |
| `get_wiki_status` | Get status for a single wiki. |

### story

> Story and release management commands.

**Blueprint:** [implementation-cli-story-blueprint](implementation-cli-story-blueprint)
**Tests:** 0/0 (not_run)
**Functions:** 28 (12 with Capability)

#### story-tracking

| Function | Description |
|----------|-------------|
| `_build_version` | Build version string based on last release and what changed. |
| `_find_story_path` | Find story file path - handles both epic and subepic stor... |
| `_get_last_epic_release` | Get the last epic release version number (the epic_story ... |
| `_get_last_release` | Get the last release version components. |
| `_get_last_story_release` | Get the last release version for a SPECIFIC story. |
| `_get_story_target_path` | Get target path for a story file (for creating/moving). |
| `_get_story_type_info` | Resolve a story document's **Type:** to its type config. |
| `_get_subepic_from_config` | Check if story belongs to a subepic based on config story... |
| `_reconcile_active_pointer` | Reconcile the active pointer with a story completion. |
| `story_create` | Create a new Story with specified type. |
| `story_reopen` | Reopen completed story for patch release. |
| `story_switch` | Switch to a story (set active and checkout branch). |

#### unassigned

| Function | Description |
|----------|-------------|
| `_extract_story_number` | Extract numeric part from story ID for sorting. |
| `_find_latest_tag` | Find the latest tag for a story. |
| `_get_repo_from_remote` | Extract owner/repo and username from git remote URL. |
| `_get_subepic_order` | Get subepic order by alphabetical position in subepic/ dir. |
| `_parse_story_id` | Parse story ID into components. |
| `_switch_gh_account` | Switch gh CLI to specified account. |
| `archive_old_stories` | Archive old stories to history/ subfolder. |
| `normalize_story_dashes` | Normalize dash characters in story filenames. |
| `release_group` | Release management commands. |
| `release_prepare` | Verify clean state before release. |
| `release_publish` | Create GitHub release for latest tag. |
| `release_run` | Release workflow: prepare → tag → publish. |
| `release_tag` | Create release tag with auto-increment patch. |
| `story_complete` | Complete story after tests pass: verify → commit → merge ... |
| `story_group` | Story management commands. |
| `story_types_cmd` | List available story types for an Epic. |

### sync

> Sync logic - main workflow.

**Blueprint:** [implementation-cli-sync-blueprint](implementation-cli-sync-blueprint)
**Tests:** 0/0 (not_run)
**Functions:** 6 (5 with Capability)

#### data-persistence

| Function | Description |
|----------|-------------|
| `_check_author_changes` | Check for author changes in parsed stories. |
| `_migrate_last_sync_keys` | Re-key legacy folder-named last_sync entries to Epic name... |
| `sync` | Main sync workflow. Returns True if changes were processed. |
| `verify` | Verify MD == JSON == DuckDB == Kuzu. |

#### export-generation

| Function | Description |
|----------|-------------|
| `_get_epic_name` | Extract Epic name (the cloned repository directory) from ... |

#### unassigned

| Function | Description |
|----------|-------------|
| `iter_km_files` | Yield real knowledge-map files, excluding pattern templates. |

### test_runner

> Test runner for -tests.md files.

**Blueprint:** [implementation-cli-test_runner-blueprint](implementation-cli-test_runner-blueprint)
**Tests:** 6/6 (pass)
**Functions:** 7 (7 with Capability)

#### config-management

| Function | Description |
|----------|-------------|
| `_get_timbr_python` | Get Python path from timbr runtime config. |

#### export-generation

| Function | Description |
|----------|-------------|
| `update_execution_table` | Update Execution table in -tests.md file with test results. |

#### parsing

| Function | Description |
|----------|-------------|
| `expand_variables` | Expand variables in command string. |
| `extract_yaml_block` | Extract yaml block from ## Definition section. |
| `parse_tests` | Parse yaml content into test specifications. |

#### test-execution

| Function | Description |
|----------|-------------|
| `run_test` | Execute a single test and validate expectations. |
| `run_tests_from_file` | Run tests from a -tests.md file. |

### verify

> Document verification logic.

**Blueprint:** [implementation-cli-verify-blueprint](implementation-cli-verify-blueprint)
**Tests:** 0/0 (not_run)
**Functions:** 7 (7 with Capability)

#### document-validation

| Function | Description |
|----------|-------------|
| `_validate_ontology_file` | Validate ontology-blueprint.md consistency. |
| `_validate_story_lifecycle` | Validate story lifecycle rules. |
| `is_type_blueprint` | Check if file is a type-blueprint (defines rules for othe... |
| `run_check` | Run a single validation check. Returns (errors, warnings). |
| `verify_file` | Verify file structure against its blueprint. |
| `verify_stdin_content` | Verify content from stdin against document type rules. |

#### issue-matching

| Function | Description |
|----------|-------------|
| `_check_entropy` | Check content for entropy patterns. |

### wiki

> Wiki sync commands.

**Blueprint:** [implementation-cli-wiki-blueprint](implementation-cli-wiki-blueprint)
**Tests:** -
**Functions:** 9 (9 with Capability)

#### wiki-sync

| Function | Description |
|----------|-------------|
| `sync_document` | Copy a single document from source to target. |
| `wiki_clean` | Remove duplicate files from subfolders, keeping root copy. |
| `wiki_generate` | Generate _Sidebar.md and Home.md from config. |
| `wiki_group` | Wiki sync commands. |
| `wiki_sync` | Sync documents from _grid4d to wiki based on config. |

#### wiki-validation

| Function | Description |
|----------|-------------|
| `find_duplicates` | Find duplicate files in wiki (same filename in multiple l... |
| `load_wiki_config` | Load wiki configuration for Epic. |
| `resolve_wiki_paths` | Resolve wiki target and source paths. |
| `wiki_check` | Validate wiki structure, detect duplicates, check links. |

---

## Commands

| Command | Description |
|---------|-------------|
| `active-story` | Show current active story and model (debug command). |
| `claude current` | Show current provider and model with recommendations. |
| `claude doctor` | Audit Claude Code hook events: OK / DRIFT / DEAD + opportunities. |
| `claude list` | List all providers with local availability. |
| `claude list-backups` | List available backup files. |
| `claude list-models` | List available models for a provider. |
| `claude model-history` | Show model usage history. |
| `claude prefer-model` | Set preference for a model (preferred/avoid). |
| `claude restore` | Restore settings from backup. |
| `claude rollback` | Rollback to last known good configuration (FASTEST recovery). |
| `claude status` | Show current Claude Code configuration with context. |
| `claude switch` | Switch to a different Claude Code provider with automatic model selection. |
| `claude switch-model` | Switch to a different model of the current provider. |
| `claude sync` | Sync provider registry from remote source. |
| `claude sync-simulate` | Simulate provider registry sync without making changes. |
| `claude sync-status` | Show provider registry sync status. |
| `config check-token` | Check if GitHub token(s) are valid. |
| `config show` | Show current configuration. |
| `config update-token` | Update GitHub PAT token for an organization. |
| `doctor` | Check installation and dependencies. |
| `epic init` | Scaffold NAME inside its prepared clone and register it in ahabase.yaml. |
| `epic init-subepic` | Scaffold a minimal SubEpic NAME inside an initialized EPIC clone. |
| `export-dbt` | Generate dbt project exports for an epic. |
| `export-gradient` | Generate gradient report comparing blueprints to code. |
| `export-karma` | Generate Karma-Report.md to all Epics. |
| `extract-functions` | Extract functions with Capabilities from CLI module. |
| `extract-rules` | Extract validation rules from type-blueprints. |
| `fork` | Create a new version (fork) of a document. |
| `hook-handler` | Handle PostToolUse hooks from Claude Code. |
| `init` | Setup complete Evolucean game board. |
| `karma` | Show karma metrics. |
| `link fix` | Fix path_in_link issues by converting to filename-only. |
| `llm check` | Check LLM configuration and dependencies. |
| `llm config-status` | Show which LLM hook instructions come from the pattern vs code. |
| `llm discover-models` | Discover currently working free models from OpenRouter. |
| `llm free-models-update` | Update OpenRouter free models in config.yaml. |
| `llm lmstudio-auto-setup` | Complete automated LM Studio setup. |
| `llm lmstudio-daemon-logs` | Show LM Studio daemon logs. |
| `llm lmstudio-daemon-restart` | Restart LM Studio daemon. |
| `llm lmstudio-daemon-start` | Start LM Studio daemon. |
| `llm lmstudio-daemon-status` | Check LM Studio daemon status. |
| `llm lmstudio-daemon-stop` | Stop LM Studio daemon. |
| `llm lmstudio-download-model` | Download and load model to LM Studio. |
| `llm lmstudio-install` | Check/install LM Studio application. |
| `llm lmstudio-status` | Check LM Studio status and loaded model. |
| `llm lmstudio-test` | Test LM Studio completion. |
| `llm lmstudio-watchdog` | LM Studio watchdog - check and auto-restart. |
| `llm path-list` | List known LLM access paths and which one is current. |
| `llm path-switch` | Switch Claude Code to a verified access path (preflight first). |
| `llm path-verify` | Preflight-verify an access path with a minimal messages request. |
| `llm proxy-configure` | Configure Claude Code to use LiteLLM proxy. |
| `llm proxy-generate-config` | Generate LiteLLM proxy configuration file. |
| `llm proxy-start` | Start LiteLLM proxy for Claude Code integration. |
| `llm proxy-status` | Check LiteLLM proxy status. |
| `llm proxy-stop` | Stop LiteLLM proxy server. |
| `llm recommend-config` | Generate recommended LiteLLM config based on working models. |
| `llm recover` | Revive the LiteLLM proxy offline (run outside Claude Code). |
| `llm service-doctor` | Run LiteLLM service diagnostics. |
| `llm service-install` | Install and start LiteLLM as launchd service. |
| `llm service-logs` | Show LiteLLM service logs. |
| `llm service-restart` | Restart LiteLLM launchd service. |
| `llm service-status` | Show LiteLLM launchd service status. |
| `llm service-uninstall` | Uninstall LiteLLM launchd service. |
| `llm step-map` | Show step profiles and the selection proposal for a task type. |
| `llm telemetry-env` | Show (default) or install the telemetry env block. |
| `llm telemetry-start` | Start the agent telemetry OTLP collector. |
| `llm telemetry-status` | Show collector status, last activity and env-block state. |
| `llm telemetry-stop` | Stop the agent telemetry OTLP collector. |
| `llm-init` | Initialize LLM module configuration. |
| `llm-update` | Update OpenRouter free models list from API. |
| `ontology validate` | Validate ontology/ folder structure and cross-references. |
| `pattern fix` | Rename patterns to use epic/subepic prefix. |
| `pattern list` | List available patterns for a context. |
| `pattern show` | Show effective pattern with lineage info. |
| `pattern validate` | Validate all documents against their patterns. |
| `pause` | Pause active story - keeps it in pool but stops tracking. |
| `projection` | Generate Epic-level projections to _generated/epic/. |
| `query` | Run ad-hoc query. |
| `resume` | Resume a story from pool (or show pool if no argument). |
| `sensor list` | List registered sensors and their gradient metrics. |
| `sensor read` | Measure all implemented sensors and store readings to DuckDB. |
| `snapshot baseline` | Tag current snapshot as baseline for Story. |
| `snapshot completion` | Tag current snapshot as completion for Story. |
| `snapshot create` | Create new snapshot of Instance. |
| `snapshot diff` | Show diff between snapshots. |
| `snapshot list` | List recent snapshots. |
| `status` | Show game status - active story, open stories, debt. |
| `stop-handler` | Game Master - show game status and guide next move. |
| `sync` | Pull + parse + load + verify + export (if changes). |
| `test` | Execute tests from a -tests.md file. |
| `test-role` | Test role determination (for testing). |
| `test-scope` | Test scope determination (for testing). |
| `verify` | Check consistency (MD == JSON == DBs + Capabilities). |
| `verify-capabilities` | Verify Capability declarations in CLI module(s). |
| `verify-file` | Verify single file structure against its blueprint. |
| `verify-stdin` | Verify content from stdin against document type rules. |

---

## Capabilities

### claude-cli

**Modules:** 1 | **Functions:** 17

| Module | Function |
|--------|----------|
| claude_cli_commands | `_create_backup` |
| claude_cli_commands | `_get_last_known_good_path` |
| claude_cli_commands | `_save_last_known_good` |
| claude_cli_commands | `_validate_provider_switch` |
| claude_cli_commands | `_write_settings_atomic` |
| claude_cli_commands | `get_current_provider_and_model` |
| claude_cli_commands | `get_model_history` |
| claude_cli_commands | `list_backups` |
| claude_cli_commands | `list_provider_models` |
| claude_cli_commands | `list_providers` |
| claude_cli_commands | `restore_backup` |
| claude_cli_commands | `rollback_last_known_good` |
| claude_cli_commands | `set_model_preference` |
| claude_cli_commands | `show_status` |
| claude_cli_commands | `switch_model_only` |
| claude_cli_commands | `switch_provider` |
| claude_cli_commands | `switch_provider_with_model` |

### claude-config

**Modules:** 1 | **Functions:** 11

| Module | Function |
|--------|----------|
| claude_claude_config | `__post_init__` |
| claude_claude_config | `__post_init__` |
| claude_claude_config | `detect_environment_context` |
| claude_claude_config | `discover_providers` |
| claude_claude_config | `get_current_provider` |
| claude_claude_config | `get_machine_id` |
| claude_claude_config | `get_settings_path` |
| claude_claude_config | `read_settings` |
| claude_claude_config | `select_best_provider` |
| claude_claude_config | `test_provider_availability` |
| claude_claude_config | `write_settings` |

### claude-model-selection

**Modules:** 1 | **Functions:** 10

| Module | Function |
|--------|----------|
| claude_model_selection | `__post_init__` |
| claude_model_selection | `format_provider_models_for_registry` |
| claude_model_selection | `get_available_models` |
| claude_model_selection | `get_model_info` |
| claude_model_selection | `get_model_stats` |
| claude_model_selection | `parse_provider_models` |
| claude_model_selection | `recommend_models` |
| claude_model_selection | `record_usage` |
| claude_model_selection | `select_best_model` |
| claude_model_selection | `set_user_preference` |

### claude-provider-registry

**Modules:** 1 | **Functions:** 20

| Module | Function |
|--------|----------|
| claude_provider_registry | `from_dict` |
| claude_provider_registry | `from_dict` |
| claude_provider_registry | `from_dict` |
| claude_provider_registry | `from_dict` |
| claude_provider_registry | `get_available_providers` |
| claude_provider_registry | `get_default_model` |
| claude_provider_registry | `get_default_registry_path` |
| claude_provider_registry | `get_local_availability` |
| claude_provider_registry | `get_provider_by_type` |
| claude_provider_registry | `get_registry_path` |
| claude_provider_registry | `import_provider_from_discovery` |
| claude_provider_registry | `is_experimental` |
| claude_provider_registry | `load_registry` |
| claude_provider_registry | `save_registry` |
| claude_provider_registry | `to_dict` |
| claude_provider_registry | `to_dict` |
| claude_provider_registry | `to_dict` |
| claude_provider_registry | `to_dict` |
| claude_provider_registry | `update_local_availability` |
| claude_provider_registry | `update_local_context` |

### claude-provider-sync

**Modules:** 1 | **Functions:** 6

| Module | Function |
|--------|----------|
| claude_provider_sync | `_is_newer` |
| claude_provider_sync | `_merge_providers` |
| claude_provider_sync | `get_registry_sync_status` |
| claude_provider_sync | `merge_registries` |
| claude_provider_sync | `simulate_sync` |
| claude_provider_sync | `sync_provider_registry` |

### cli-command

**Modules:** 1 | **Functions:** 62

| Module | Function |
|--------|----------|
| cli | `_is_story_file` |
| cli | `_verify_file_internal` |
| cli | `active_story` |
| cli | `claude` |
| cli | `claude_current` |
| cli | `claude_doctor` |
| cli | `claude_list` |
| cli | `claude_list_backups` |
| cli | `claude_list_models` |
| cli | `claude_model_history` |
| cli | `claude_prefer_model` |
| cli | `claude_restore` |
| cli | `claude_rollback` |
| cli | `claude_status` |
| cli | `claude_switch` |
| cli | `claude_switch_model` |
| cli | `claude_sync` |
| cli | `claude_sync_simulate` |
| cli | `claude_sync_status` |
| cli | `config` |
| cli | `config` |
| cli | `config_check_token` |
| cli | `config_show` |
| cli | `config_update_token` |
| cli | `doctor` |
| cli | `extract_rules` |
| cli | `fork` |
| cli | `hook_handler` |
| cli | `karma` |
| cli | `llm` |
| cli | `llm_check` |
| cli | `llm_init` |
| cli | `llm_proxy_configure` |
| cli | `llm_proxy_generate_config` |
| cli | `llm_proxy_start` |
| cli | `llm_proxy_status` |
| cli | `llm_proxy_stop` |
| cli | `llm_telemetry_env` |
| cli | `llm_telemetry_start` |
| cli | `llm_telemetry_status` |
| cli | `llm_telemetry_stop` |
| cli | `llm_update` |
| cli | `ontology` |
| cli | `pattern` |
| cli | `pattern_list` |
| cli | `pattern_show` |
| cli | `pattern_validate` |
| cli | `pause_story` |
| cli | `resume_story` |
| cli | `snapshot` |
| cli | `snapshot_baseline` |
| cli | `snapshot_completion` |
| cli | `snapshot_create` |
| cli | `snapshot_diff` |
| cli | `snapshot_list` |
| cli | `status` |
| cli | `stop_handler` |
| cli | `test` |
| cli | `test_role` |
| cli | `test_scope` |
| cli | `verify_file_cmd` |
| cli | `verify_stdin_cmd` |

### config-management

**Modules:** 11 | **Functions:** 78

| Module | Function |
|--------|----------|
| bootstrap | `load_registry` |
| bootstrap | `register_epic` |
| bootstrap | `register_subepic` |
| bootstrap | `write_registry` |
| check_executor | `load_document_rules` |
| cli | `cli` |
| cli | `init` |
| config | `_expand_path` |
| config | `_get_settings_path` |
| config | `_get_subepic_for_story` |
| config | `check_github_token` |
| config | `ensure_gh_account` |
| config | `get_all_repositories` |
| config | `get_all_story_prefixes` |
| config | `get_claude_hooks` |
| config | `get_cli_src_dir` |
| config | `get_clone_url` |
| config | `get_config_dir` |
| config | `get_configured_epics` |
| config | `get_configured_epics_knowledge` |
| config | `get_configured_knowledge_paths` |
| config | `get_data_dir` |
| config | `get_document_types` |
| config | `get_epic_branch` |
| config | `get_epic_from_knowledge_path` |
| config | `get_epic_gh_account` |
| config | `get_epic_git_operations` |
| config | `get_epic_knowledge_path` |
| config | `get_epic_merge` |
| config | `get_epic_names` |
| config | `get_epic_release` |
| config | `get_epic_snapshot_on_complete` |
| config | `get_epic_story_history_keep` |
| config | `get_epic_story_lifecycle` |
| config | `get_github_token_orgs` |
| config | `get_idle_stop_cooldown_seconds` |
| config | `get_json_dir` |
| config | `get_primary_epic` |
| config | `get_primary_wiki` |
| config | `get_project_root` |
| config | `get_queries_dir` |
| config | `get_repo_path` |
| config | `get_repository_config` |
| config | `get_schema_dir` |
| config | `get_state_path` |
| config | `get_stop_cooldown_seconds` |
| config | `get_story_lifecycle` |
| config | `get_story_pattern` |
| config | `get_story_type_config` |
| config | `get_story_type_requirements` |
| config | `get_story_types` |
| config | `get_templates_dir` |
| config | `get_wiki_path` |
| config | `get_wikis_dir` |
| config | `get_workspace_dir` |
| config | `is_local_epic` |
| config | `is_local_repo` |
| config | `load_ahabase_config` |
| config | `load_secrets` |
| config | `load_settings` |
| config | `load_state` |
| config | `save_state` |
| config | `update_github_token` |
| dbt_export | `get_dbt_export_config` |
| git_utils | `update_settings_to_local` |
| km_logger | `get_km_path` |
| projections_base | `grid4d_path` |
| projections_base | `has_ontology` |
| projections_base | `implementation_path` |
| projections_base | `ontology_path` |
| projections_base | `story_path` |
| projections_registry | `clear` |
| projections_registry | `create` |
| projections_registry | `list` |
| projections_registry | `names_for_scope` |
| projections_registry | `register` |
| rule_extractor | `get_type_blueprints` |
| test_runner | `_get_timbr_python` |

### data-persistence

**Modules:** 4 | **Functions:** 19

| Module | Function |
|--------|----------|
| cli | `sync` |
| cli | `verify` |
| db | `__init__` |
| db | `_init_schema` |
| db | `delete_stories` |
| db | `ensure_schema` |
| db | `get_kuzu_story_ids` |
| db | `get_stored_doc_author` |
| db | `get_story_ids` |
| db | `get_usage_epics` |
| db | `insert_many` |
| db | `query_cypher` |
| db | `query_sql` |
| db | `upsert_story_status` |
| parser | `parse_and_save_json` |
| sync | `_check_author_changes` |
| sync | `_migrate_last_sync_keys` |
| sync | `sync` |
| sync | `verify` |

### dbt-export

**Modules:** 2 | **Functions:** 9

| Module | Function |
|--------|----------|
| cli | `export_dbt` |
| dbt_export | `export_dbt` |
| dbt_export | `generate_dbt_index` |
| dbt_export | `generate_mart_export` |
| dbt_export | `get_model_layer` |
| dbt_export | `get_source_dependencies` |
| dbt_export | `get_upstream_chain` |
| dbt_export | `parse_manifest` |
| dbt_export | `run_dbt_setup` |

### document-validation

**Modules:** 7 | **Functions:** 23

| Module | Function |
|--------|----------|
| capability_extractor | `validate_module_capabilities` |
| check_executor | `check_at_least_one` |
| check_executor | `check_has_subsection` |
| check_executor | `check_list_format` |
| check_executor | `check_not_empty` |
| check_executor | `check_unique_across` |
| check_executor | `execute_checks` |
| check_executor | `validate_document` |
| check_executor | `validate_type_blueprint` |
| cli | `ontology_validate` |
| cli | `verify_capabilities` |
| ontology | `check_index_completeness` |
| ontology | `check_required_sections` |
| ontology | `validate_ontology` |
| parser | `_validate_doc_exists` |
| parser | `_validate_one_doc_one_place` |
| snapshot | `validate_capabilities` |
| verify | `_validate_ontology_file` |
| verify | `_validate_story_lifecycle` |
| verify | `is_type_blueprint` |
| verify | `run_check` |
| verify | `verify_file` |
| verify | `verify_stdin_content` |

### epic-bootstrap

**Modules:** 1 | **Functions:** 2

| Module | Function |
|--------|----------|
| bootstrap | `epic_init` |
| bootstrap | `subepic_init` |

### export-generation

**Modules:** 8 | **Functions:** 19

| Module | Function |
|--------|----------|
| capability_extractor | `_extract_function_info` |
| capability_extractor | `extract_capabilities_by_module` |
| capability_extractor | `extract_cli_commands` |
| capability_extractor | `extract_module_functions` |
| capability_extractor | `get_valid_capabilities` |
| cli | `export_karma` |
| cli | `extract_functions` |
| karma_export | `_build_file_index` |
| karma_export | `_get_epic_name` |
| karma_export | `_is_valid_doc_name` |
| karma_export | `export_karma_report` |
| km_logger | `ensure_km_structure` |
| parser | `clear_json_dir` |
| parser | `delete_json` |
| rule_extractor | `extract_all_rules` |
| rule_extractor | `generate_document_rules_yaml` |
| rule_extractor | `save_document_rules` |
| sync | `_get_epic_name` |
| test_runner | `update_execution_table` |

### git-operations

**Modules:** 4 | **Functions:** 22

| Module | Function |
|--------|----------|
| bootstrap | `read_remote` |
| counters | `_git` |
| counters | `_push_counters` |
| counters | `_read_remote_counters` |
| counters | `_remote_branch_exists` |
| counters | `allocate` |
| counters | `has_remote` |
| git_utils | `_get_repo_root` |
| git_utils | `get_doc_author` |
| git_utils | `git_diff_status` |
| git_utils | `git_file_info` |
| git_utils | `git_head` |
| git_utils | `git_pull` |
| git_utils | `git_revert_to_author` |
| git_utils | `has_uncommitted` |
| git_utils | `init_git_repo` |
| git_utils | `is_git_repo` |
| git_utils | `is_remote_accessible` |
| hooks | `_get_git_changes` |
| hooks | `_get_recent_commits` |
| hooks | `get_wiki_git_status` |
| hooks | `needs_sync` |

### gradient-check

**Modules:** 2 | **Functions:** 4

| Module | Function |
|--------|----------|
| cli | `export_gradient` |
| gradient | `calculate_gradient` |
| gradient | `generate_gradient_report` |
| gradient | `get_all_cli_modules` |

### hook-handling

**Modules:** 1 | **Functions:** 4

| Module | Function |
|--------|----------|
| hooks | `_format_no_story_enforcement` |
| hooks | `audit_hook_registration` |
| hooks | `handle_post_tool_use` |
| hooks | `handle_stop` |

### instance-state

**Modules:** 1 | **Functions:** 19

| Module | Function |
|--------|----------|
| snapshot | `_ensure_snapshot_repo` |
| snapshot | `_get_authenticated_remote` |
| snapshot | `check_blueprint_sync` |
| snapshot | `check_cli_export_sync` |
| snapshot | `create_snapshot` |
| snapshot | `diff_for_story` |
| snapshot | `diff_from_last` |
| snapshot | `diff_snapshots` |
| snapshot | `effective_push` |
| snapshot | `generate_artifact_map` |
| snapshot | `get_credential_strategy` |
| snapshot | `get_exclusions` |
| snapshot | `get_instance_config` |
| snapshot | `get_instance_id` |
| snapshot | `get_instance_root` |
| snapshot | `get_last_snapshot` |
| snapshot | `get_snapshot_dir` |
| snapshot | `get_story_baseline` |
| snapshot | `tag_snapshot` |

### issue-matching

**Modules:** 2 | **Functions:** 5

| Module | Function |
|--------|----------|
| issue_matcher | `get_entropy_warnings` |
| issue_matcher | `get_error_suggestion` |
| issue_matcher | `match_entropy_pattern` |
| issue_matcher | `match_error_pattern` |
| verify | `_check_entropy` |

### knowledge-map-logging

**Modules:** 1 | **Functions:** 2

| Module | Function |
|--------|----------|
| km_logger | `add_entry` |
| km_logger | `log_file_access` |

### link-management

**Modules:** 1 | **Functions:** 2

| Module | Function |
|--------|----------|
| cli | `link` |
| cli | `link_fix` |

### llm-agent

**Modules:** 1 | **Functions:** 8

| Module | Function |
|--------|----------|
| llm_agent | `_proxy_routing` |
| llm_agent | `_resolve_bedrock_direct` |
| llm_agent | `agent_indicator` |
| llm_agent | `agent_models` |
| llm_agent | `json_loads` |
| llm_agent | `resolve_agent_model` |
| llm_agent | `resolve_inference_profile` |
| llm_agent | `strip_profile_prefix` |

### llm-configuration

**Modules:** 2 | **Functions:** 10

| Module | Function |
|--------|----------|
| cli | `llm_config_status` |
| llm_config | `config_layer` |
| llm_config | `config_status` |
| llm_config | `config_value` |
| llm_config | `hook_instruction` |
| llm_config | `hook_instructions_layer` |
| llm_config | `instance_config_layer` |
| llm_config | `instance_config_path` |
| llm_config | `parse_pattern_config` |
| llm_config | `pattern_path` |

### llm-lmstudio

**Modules:** 2 | **Functions:** 19

| Module | Function |
|--------|----------|
| cli | `llm_lmstudio_auto_setup` |
| cli | `llm_lmstudio_download_model` |
| cli | `llm_lmstudio_install` |
| llm_lmstudio | `_find_llama_server` |
| llm_lmstudio | `_install_lmstudio_linux` |
| llm_lmstudio | `_install_lmstudio_macos` |
| llm_lmstudio | `_install_lmstudio_windows` |
| llm_lmstudio | `check_lmstudio_installed` |
| llm_lmstudio | `create_daemon_scripts` |
| llm_lmstudio | `download_model` |
| llm_lmstudio | `from_dict` |
| llm_lmstudio | `get_alternative_models` |
| llm_lmstudio | `get_default_model_config` |
| llm_lmstudio | `get_lmstudio_config` |
| llm_lmstudio | `get_project_root` |
| llm_lmstudio | `install_lmstudio` |
| llm_lmstudio | `list_available_models` |
| llm_lmstudio | `start_daemon` |
| llm_lmstudio | `verify_setup` |

### llm-model-config

**Modules:** 1 | **Functions:** 22

| Module | Function |
|--------|----------|
| llm_model_config | `__init__` |
| llm_model_config | `_categorize_model` |
| llm_model_config | `_generate_config` |
| llm_model_config | `_generate_selection_criteria` |
| llm_model_config | `_generate_task_mapping` |
| llm_model_config | `_generate_yaml_from_models` |
| llm_model_config | `_is_config_old` |
| llm_model_config | `_load_config` |
| llm_model_config | `_sort_by_scores` |
| llm_model_config | `_update_from_api` |
| llm_model_config | `filter_by_category` |
| llm_model_config | `filter_by_min_quality` |
| llm_model_config | `filter_by_task_type` |
| llm_model_config | `from_dict` |
| llm_model_config | `get_all_models` |
| llm_model_config | `get_auto_selected_model` |
| llm_model_config | `get_model` |
| llm_model_config | `get_model_config` |
| llm_model_config | `get_project_root` |
| llm_model_config | `select_best_for_task_type` |
| llm_model_config | `supports_task_type` |
| llm_model_config | `update_models` |

### llm-openrouter

**Modules:** 1 | **Functions:** 9

| Module | Function |
|--------|----------|
| llm_openrouter | `_defensive_update` |
| llm_openrouter | `_get_api_key` |
| llm_openrouter | `_is_model_available` |
| llm_openrouter | `complete` |
| llm_openrouter | `discover_working_free_models` |
| llm_openrouter | `get_free_models` |
| llm_openrouter | `get_recommended_config` |
| llm_openrouter | `test_model` |
| llm_openrouter | `verify_api_key` |

### llm-paths

**Modules:** 2 | **Functions:** 15

| Module | Function |
|--------|----------|
| cli | `llm_path_list` |
| cli | `llm_path_switch` |
| cli | `llm_path_verify` |
| cli | `llm_recover` |
| llm_paths | `_probe_suffixes` |
| llm_paths | `_settings_env` |
| llm_paths | `current_path` |
| llm_paths | `known_paths` |
| llm_paths | `path_sensors` |
| llm_paths | `recover_service` |
| llm_paths | `recover_with_fallback` |
| llm_paths | `resolve_auth` |
| llm_paths | `switch_path` |
| llm_paths | `validate_proxy_config` |
| llm_paths | `verify_path` |

### llm-proxy

**Modules:** 1 | **Functions:** 19

| Module | Function |
|--------|----------|
| llm_proxy | `_asked_alias` |
| llm_proxy | `_fallback_depth` |
| llm_proxy | `_format_from_health` |
| llm_proxy | `check_litellm_installed` |
| llm_proxy | `check_openrouter_api_key` |
| llm_proxy | `ensure_config` |
| llm_proxy | `format_model_status` |
| llm_proxy | `generate_config` |
| llm_proxy | `get_claude_code_config` |
| llm_proxy | `get_default_config` |
| llm_proxy | `get_last_used_model` |
| llm_proxy | `get_proxy_health` |
| llm_proxy | `ingest_usage_history` |
| llm_proxy | `is_proxy_running` |
| llm_proxy | `log_success_event` |
| llm_proxy | `record_model_usage` |
| llm_proxy | `restore_claude_code_config` |
| llm_proxy | `set_claude_code_proxy_config` |
| llm_proxy | `start_proxy` |

### llm-selection

**Modules:** 2 | **Functions:** 6

| Module | Function |
|--------|----------|
| cli | `llm_step_map` |
| llm_selection | `format_proposal` |
| llm_selection | `is_paid_model` |
| llm_selection | `resolve_step_profile` |
| llm_selection | `select_step_model` |
| llm_selection | `usage_evidence` |

### llm-service

**Modules:** 2 | **Functions:** 44

| Module | Function |
|--------|----------|
| cli | `llm_discover_models` |
| cli | `llm_free_models_update` |
| cli | `llm_lmstudio_daemon_logs` |
| cli | `llm_lmstudio_daemon_restart` |
| cli | `llm_lmstudio_daemon_start` |
| cli | `llm_lmstudio_daemon_status` |
| cli | `llm_lmstudio_daemon_stop` |
| cli | `llm_lmstudio_status` |
| cli | `llm_lmstudio_test` |
| cli | `llm_lmstudio_watchdog` |
| cli | `llm_recommend_config` |
| cli | `llm_service_doctor` |
| cli | `llm_service_install` |
| cli | `llm_service_logs` |
| cli | `llm_service_restart` |
| cli | `llm_service_status` |
| cli | `llm_service_uninstall` |
| llm_service | `check_claude_settings_conflict` |
| llm_service | `check_lmstudio` |
| llm_service | `check_lmstudio_daemon_installed` |
| llm_service | `check_openrouter_free_models_quick` |
| llm_service | `create_launchd_service` |
| llm_service | `default` |
| llm_service | `detect_environment` |
| llm_service | `ensure_directories` |
| llm_service | `generate_config` |
| llm_service | `get_lmstudio_daemon_logs` |
| llm_service | `get_lmstudio_daemon_script` |
| llm_service | `get_lmstudio_daemon_status` |
| llm_service | `get_lmstudio_models` |
| llm_service | `get_logs` |
| llm_service | `get_service_status` |
| llm_service | `install_litellm` |
| llm_service | `lmstudio_daemon_restart` |
| llm_service | `lmstudio_daemon_start` |
| llm_service | `lmstudio_daemon_stop` |
| llm_service | `lmstudio_watchdog_check` |
| llm_service | `load_service` |
| llm_service | `run_doctor` |
| llm_service | `test_lmstudio_completion` |
| llm_service | `uninstall_service` |
| llm_service | `unload_service` |
| llm_service | `update_config_with_free_models` |
| llm_service | `validate_prerequisites` |

### llm-telemetry

**Modules:** 1 | **Functions:** 18

| Module | Function |
|--------|----------|
| llm_telemetry | `_attr_value` |
| llm_telemetry | `_decode_attributes` |
| llm_telemetry | `_load_settings` |
| llm_telemetry | `_log_collector_line` |
| llm_telemetry | `_record_event_name` |
| llm_telemetry | `_record_timestamp` |
| llm_telemetry | `_usage_history_path` |
| llm_telemetry | `append_agent_telemetry` |
| llm_telemetry | `collector_stats` |
| llm_telemetry | `handle_otlp_logs` |
| llm_telemetry | `install_telemetry_env` |
| llm_telemetry | `is_collector_running` |
| llm_telemetry | `main` |
| llm_telemetry | `parse_api_requests` |
| llm_telemetry | `run_collector` |
| llm_telemetry | `show_telemetry_env` |
| llm_telemetry | `start_collector` |
| llm_telemetry | `stop_collector` |

### naming

**Modules:** 1 | **Functions:** 1

| Module | Function |
|--------|----------|
| bootstrap | `canonical_subepic` |

### parsing

**Modules:** 14 | **Functions:** 43

| Module | Function |
|--------|----------|
| bootstrap | `clean_remote_url` |
| bootstrap | `remote_owner` |
| capability_extractor | `extract_capability_from_docstring` |
| check_executor | `extract_links_from_section` |
| check_executor | `extract_template_content` |
| check_executor | `find_sections` |
| check_executor | `find_subsections` |
| cli | `query` |
| hooks | `_get_story_type_from_content` |
| hooks | `_parse_test_results_per_requirement` |
| hooks | `parse_acceptance_criteria` |
| hooks | `parse_execution_table` |
| hooks | `update_execution_table` |
| km_logger | `entry_exists` |
| km_logger | `find_or_create_section` |
| km_logger | `normalize_km` |
| links | `extract_links` |
| links | `get_all_links` |
| links | `get_incoming_links` |
| ontology | `extract_vocabulary_links` |
| ontology | `get_ontology_files` |
| parser | `_check_deploy_to_test` |
| parser | `_check_tests_pass` |
| parser | `clear_validation_errors` |
| parser | `extract_doc_reference` |
| parser | `extract_story_id` |
| parser | `get_epic_and_subepic` |
| parser | `get_validation_errors` |
| parser | `parse_knowledge_sections` |
| parser | `parse_story_success` |
| patterns | `parse_pattern` |
| rule_extractor | `extract_rules_from_blueprint` |
| rule_extractor | `find_sections_markdown_aware` |
| rule_extractor | `parse_structure_table` |
| rule_extractor | `parse_validation_checks` |
| scope_role | `determine_action` |
| scope_role | `determine_role` |
| scope_role | `determine_scope` |
| status | `extract_goal` |
| status | `is_story_file` |
| test_runner | `expand_variables` |
| test_runner | `extract_yaml_block` |
| test_runner | `parse_tests` |

### pattern-driven

**Modules:** 1 | **Functions:** 1

| Module | Function |
|--------|----------|
| hooks | `get_story_behavior` |

### pattern-inference

**Modules:** 1 | **Functions:** 5

| Module | Function |
|--------|----------|
| pattern_inference | `_deep_merge` |
| pattern_inference | `_parse_behavior` |
| pattern_inference | `extract_rules` |
| pattern_inference | `get_behavior_config` |
| pattern_inference | `validate_document` |

### pattern-lookup

**Modules:** 1 | **Functions:** 1

| Module | Function |
|--------|----------|
| km_logger | `_find_pattern_template` |

### pattern-management

**Modules:** 1 | **Functions:** 6

| Module | Function |
|--------|----------|
| patterns | `check_exit_condition` |
| patterns | `determine_phase_state` |
| patterns | `format_phase_status` |
| patterns | `get_current_phase` |
| patterns | `get_pattern_path` |
| patterns | `load_pattern` |

### pattern-resolver

**Modules:** 2 | **Functions:** 7

| Module | Function |
|--------|----------|
| cli | `pattern_fix` |
| pattern_resolver | `_convert_value` |
| pattern_resolver | `_parse_epic_definition` |
| pattern_resolver | `get_context` |
| pattern_resolver | `list_patterns` |
| pattern_resolver | `lookup` |
| pattern_resolver | `lookup_epic_config` |

### projection-generation

**Modules:** 29 | **Functions:** 184

| Module | Function |
|--------|----------|
| cli | `projection` |
| projections_base | `extract` |
| projections_base | `generate` |
| projections_base | `get_timestamp` |
| projections_base | `render` |
| projections_base | `transform` |
| projections_base | `write` |
| projections_epic_artifacts | `_escape_markdown_links` |
| projections_epic_artifacts | `_extract_module_docstring` |
| projections_epic_artifacts | `_parse_test_results` |
| projections_epic_artifacts | `_render_test_coverage` |
| projections_epic_artifacts | `extract` |
| projections_epic_artifacts | `render` |
| projections_epic_artifacts | `transform` |
| projections_epic_capabilities | `_collect_blueprint_files` |
| projections_epic_capabilities | `_read_index` |
| projections_epic_capabilities | `_read_tests` |
| projections_epic_capabilities | `_scan_modules` |
| projections_epic_capabilities | `extract` |
| projections_epic_capabilities | `render` |
| projections_epic_capabilities | `resolve_blueprint` |
| projections_epic_capabilities | `transform` |
| projections_epic_complexity | `ast_entropy` |
| projections_epic_complexity | `cyclomatic_complexity` |
| projections_epic_complexity | `detect_symptoms` |
| projections_epic_complexity | `extract` |
| projections_epic_complexity | `find_manual` |
| projections_epic_complexity | `module_metrics` |
| projections_epic_complexity | `param_count` |
| projections_epic_complexity | `parse_manual` |
| projections_epic_complexity | `render` |
| projections_epic_complexity | `transform` |
| projections_epic_concepts | `_module_exists` |
| projections_epic_concepts | `_parse_concept` |
| projections_epic_concepts | `_scan_code_grounding` |
| projections_epic_concepts | `_scan_implementations` |
| projections_epic_concepts | `_strip_concept_name` |
| projections_epic_concepts | `extract` |
| projections_epic_concepts | `render` |
| projections_epic_concepts | `transform` |
| projections_epic_design_patterns | `_header` |
| projections_epic_design_patterns | `_render_applied` |
| projections_epic_design_patterns | `_render_referenced` |
| projections_epic_design_patterns | `_render_unapplied` |
| projections_epic_design_patterns | `extract` |
| projections_epic_design_patterns | `parse_declarations` |
| projections_epic_design_patterns | `parse_design_pattern` |
| projections_epic_design_patterns | `parse_pattern_links` |
| projections_epic_design_patterns | `render` |
| projections_epic_design_patterns | `transform` |
| projections_epic_gradients | `extract` |
| projections_epic_gradients | `render` |
| projections_epic_gradients | `transform` |
| projections_epic_graph | `_build_file_index` |
| projections_epic_graph | `_is_valid_doc_name` |
| projections_epic_graph | `extract` |
| projections_epic_graph | `render` |
| projections_epic_graph | `transform` |
| projections_epic_issues | `extract` |
| projections_epic_issues | `render` |
| projections_epic_issues | `transform` |
| projections_epic_llm_status | `_agent_usage` |
| projections_epic_llm_status | `_endpoint_models` |
| projections_epic_llm_status | `_human_age` |
| projections_epic_llm_status | `_recent_usage` |
| projections_epic_llm_status | `_recovery_rows` |
| projections_epic_llm_status | `extract` |
| projections_epic_llm_status | `render` |
| projections_epic_llm_status | `transform` |
| projections_epic_orphans | `_calc_coverage` |
| projections_epic_orphans | `_collect_blueprints` |
| projections_epic_orphans | `_collect_code_modules` |
| projections_epic_orphans | `_collect_tests` |
| projections_epic_orphans | `_extract_module_from_blueprint` |
| projections_epic_orphans | `_extract_module_from_tests` |
| projections_epic_orphans | `_find_missing_blueprints` |
| projections_epic_orphans | `_find_orphan_blueprints` |
| projections_epic_orphans | `_find_orphan_tests` |
| projections_epic_orphans | `_module_to_code_path` |
| projections_epic_orphans | `extract` |
| projections_epic_orphans | `render` |
| projections_epic_orphans | `transform` |
| projections_epic_patterns | `_parse_pattern` |
| projections_epic_patterns | `extract` |
| projections_epic_patterns | `render` |
| projections_epic_patterns | `transform` |
| projections_epic_pool_views | `_entries` |
| projections_epic_pool_views | `extract` |
| projections_epic_pool_views | `generate` |
| projections_epic_pool_views | `render` |
| projections_epic_shaping | `_analyze_blueprint_traceability` |
| projections_epic_shaping | `_analyze_ontology_coverage` |
| projections_epic_shaping | `_collect_implementation_blueprints` |
| projections_epic_shaping | `_collect_ontology_concepts` |
| projections_epic_shaping | `extract` |
| projections_epic_shaping | `render` |
| projections_epic_shaping | `transform` |
| projections_epic_stories | `_parse_story` |
| projections_epic_stories | `_parse_test_status` |
| projections_epic_stories | `extract` |
| projections_epic_stories | `render` |
| projections_epic_stories | `transform` |
| projections_epic_story_views | `_completed_stories` |
| projections_epic_story_views | `extract` |
| projections_epic_story_views | `generate` |
| projections_epic_story_views | `render` |
| projections_epic_subepics | `_parse_subepic` |
| projections_epic_subepics | `extract` |
| projections_epic_subepics | `render` |
| projections_epic_trace | `extract` |
| projections_epic_trace | `generate` |
| projections_epic_trace | `render` |
| projections_epic_trace | `transform` |
| projections_epic_usage | `extract` |
| projections_epic_usage | `render` |
| projections_epic_usage | `transform` |
| projections_epic_viewlib | `git_activity_map` |
| projections_epic_viewlib | `list_rows` |
| projections_epic_viewlib | `load_pattern_sections` |
| projections_epic_viewlib | `parse_fields` |
| projections_epic_viewlib | `section_text` |
| projections_fragments | `definition_document_path` |
| projections_fragments | `update_definition_fragment` |
| projections_fragments | `update_projections_fragment` |
| projections_namespace_base | `generate` |
| projections_namespace_base | `instance_epic_dirs` |
| projections_namespace_base | `write` |
| projections_namespace_instance | `_conn` |
| projections_namespace_instance | `_cross_epic_usage` |
| projections_namespace_instance | `_display_remote` |
| projections_namespace_instance | `_document_counts` |
| projections_namespace_instance | `_fmt` |
| projections_namespace_instance | `_git_state` |
| projections_namespace_instance | `_identity` |
| projections_namespace_instance | `_is_git_repo` |
| projections_namespace_instance | `_open_issues` |
| projections_namespace_instance | `_remote_is_live` |
| projections_namespace_instance | `_render_cross_epic` |
| projections_namespace_instance | `_render_documents` |
| projections_namespace_instance | `_render_epics` |
| projections_namespace_instance | `_render_incomplete` |
| projections_namespace_instance | `_render_inventory` |
| projections_namespace_instance | `_render_open_issues` |
| projections_namespace_instance | `_render_stories` |
| projections_namespace_instance | `_render_structure_audit` |
| projections_namespace_instance | `_render_summary` |
| projections_namespace_instance | `_scan_epic` |
| projections_namespace_instance | `_scan_structure_audit` |
| projections_namespace_instance | `_story_status` |
| projections_namespace_instance | `extract` |
| projections_namespace_instance | `render` |
| projections_namespace_instance | `transform` |
| projections_namespace_issues | `_first_paragraph` |
| projections_namespace_issues | `_occurrence_rows` |
| projections_namespace_issues | `_render_lessons` |
| projections_namespace_issues | `_render_open` |
| projections_namespace_issues | `_render_recurring` |
| projections_namespace_issues | `_section` |
| projections_namespace_issues | `extract` |
| projections_namespace_issues | `parse_issue` |
| projections_namespace_issues | `render` |
| projections_namespace_issues | `transform` |
| projections_namespace_patterns | `extract` |
| projections_namespace_patterns | `parse_template` |
| projections_namespace_patterns | `render` |
| projections_namespace_patterns | `transform` |
| projections_registry | `generate_all` |
| projections_registry | `generate_scope` |
| projections_utility_inheritance | `_build_node` |
| projections_utility_inheritance | `_build_tree` |
| projections_utility_inheritance | `_find_epic_definition` |
| projections_utility_inheritance | `_parse_definition` |
| projections_utility_inheritance | `_render_node` |
| projections_utility_inheritance | `extract` |
| projections_utility_inheritance | `render` |
| projections_utility_validation | `_build_file_index` |
| projections_utility_validation | `_check_file` |
| projections_utility_validation | `_check_pattern_prefix` |
| projections_utility_validation | `_extract_filename` |
| projections_utility_validation | `_get_scan_root` |
| projections_utility_validation | `_should_include_file` |
| projections_utility_validation | `_validate_link` |
| projections_utility_validation | `extract` |
| projections_utility_validation | `render` |

### sensor-read

**Modules:** 2 | **Functions:** 32

| Module | Function |
|--------|----------|
| cli | `sensor` |
| cli | `sensor_list` |
| cli | `sensor_read` |
| sensors | `_cli_source_modules` |
| sensors | `_measure_execution_table` |
| sensors | `_shaping_coverage` |
| sensors | `_suite_import_subjects` |
| sensors | `get` |
| sensors | `knowledge_documents` |
| sensors | `list` |
| sensors | `load_readings` |
| sensors | `measure_all` |
| sensors | `measure_and_store` |
| sensors | `measure_bpcov` |
| sensors | `measure_bpfunc` |
| sensors | `measure_bptrace` |
| sensors | `measure_codeent` |
| sensors | `measure_concept_testcov` |
| sensors | `measure_depvalid` |
| sensors | `measure_epic_progress` |
| sensors | `measure_issue_rec` |
| sensors | `measure_karma` |
| sensors | `measure_know_chg_fresh` |
| sensors | `measure_know_use_fresh` |
| sensors | `measure_module_testcov` |
| sensors | `measure_ontcov` |
| sensors | `measure_patcov` |
| sensors | `measure_story_progress` |
| sensors | `measure_testpass` |
| sensors | `register` |
| sensors | `scan_issue_documents` |
| sensors | `store_readings` |

### story-tracking

**Modules:** 6 | **Functions:** 39

| Module | Function |
|--------|----------|
| config | `_check_definition_for_prefix` |
| config | `get_active_story` |
| config | `get_epic_for_story` |
| config | `get_story_pool` |
| config | `set_active_story` |
| counters | `allocate_story_id` |
| counters | `seed_from_stories` |
| hooks | `_check_concept_coverage` |
| hooks | `_find_story_file` |
| hooks | `_find_tracked_requirement` |
| hooks | `_format_ac_status` |
| hooks | `_format_checkpoint_status` |
| hooks | `_format_idle_status` |
| hooks | `_format_pattern_status` |
| hooks | `_format_requirements_status` |
| hooks | `_format_tracked_status` |
| hooks | `_generate_story_context` |
| hooks | `_get_done_story_instructions` |
| hooks | `_parse_phase_from_status` |
| hooks | `_parse_requirements` |
| hooks | `get_active_story_info` |
| hooks | `pause_active_story` |
| hooks | `resume_story_from_pool` |
| karma | `get_karma_per_author` |
| karma | `get_top_documents` |
| status | `get_llm_instruction` |
| status | `get_wiki_status` |
| story | `_build_version` |
| story | `_find_story_path` |
| story | `_get_last_epic_release` |
| story | `_get_last_release` |
| story | `_get_last_story_release` |
| story | `_get_story_target_path` |
| story | `_get_story_type_info` |
| story | `_get_subepic_from_config` |
| story | `_reconcile_active_pointer` |
| story | `story_create` |
| story | `story_reopen` |
| story | `story_switch` |

### template-rendering

**Modules:** 1 | **Functions:** 2

| Module | Function |
|--------|----------|
| bootstrap | `epic_identity` |
| bootstrap | `subepic_identity` |

### test-execution

**Modules:** 2 | **Functions:** 4

| Module | Function |
|--------|----------|
| hooks | `handle_tests_file_auto` |
| hooks | `needs_test_run` |
| test_runner | `run_test` |
| test_runner | `run_tests_from_file` |

### wiki-sync

**Modules:** 1 | **Functions:** 5

| Module | Function |
|--------|----------|
| wiki | `sync_document` |
| wiki | `wiki_clean` |
| wiki | `wiki_generate` |
| wiki | `wiki_group` |
| wiki | `wiki_sync` |

### wiki-validation

**Modules:** 1 | **Functions:** 4

| Module | Function |
|--------|----------|
| wiki | `find_duplicates` |
| wiki | `load_wiki_config` |
| wiki | `resolve_wiki_paths` |
| wiki | `wiki_check` |
