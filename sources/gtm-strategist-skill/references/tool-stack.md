# GTM Tool Stack & Comparisons

Source: curated from Maja Voje / GTM Strategist LinkedIn content. Use when a user asks "what tool should I use for X" or wants to compare specific GTM tools. Don't just list tools — tie the recommendation back to what stage/layer of GTM they're actually solving for (see [frameworks.md](frameworks.md) GTM Iceberg first if that hasn't been established).

## 4 Layers of the AI GTM Stack (mental model)

1. **AI/Reasoning ("the brain")** — Claude, ChatGPT, Gemini
2. **Context ("the memory")** — the ICP, signals, account history, voice (see [repo-architecture.md](repo-architecture.md))
3. **Orchestration ("the engine")** — right play, right trigger, account-by-account, at scale
4. **Specialist tools ("the hands")** — Data & Enrichment (Apollo, ZoomInfo), Delivery (Instantly, HeyReach), CRM (Salesforce, HubSpot)

Framing: "AI agents can now do the actual GTM work: research the account, write the outreach, score the lead, update the CRM." When a user is missing layer 2 (context) and jumps straight to layer 4 (tools), that's the GTM Iceberg failure mode again — flag it.

## The GTM AI Stack — Tool Wheel by Job-To-Be-Done

Organize AI/GTM tool recommendations by job category, not by hype:
- **GTM Agents**: Relevance AI, Gumloop, Clay, n8n, Lindy
- **Sales**: 1mind, Instantly, HeyReach, Attio, Apollo
- **Design**: Midjourney, Magnific, Figma, Framer, Recraft
- **Content**: Descript, Wispr Flow, ElevenLabs, Tella, Opus Clip
- **Development**: Claude Code, v0, Swan AI, Cursor, Lovable
- **Research**: NotebookLM, Exa, Ahrefs, Perplexity
- **Productivity**: Fireflies, Superhuman, ChatGPT, Granola, Notion
- **Foundation**: Claude, ChatGPT, Gmail, Google Calendar, Gemini, Google Drive, Miro, ClickUp

## GTM Engineering — 17 Tools Used by 500+ GTM Engineers

Organized around a central "build layer" (Claude Code, Cursor), in three categories with overlap zones:
- **Data & Signal**: Apollo, Clay, Apify, ZoomInfo, RB2B
- **RevOps & Orchestration**: HubSpot, n8n, Attio, Notion, Zapier
- **Outbound & Conversation**: Smartlead, Outreach, 11x, Instantly, HeyReach
- Overlap zones: "Enrichment & sync" (Data ∩ RevOps), "Trigger plays" (Data ∩ Outbound), "Pipeline routing" (RevOps ∩ Outbound)

## A Real Q3 GTM Stack Example (30 tools by JTBD, bottom-up pyramid)

Useful as a template for auditing a user's own stack layer by layer:
- **Business essentials** (where the work lives): Google Workspace, Trello, Slack, Claude, ChatGPT, Miro, accounting software
- **Productivity** (speed & leverage): Wispr Flow, Granola, n8n, Replit, Gamma
- **Inbound/content creation**: Tella, Ahrefs, Notion, Kit, Figma, Claude Code
- **Outbound/sales**: Exa, Attio, Clay, Swan AI, Apify, Claude Code
- **Digital products**: Zapier, Lemon Squeezy, Framer
- **Analytics**: Google Analytics, Microsoft Clarity
Note the periodic advice: "consolidate before expanding" — when a user's stack is sprawling, recommend a consolidation pass across these six layers before adding new tools.

## MCP Integration Map for Claude Code

Premise: "Agents got the hype. MCPs got the adoption." MCPs are the quiet infrastructure behind GTM systems built in Claude Code:
- **Productivity**: Google Calendar, Slack, Attio, Asana
- **Database**: Apollo, Supabase, Google Drive, Exa
- **Outreach**: Clay, Instantly, HeyReach, Lemlist
- **Content**: Miro, Canva, Firecrawl, Notion

## Attio vs. HubSpot (CRM choice)

| Attribute | Attio | HubSpot |
|---|---|---|
| Customizable | Fully | Limited |
| AI capabilities | Universal | Siloed |
| Call recording | Unlimited | Capped |
| Learning curve | Fast | Steeper |
| Free to start | Up to 3 seats | Up to 2 seats |
| Automations | All plans | From Pro |
| Integrations | 100+ apps | 1,700+ apps |
| Reporting | Growing | Advanced |

Rule of thumb: Attio for teams that want speed/customization and are comfortable with a smaller integration ecosystem; HubSpot for teams that need the largest integration marketplace and advanced reporting out of the box.

## Swan AI vs. Claude Code (for GTM automation)

| Dimension | Swan AI | Claude Code |
|---|---|---|
| Built for | Async GTM workflows | Real-time conversations |
| Triggering | Signal-based (intent, hiring, demos) | Manual/cron jobs |
| Email + LinkedIn sequencer | Native, built-in | Needs external tool |
| B2B data + signals | Marketplace built-in | Bring your own (via MCPs) |
| GTM context architecture | Pre-built files (ICP, scoring, per-sender) | Build from scratch (CLAUDE.md) |
| Team controls (B2B) | Built for teams | Solo-first |
| Credit visibility | Dashboards + limits, cost estimates upfront | Token usage, less visible until you hit a wall |
| Learning curve (non-eng) | Designed for GTM ops | Engineer-friendly |
| Skill marketplace | Curated experts (beta) | Open-source on GitHub |
| Output type | Data + actions | Data, actions, UI, apps |
| Entry price | ~$50/month | ~$20/month |

Rule of thumb: recommend Swan AI when the user is non-technical, wants GTM-specific plays out of the box, and values team-level cost visibility. Recommend Claude Code when the user (or someone on the team) is comfortable building `CLAUDE.md`/context files from scratch and wants full flexibility, including building actual UI/apps, not just data/actions.

### Example Swan AI plays (voice-prompted, no code)
1. **Website Visitor Identification & Follow-Up** — surfaces who's visiting the site and what they viewed, for targeted follow-up.
2. **GTM Engineer Hiring Trigger** — surfaces ICP-fit companies hiring GTM engineers (via Apify + LinkedIn Jobs), scored with an explanation of relevance.
3. **LinkedIn Mentions & Tag Tracking** — scrapes mentions LinkedIn's own notifications miss, drafts thank-you notes automatically.
4. **Lookalike List Generation** — fed a screenshot of past clients/partners, builds a lookalike prospect list.
5. **LinkedIn Trending Topic Detection** — flags what's currently hot in the user's space for early/first-comment opportunities, instead of commenting on a fixed list of profiles with diminishing returns.

## 12 Real-Company Clay Playbooks

Clay positioned not just as an enrichment tool but a GTM engineering platform. Each with the play type, mechanism, and reported result:

| Company | Play | Mechanism | Result |
|---|---|---|---|
| OpenAI | Enrichment Actions in Salesforce (inbound) | One-click enrichment native to CRM, mimics best sales reps | 2x enrichment |
| Vanta | Event-triggered outbound | Watches funding/CISO hires/SOC2 page changes, auto-IDs decision makers | 80%+ coverage |
| Rippling | Experiment Engine (outbound) | Iterate, scale what works, kill what doesn't | 2x cold email |
| Lovable | GTM Engineering (outbound) | Test small, validate, then scale | +50% meetings/rep |
| Figma | Orchestration Layer (PLG) | Salesforce records + Snowflake product intelligence turned into action | Better pipeline |
| Notion | Auto-vetting startup applicants (inbound) | Enriches/scores every applicant, team only reviews edge cases | 40% auto-approve |
| ElevenLabs | Auto-Scoring Play (inbound) | Every lead pre-qualified, scored, routed | +50% SQLs |
| Intercom | Niche signals to find ICP (outbound) | Targeted by support-team size + hiring patterns when launching Fin | +140% pipeline |
| Mistral AI | Global GTM engine (outbound) | TAM mapping/account sourcing — 3-month analysis done in 3 days | 25K+ accounts |
| Sendoso | Outbound productivity boost | Enrichment, signal capture, CRM sync, personalization, automation | $1M+ pipeline |
| Anthropic | Consolidation Play (inbound) | Unique segmentation, conditional upsert into Salesforce | 3x enrichment |
| Verkada | Geo Expansion Play (outbound) | 28 European countries, each with its own tested/ramped GTM | 10x faster experiments |

Use this table to pattern-match a user's situation (inbound vs outbound, PLG vs sales-led, geo-expansion) to the closest real-company play rather than starting from a blank page.

## Choosing between Claude Chat, Claude Code, and Claude Cowork for GTM

See [claude-workflows.md](claude-workflows.md) for the full comparison and the top-20 workflow adoption data.

## AI Model Choice for GTM Design/Content Tasks

From a side-by-side test of the same design brief across 6 AI models — useful as a rough prior, not gospel, since model capabilities shift fast:
- **ChatGPT** — strong blend of creative + real research/microcopy, can run dense
- **Claude Code (agentic)** — pulled brand context on its own even with a neutral brief, produced near-final output — best default for a user with an existing brand-context repo
- **Claude in chat** — most disciplined, follows the brief literally, clean and well-synthesized, best for simple educational visuals
- **Gemini** — flashy/creative but prone to wandering from the actual brief
- **Mistral** — basic, gets the job done, no distinctiveness
- **GLM-4.x (Chinese model)** — can produce a surprisingly coherent layout, but flag real data-privacy risk — keep sensitive company/customer info out of prompts sent to it
Recommendation for regular GTM design/content work: an agentic coding tool (like Claude Code) wired into the user's actual brand context outperforms one-off chat prompts to a general model.
