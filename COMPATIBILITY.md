# Source compatibility notes

Original files remain byte-for-byte unchanged. Apply these integration rules only when reading them through the unified entry point.

## Prior-output aliases

These are content lookup aliases, not files to create or rename. Prefer an existing equivalent artifact and record its real filename. Do not claim a document exists merely because an alias is listed.

| Name used by a later phase | Actual originating artifact |
|---|---|
| `01-ope-canvas.md` | `01-one-page-endgame.md` |
| `01-value-proposition.md` | `01-value-proposition-canvas.md` |
| `01-90-day-plan.md` | `01-90-day-gtm-plan.md` |
| `03-validated-persona.md`, `03-icp-profile.md` | `03-customer-archetype.md` |
| `04-jtbd-analysis.md` | `04-jtbd-value-proposition.md` |
| `05-pricing-model.md`, `05-pricing-strategy.md` | Review `05-pricing-hypothesis.md`, `05-offers.md`, and `05-business-model.md` together |
| `06-messaging-framework.md` | `06-messaging-house.md` |
| `08-channel-strategy.md` | `08-channel-selection.md`, with `08-gtm-motions.md` and `08-funnel-projection.md` where needed |
| `08-social-proof-plan.md` | `08-social-proof-collection.md` |
| `09-launch-plan.md` | `09-launch-execution-summary.md`, with the relevant Phase 9 preparation artifacts |
| `09-launch-retrospective.md`, `10-gtm-retrospective.md` | `10-launch-retrospective.md` |

Phase 12 Task 1 refers to positioning as Phase 4 and messaging as Phase 5. Both belong to Phase 6: use `06-positioning-statement.md` and `06-messaging-house.md`.

## Counts and framework variants

The official README advertises 100 tasks; its table and actual numbered headings both total 100. Five official communication motions and seven curated motion categories are alternative taxonomies. Do not silently combine scores across them. The two context templates have the same Git blob hash; use one working copy. Framework abbreviations and explanatory wording can differ: use the definition in the active official task and label supplementary interpretations.

## Host behavior

The archived official repository targets Claude; its installation instructions and plugin manifest are preserved as source documentation. The unified entry point uses readable Markdown references and does not require those archived skills to be separately installed. Automatic file synchronization, recurring updates, tool access, and nested skill invocation require actual host capabilities and configuration; the reference architecture alone does not implement them.
