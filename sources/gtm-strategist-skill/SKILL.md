---
name: gtm-strategist
description: Go-to-market strategy knowledge base — frameworks, prompts, checklists, and tool comparisons for B2B GTM work (ICP/ECP definition, positioning & messaging, launch planning, pricing, AEO/SEO for AI visibility, GTM tool stack choices, GTM repo/context architecture for Claude Code). Use this skill whenever the user asks about go-to-market strategy, ICP, positioning, messaging, launch plans, pricing frameworks, competitive battlecards, AEO ("how do I show up in ChatGPT/Perplexity"), or which GTM tools/stack to use — even if they don't say "GTM" explicitly (e.g. "help me define who I should be selling to", "write a cold email sequence", "how do I get AI to recommend my product"). Content curated from Maja Voje / GTM Strategist public LinkedIn material — apply the frameworks, don't just recite them.
---

# GTM Strategist

A reference knowledge base for go-to-market work: strategy, positioning, launch, pricing, AEO/SEO, and the GTM tool stack. All content here is curated from Maja Voje / GTM Strategist's public LinkedIn posts and infographics — treat it as a proven external framework to *apply*, not as Anthropic or the user's own research.

## Relationship to the 12 official GTM Strategist skills

This skill is a **quick-reference knowledge base** (frameworks, prompts, tool comparisons, checklists) synthesized from social-media content. It is complementary to, and distinct from, the **official 12-phase GTM Strategist skill set** (`gtm-foundations`, `collecting-intelligence`, `validating-customers`, `building-product`, `setting-pricing`, `crafting-positioning`, `preparing-launch-assets`, `building-communication-engine`, `executing-launch`, `building-gtm-system`, `running-marketing`, `executing-sales`) — the real, MIT-licensed skills from [github.com/GTM-Strategist/gtm-strategist-skills](https://github.com/GTM-Strategist/gtm-strategist-skills), also installed under `~/.claude/skills/`.

**When to use which:**
- The user wants a **quick answer, a specific prompt, a tool comparison, or a single framework applied to a specific question** → use *this* skill (`gtm-strategist`) and its reference files below.
- The user wants to **work through their actual GTM strategy step by step** (a full 90-day plan, sequential phases building on each other, saved outputs) → point them to the 12-phase skill set instead; each phase skill activates on its own (e.g. "help me with positioning" → `crafting-positioning` activates). Suggest they fill in `references/my-gtm-context-template.md` (or their own copy of it) first, since all 12 phase skills expect that product/market context to exist.
- Don't run both skill systems on the same request — pick the one that matches what the user is actually asking for.

## How to use this skill

Don't dump reference content back at the user. Figure out which stage of their GTM problem they're actually in, pull the relevant framework(s) from the reference files below, and apply them directly to their specifics — their product, their market, their numbers. If a framework needs inputs (an ICP, a competitor list, a call transcript), ask for them before running the framework blind.

Load only the reference file(s) relevant to the task — don't read all of them into context for a narrow question.

## Reference files

| File | Load when the user needs... |
|---|---|
| [references/frameworks.md](references/frameworks.md) | Core strategy frameworks: GTM Iceberg (7-layer stack), 4 mission-critical frameworks (Power Hour, Market Problem Map, Positioning 5-step, GTM Blueprint), ECP-before-ICP + 4-bracket qualification, Product-Market Fit Cycle, 3 Silent Killers of GTM orchestration, Beachhead/Chasm/Segment Prioritization/Validation Methods/Bullseye/GTM Motions, DMU buying-committee pyramid, ICP Voice Mining, Gap Ranking, Price Friction |
| [references/prompts.md](references/prompts.md) | 15 ready-to-adapt GTM prompts (cold start → heating up → on fire), for outreach, positioning, battlecards, content, case studies, sales decks, loss analysis |
| [references/aeo-seo.md](references/aeo-seo.md) | Answer Engine Optimization (AEO) — the 6-pillar framework and the 6-step AEO playbook, for "how do I show up when people ask AI for recommendations" |
| [references/repo-architecture.md](references/repo-architecture.md) | GTM context/repo architecture pattern for Claude Code — CLAUDE.md + context/ + skills/ + workflows/ + outputs/ — for when the user wants to build a durable GTM system instead of one-off chats |
| [references/tool-stack.md](references/tool-stack.md) | Tool comparisons and stack architecture: GTM AI tool wheel, 30-tool Q3 stack example, 17-tool GTM engineering venn, MCP integration map, Attio vs HubSpot, Swan AI vs Claude Code, 12 real-company Clay playbooks, AI model choice for design/content |
| [references/claude-workflows.md](references/claude-workflows.md) | Claude Code / Cowork / Chat usage for GTM — command cheat sheet, top 20 workflows other GTM operators run, when to use Chat vs Code vs Cowork, international GTM launch checklist, survival-kit resources (books, KPIs, newsletters) |
| [references/growth-loops.md](references/growth-loops.md) | Growth loop archetypes (referral, UGC, integration, retention, onboarding, viral, etc.) with real company examples, plus the 2026 shift toward GEO/influencers/affiliates/referrals/integrations as acquisition channels |
| [references/linkedin-playbook.md](references/linkedin-playbook.md) | LinkedIn as a GTM channel — the 5-second ICP relevance profile test, the 5 modes of LinkedIn GTM, the 7 LinkedIn playbooks from personal-network DMs to ABM/ads |
| [references/my-gtm-context-template.md](references/my-gtm-context-template.md) | The official GTM Strategist product/market context template — fill this in (or help the user fill it in) before running any of the 12 phase skills, since they all expect this context to exist |

## Quick triage

- **"Who should I sell to?"** → `frameworks.md` (ECP before ICP, 4-bracket qualification, DMU pyramid) + `prompts.md` prompt #1
- **"How do I position/differentiate?"** → `frameworks.md` (Positioning 5-step) + `prompts.md` prompts #4, #6, #7
- **"Write me outreach / a cold email / a post"** → `prompts.md` prompts #8–10
- **"We're not showing up in ChatGPT/AI search"** → `aeo-seo.md`
- **"What GTM tools should I use / should I use Attio or HubSpot / Clay or X / Swan or Claude Code"** → `tool-stack.md`
- **"Help me set up a GTM system in Claude Code, not just a chat"** → `repo-architecture.md`
- **"Planning a launch / entering a new market / going international"** → `claude-workflows.md` (international checklist) + `frameworks.md` (GTM Blueprint, Beachhead Strategy)
- **"Why did we lose this deal / analyze this call"** → `prompts.md` prompts #3, #14 + `frameworks.md` (ICP Voice Mining, DMU pyramid)
- **"Growth is stalling, should we do more ads/SEO?"** → `frameworks.md` (Product-Market Fit Cycle, The Chasm) — the real problem is often PMF, not demand-gen volume
- **"How do I get more referrals / build a growth loop / reduce CAC"** → `growth-loops.md`
- **"Help with my LinkedIn / personal brand / posting strategy"** → `linkedin-playbook.md`
- **"What should our channel mix / traction channels be"** → `frameworks.md` (Bullseye Framework, GTM Motions) + `growth-loops.md` (new acquisition channels)
- **"How do other GTM operators actually use Claude"** → `claude-workflows.md` (top 20 workflows)
