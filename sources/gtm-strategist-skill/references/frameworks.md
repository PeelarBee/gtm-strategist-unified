# Core GTM Frameworks

Source: curated from Maja Voje / GTM Strategist public LinkedIn content.

## The GTM Iceberg — 7-Layer Tool Stack

Most GTM teams only see and obsess over the visible tip (execution/tactics). The six layers beneath determine whether execution actually works. "Tools amplify strategy. They don't create it."

Bottom-up, the layers are:

1. **Strategy** — alignment before motion. Get the team pointed at the same objective before anyone touches a tool. (Example tools: Miro, Notion, Claude)
2. **Market** — find where you're a painkiller, not a vitamin. Understand what's actually changing in the category before you build anything. (Perplexity, SparkToro, Similarweb, Crunchbase, G2, Google Trends)
3. **Early Customer Profile (ECP)** — the buyers saying "shut up and take my money" *today*, not your eventual ideal customer. (LinkedIn Sales Navigator, user interviews, Granola, Common Room, Typeform)
4. **Product** — build in iteration, not in isolation. (Lovable, Claude Code, Figma, Amplitude, PostHog, Microsoft Clarity)
5. **Pricing** — willingness to pay, not guesswork. (Paddle, Stripe, ChartMogul, Schematic)
6. **Positioning & Messaging** — in a sea of AI sameness, differentiation isn't optional. (Wynter, Klue, Crayon, Gong, UserEvidence)
7. **GTM System** — growth loops and compounding engines: outbound, inbound, ads, ABM, automation. (Clay, Attio, HubSpot, Ahrefs, Instantly.ai, n8n)

**The failure mode this framework warns against:** "That's how teams end up scaling a value prop nobody validated. Automating outreach to an ICP nobody defined. Buying distribution for positioning nobody tested."

**Rule of thumb:** get the foundations aligned first (layers 1-3), then the stack starts compounding. Strategy before tactics, always. If a user asks "what tool should I use for X" without having answered layers 1-3 for their business, flag that before recommending tools.

---

## The 4 Mission-Critical GTM Frameworks

Used across thousands of companies. Apply whichever matches the user's current stage.

### 1. GTM Power Hour
A rapid workshop format to align a team on go-to-market direction in one sitting. Use cases differ by stage:
- **Pre-Product-Market Fit** — validate the problem and early customer profile
- **Product-Market Fit** — nail positioning and the initial GTM motion
- **Post-Product-Market Fit** — scale the system (CRM, growth loops, channel mix)

When running this with a user, start by identifying which of the three stages they're in — the workshop's focus changes completely.

### 2. Market Problem Map
A structured way to map and score market pain points before building anything. Mechanics: list every pain point/problem you hear from prospects or research, then score/rank each one by frequency and severity (e.g. how many interviews mentioned it, how painful it is). Prioritize building/positioning around the highest-scoring problems, not the loudest one or the first one heard.

### 3. Positioning & Messaging — 5-Step Flow
1. **Map competitive alternatives** — what does your ICP actually use instead of you today (including "do nothing" and spreadsheets)? How do they judge those alternatives?
2. **Score customer satisfaction** — for each alternative, where are customers already dissatisfied? That's where you can genuinely win — don't compete where incumbents are strong.
3. **Map your competitive assets** — list your capabilities, then filter out table stakes (things every alternative also has). Keep only what actually differentiates.
4. **Benefits + proof points** — for every claim/benefit you plan to make, attach a proof point (data, case study, demo) that backs it up. Never claim a benefit you can't back up.
5. **Land your first positioning** — synthesize into a value proposition + 3 key benefits (each with a differentiator + proof point from steps 3-4).

This feeds directly into: landing page copy, sales decks, content strategy, and AI/context engineering (i.e., this is also what should go in a `positioning.md` context file — see [repo-architecture.md](repo-architecture.md)).

### 4. GTM Blueprint
An end-to-end GTM plan and roadmap format — the container that the other three frameworks feed into. Use it as the top-level plan structure when a user asks for "a GTM plan" broadly rather than one specific piece (positioning, pricing, etc).

---

## ECP Before ICP

**Principle:** "You don't earn the right to chase your Ideal Customer Profile (ICP) until you've won your Early Customer Profile (ECP) first."

Why: regulated enterprises and late-majority buyers want case studies you don't have yet. Early adopters, by contrast, want to co-design with you and will tolerate rough edges. "You'll run out of runway talking to your ICP. ECP first." — when a user with an early-stage product asks to define their "ideal customer," redirect them to defining who will buy *today*, not who they'll eventually want.

### Qualify in Four Brackets
When scoring or defining a customer profile (ECP or ICP), score across all four, not just firmographics:
1. **Firmographics** — company size, industry, geography, tech stack
2. **Behaviors** — what they're doing that signals fit (content consumed, tools used, hiring patterns)
3. **Timing and momentum** — trigger events, why now (funding, leadership change, compliance deadline)
4. **Revenue potential** — deal size, expansion potential, LTV

**Method:** reverse-engineer the weighting from actual traction, not theory. Pull the 10 best current clients and ask "which of these do I want 500 more of?" — that answer defines the real ICP.

**Warning — don't build your ICP around "snow leopards":** rare, prestigious, but unrepresentative clients (e.g. one huge logo that took a fluke to land) will skew the profile and send the team chasing an unreplicable pattern.

---

## The Product-Market Fit Cycle

(Adapted from Carlos Eduardo Espinal's "Product/Market Fit Cycle.") Use this whenever a demand-gen or growth problem might actually be a PMF problem in disguise — e.g. "signups are declining, should we spend more on ads/SEO?" The instinctive answer (more top-of-funnel) is often wrong; the cycle exists to force a check further upstream first.

**Cycle:**
```
START: Big Vision → Product Hypothesis
  → IDENTIFY: Beachhead Segment (Minimum Viable Segment)
  → CREATE: Minimum Viable Business (MVB)
  → BUILD: Minimum Viable Product (MVP)
  → Test → Analyze (pick key metrics) → Learn → "Did it work?"
```
- **If NO:** loop back, but tag *why* it failed and route to the matching stage:
  - "Problem with Product" → back to Product Hypothesis
  - "Problem with Segment" → back to Beachhead Segment
  - "Problem with Business" → back to Minimum Viable Business
- **If YES:** FINISH — PMF proven for this scope, loop back to Big Vision to restart the cycle at a bigger scale (next segment, next product line).

When a user brings a growth-decline problem, ask: has anything upstream (segment, product, business model) shifted, or is this a pure top-of-funnel volume problem? Don't default to "more ads" without checking.

---

## The 3 Silent Killers of GTM Orchestration

Applies to outbound/nurture systems that operate at the *account* level instead of the *contact* level.

- **Killer 1 — Fake Personalization:** nurture treats every buyer at an account like one person; firmographic-based "personalization" (company size, industry) is not real personalization. **Fix:** branch messaging by individual behavior, not company data.
- **Killer 2 — Latency:** buyer signals get rolled up to the account level before anyone acts, so by the time sales sees it the buyer has moved on. **Fix:** build systems that act the moment an individual signal fires, not on a batch/rollup cadence.
- **Killer 3 — False Attribution:** CRMs credit the last touch, dashboards credit the loudest channel — neither identifies who actually moved the deal. **Fix:** track and credit the person/action that moved the deal, not just the channel it came through.

**Supporting framework — "Same deal, 5 people, 5 different priorities"** (50%+ of B2B deals involve 5+ buyers, each caring about something different):
| Buyer | Cares about |
|---|---|
| VP Sales | Pipeline velocity |
| Head of Ops | How it fits the existing stack |
| CFO | ROI & total cost |
| End User | Ease of use |
| IT/Security | Compliance & risk |

Sending all five the same generic nurture email means at most one of them finds it relevant. When designing outbound/nurture for a user, ask who the buying committee actually is and tailor per role — don't assume one persona.

---

## Segmentation & Market-Entry Frameworks

### Beachhead Strategy
"Spray-and-Pray" (attack every segment at once, weak everywhere) vs. **Beachhead** (concentrate on one segment first). Sequence: **Wave 1** — win one Beachhead Segment completely → **Wave 2** — expand to adjacent markets using the credibility/patterns from Wave 1 → **Wave 3** — conquer other segments. Strength of GTM effort compounds wave over wave instead of diluting across all of them at once. Use this whenever a user wants to "go after everyone" out of the gate — redirect them to picking one beachhead first.

### The Chasm
Classic tech-adoption curve, useful for diagnosing *which* GTM problem a company actually has: Innovators → Early Adopters → **[The Chasm]** → Early Majority → Late Majority → Laggards, mapped against a Peak of Inflated Expectations → Plateau of Productivity hype curve. Early-stage GTM work (positioning, ECP, PMF) happens on the near side of the chasm; growth-stage work (scaling channels, expanding segments) happens on the far side. A company still trying to cross the chasm needs PMF/ECP work, not more growth-stage tactics like paid channels or ABM.

### Segment Prioritization
An inverted-funnel warning about segment count:
- **Too Broad** — many diverging segments → no pattern emerges in results, resources spread thin
- **Sweet Spot** — 3 to 5 segments → enough signal to see patterns, still focused enough to execute
- **Too Narrow** — too few segments → missed opportunities, risk of over-indexing on one profile
When helping a user prioritize segments, push them toward 3-5 — flag if they're listing 10+ (too broad) or fixating on exactly one (too narrow, unless that's a deliberate beachhead-stage choice).

### Validation Methods (by confidence & product completeness)
Ordered from low-confidence/early-stage to high-confidence/late-stage:
1. Interviews
2. Surveys
3. Solution testing
4. Marketing tests (landing pages, ad tests)
5. Waitlists
6. Co-creation with a client
7. Presale
8. Testing MVP
Match the validation method to how much product actually exists — don't run a presale before you've done interviews, and don't stop at interviews once an MVP exists.

### The Bullseye Framework (finding traction channels)
1. Place your top 3 candidate channels in the center (bullseye)
2. Place your next 6 candidate channels in the middle layer
3. Test, then redo the placement based on real results — channels move rings based on evidence, not opinion
Use this to structure a channel-prioritization exercise rather than trying every channel simultaneously.

### GTM Motions (7 types)
| Motion | Growth lever | Example tools |
|---|---|---|
| Inbound | Content creation to generate leads | LinkedIn, SEMRUSH, Grammarly |
| Outbound | Cold outreach via email/social/phone | LinkedIn, ZoomInfo, Lemlist |
| Paid Digital | Media buying to capture attention | Google Ads, Meta Ads, Newswire |
| Community | Engaging/creating content for community members | Slack, Reddit, Discord |
| Partners | Collaborating with compatible companies | Miro, AWS Startups, Oracle |
| Account-Based Marketing (ABM) | Targeting high-value accounts with personalized campaigns | Pipedrive, Hunter, Clay |
| Product-Led Growth (PLG) | Self-onboarding, early value realization | Hotjar, Amplitude |
A GTM plan usually blends 2-3 of these, not all 7 — help the user pick based on deal size and buyer sophistication (PLG/inbound for low-touch, ABM/outbound for high-touch enterprise).

---

## Buying Committee & Call-Mining Frameworks

### Go-to-Market Decision Making Unit (DMU) — "Champ vs. Block"
A pyramid of roles in a B2B buying committee, top to bottom:
- **Decision Maker** (e.g. CEO) — top of pyramid, final call
- **Economic Buyer** (e.g. CFO) — controls budget
- **Initiation layer** (Researchers/R&D, Product Managers, CTO, Head of Division) — surfaces and vets the need
- **End User** (Head of Office, R&D, Product Managers) — base of pyramid, uses the product day to day
- **External Business Consultant** — an Influencer positioned outside the core pyramid
When mapping a deal, identify who in the account occupies each role — a champion at the End User layer without Economic Buyer sponsorship is a common reason deals stall ("Champ vs Block").

### ICP Voice Mining (from call recordings)
A pipeline for turning raw sales call language into usable messaging assets:
Positioning Statement → Strategic layer (USPs, Problem/Solution) → Tactical layer (key messages per Customer Profile, key messages per Customer Journey Stage) → Messaging Guidelines → Applied layer (Promotional Copy: website/ads/flyers/pitch decks; Core Copy: product messages, onboarding, support) → Channels (LinkedIn, in-app, mobile).
When a user has sales call transcripts available, mine them in this order rather than jumping straight to "write me messaging" — the strategic layer (USPs, problem/solution fit) needs to be extracted from real call language first.

### Gap Ranking (prioritization 2x2)
A value-vs-effort grid with four quadrants: **Do it now** (high value, low effort), **Do it if/when there's time** (lower priority), **Don't do it** (low value), evaluated against candidate GTM tactics (e.g. search ads, automated LinkedIn outreach, CRM setup, referral programs, podcast sponsorship, affiliate programs). Use this to triage a long list of "things we could do" into an actual priority order.

### Price Friction (Van Westendorp-style)
A price-sensitivity model plotting "Too Cheap / Not Expensive" against "Not a Bargain / Too Expensive" to find a **Range of Acceptable Prices**, bounded by:
- **PMC** (Point of Marginal Cheapness) — below this, price signals low quality
- **OPP** (Optimal Price Point) — where the curves cross
- **PME** (Point of Marginal Expensiveness) — above this, price kills conversion
When a user asks for pricing help without willingness-to-pay data, suggest running this kind of survey (ask "at what price would this be so cheap you'd question quality?" and "so expensive you wouldn't consider it?") before picking a number.
