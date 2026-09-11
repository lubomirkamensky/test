# test Usage

> Generated: 2026-09-11 19:17

Prune evidence for the Shaping cycle (measure twice, cut once):
the CLI names candidates deterministically; proposing and
confirming a Prune is LLM+Human.

## Summary

- Documents: 3
- Fresh: 0 · Aging: 0 · Stale: 0 · Unused: 3
- **Prune candidates: 3** (unused + stale)

## Documents

| Document | Karma | Last used | Changed | Signal |
|----------|-------|-----------|---------|--------|
| [TEST](TEST) | 0 | - | 0d | unused |
| [TEST-0001](TEST-0001) | 0 | - | 0d | unused |
| [TEST-SANDBOX](TEST-SANDBOX) | 0 | - | 0d | unused |

## Signals

- `unused` - no usage record: Prune candidate
- `stale` - last used > 90 days: Prune candidate (with Sustain check)
- `aging` - last used 31-90 days
- `fresh` - last used <= 30 days

A document stale for a long time in usage AND unchanged in git is
the stronger candidate; pair the two freshness columns when reviewing.

## Sources

- [ontology-shaping-blueprint](ontology-shaping-blueprint) - Prune mode, measure twice cut once
- [implementation-cli-projections_epic_usage-blueprint](implementation-cli-projections_epic_usage-blueprint) - this projection's design
- [implementation-cli-sensors-blueprint](implementation-cli-sensors-blueprint) - sensor registry consumed here
- [implementation-cli-gradient-metrics-blueprint](implementation-cli-gradient-metrics-blueprint) - Karma, KnowUseFresh, KnowChgFresh