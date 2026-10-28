# GTM Repository / Context Architecture for Claude Code

Source: curated from Maja Voje / GTM Strategist LinkedIn content, including a "GTM Starter Kit" repo pattern and a Base Operations case study (CMO built an AI content system solo with Claude Code: organic traffic doubled in ~4 months, AEO citations up 500%+, ranked #1 for core terms within weeks).

**Core principle:** "A team running a chatbot starts from scratch every time. A team doing context engineering builds a brain." The skills/prompts aren't the moat — the accumulated, structured context is. "Upload your base intelligence once. It compounds from there."

Use this pattern when a user wants a durable GTM system in Claude Code instead of re-explaining their company in every chat. Offer to actually scaffold this folder structure for them (with real content, not placeholders) rather than just describing it.

## Folder structure

```
gtm-starter-kit/  (or gtm-context/, name it to taste)
├── CLAUDE.md                     ← "The Brain" — read automatically every session
├── context/                      ← institutional knowledge (source of truth)
│   ├── profile.md                — company overview, product, team, reference customers
│   ├── icp-definition.md         — ICP tiers, filters, anti-ICP, qualification criteria
│   ├── signal-library.md         — buying signals, scoring, detection methods, hooks
│   ├── positioning.md            — value pillars, competitive positioning, what NOT to say
│   ├── competitor-radar.md       — battlecards, win/loss patterns
│   └── personas/
│       └── template.md           — persona template, duplicate per buyer role
├── customer-intelligence/        ← optional but powerful
│   ├── transcripts/              — raw sales call transcripts go in
│   └── insights/                 — structured JSON extracted from transcripts (exact
│                                    customer quotes, pain triggers, urgency signals) —
│                                    this is what makes generated content sound like a
│                                    practitioner wrote it, not a marketing team
├── proof-library/
│   ├── case-studies/             — case studies with quantifiable metrics
│   └── use-cases/                — product capability demonstrations
├── sync/                         ← scripts pulling live data into the repo
│   ├── README.md                 — setup/usage
│   ├── .env.example              — API keys
│   └── sync-*.py                 — e.g. pull reply/meeting rates from an outbound tool,
│                                    aggregate signal performance across campaigns
├── skills/                       ← Claude executes these directly, one-line prompts
│   ├── setup/SKILL.md            — run first: give it a domain, it auto-populates the repo
│   ├── account-research/SKILL.md — deep research on any account before outreach
│   ├── signal-to-sequence/SKILL.md — turn a signal into a live outbound campaign
│   ├── icp-scoring/SKILL.md      — score a list of accounts against the ICP, assign tiers
│   └── weekly-update/SKILL.md    — keep context current, run Monday mornings
├── workflows/                    ← how the *team* operates (human process docs, not
│                                    for Claude to execute)
│   ├── enrichment.md             — data waterfall: free sources → paid enrichment →
│                                    proprietary data
│   ├── signal-routing.md         — decision tree: signal fires → what happens next
│   └── campaign-build.md         — end-to-end: audience → launch → measurement
├── playbooks/                    ← step-by-step for specific recurring situations
│   ├── new-signal-response.md    — signal fires: validate → score → research → send
│   └── competitor-switch.md      — scenarios: unknown / active eval / intent / locked in
├── outputs/                      ← archive, every skill run lands here
│   ├── scoring/                  — ICP scoring outputs
│   └── campaigns/                — campaign briefs and sequences
└── examples/
    └── sample-company/           — a fully worked example company for reference
```

## The Cascade Principle

Edit the master knowledge base (`context/profile.md` or a single `knowledge-base.md`) once, and every derived module (`icp.md`, `personas.md`, `positioning.md`, etc.) updates from it. Every skill/agent that reads those modules produces different output on its next run — without needing to be re-briefed. This is the whole point of the architecture: context compounds instead of being re-explained per session.

## The 5 functional layers (mental model)

1. **CLAUDE.md — The Brain.** Single file Claude reads automatically at the start of every session: ICP summary, top signals, positioning, team, current priorities. The persistent context layer everything else flows from. Keep it scannable in ~2 minutes.
2. **Context — Institutional Knowledge.** The structured files capturing GTM strategy: ICP tier definitions, signal libraries (ideally with decay curves — how stale a signal gets over time), competitive battlecards, messaging matrices, per-persona outreach hooks.
3. **Skills — Repeatable Execution.** Markdown files telling Claude exactly how to run a specific GTM task using the context above (account research briefs, full campaign builds, ICP scoring on a list of 500, weekly repo updates).
4. **Workflows — Connective Tissue.** Decision trees and process specs for the *humans* running the system (data waterfalls, signal routing logic, campaign approval gates, deliverability thresholds) — these are not meant for Claude to execute, they document how the team works around the system.
5. **Outputs — The Archive.** Every brief, campaign, and sequence produced lives here. Months of outputs alongside the context files that produced them create a feedback loop showing how the team's thinking evolved — useful for auditing what worked.

## Worked example: "Launch outbound campaign with ads retargeting"

- **Reads:** CLAUDE.md, client profiles, signal libraries, battlecards, meeting history
- **Runs:** account research skill → ICP scoring → signal-to-sequence build → campaign QA workflow
- **Writes:** research briefs, lookalike campaign specs, outbound sequences, retargeting audiences

When a user wants to go from "chatting with Claude about GTM" to "running a GTM system," this is the concrete structure to propose and help them build out — start with `CLAUDE.md` and one or two `context/` files (usually `icp-definition.md` and `positioning.md`), don't try to scaffold all of it empty on day one.
