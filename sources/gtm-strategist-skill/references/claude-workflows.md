# Using Claude for GTM: Workflows, Commands & Resources

Source: curated from Maja Voje / GTM Strategist LinkedIn content, including the "2026 Claude for GTM Pulse Report" (Poyar & Voje, N=200 GTM operators).

## Chat vs. Code vs. Cowork — when to use which

| Surface | Positioning | Best for |
|---|---|---|
| **Claude (Chat)** | "Think & Write" — conversational, no setup | Strategic thinking partner: brainstorming, analysis, writing |
| **Claude Code** (CLI/Terminal) | "Build & Automate" — autonomous coding agent, reads systems/writes code/executes | Building GTM infrastructure (see [repo-architecture.md](repo-architecture.md)) |
| **Claude Cowork** (Desktop app) | "Operate & Organize" — desktop agent for non-developers, file access/task execution without code | Getting operational work done without needing to code |

When a user asks "should I use Claude Code or just chat," ask whether they want a durable, repeatable system (→ Code, build the context repo) or a one-off analysis/output (→ Chat is enough).

## Top 20 GTM Workflows (2026 Claude for GTM Pulse Report, % of operators using each)

1. Creating social media posts — 27%
2. Building websites and landing pages — 20%
3. Building tools for SDRs — 18%
4. Adapting messaging by segment — 16%
5. Structured content pipelines — 16%
6. Signal-based outbound sequences — 15%
7. Creating custom ICP filters — 14%
8. Automating GTM engines — 13%
9. Building trigger-based prospect lists — 13%
10. Running competitor analysis or battlecards — 12%
11. Analyzing data from external systems — 12%
12. Auditing SEO performance — 12%
13. Analyzing traffic data / content performance — 12%
14. Creating "why now" angles tied to signals — 11%
15. Merging and cleaning data for list building — 11%
16. Identifying or honing ICPs — 10%
17. Creating or editing docs, presentations — 10%
18. Scraping niche sources for lists — 9%
19. Preparing for meetings — 8%
20. Drafting emails or Slack messages — 8%

**Key findings from the survey:**
- Cowork vs. Code adoption is close to a 50/50 split — they are not substitutes for each other (one operator replaced 3 VAs with Cowork; others run full GTM systems in Code).
- 80% use Claude for productivity, but the *impact* lives elsewhere: content creation (29%) and GTM engines (23%) deliver the biggest results — productivity tasks are just the entry point most teams never get past. If a user is stuck doing only scheduling/note-taking with Claude, point them toward content/GTM-engine workflows for bigger ROI.
- The best builders don't use Claude solo — they wire it into a stack (Clay, CRMs, other models). "Claude alone is a tool. Claude inside a stack is a system."
- 92% saved time, but only 67% built a workflow that was previously impossible, and only 27% have replaced a GTM tool outright so far — set realistic expectations with users about where the real step-change is (new capability) vs. incremental (time saved).
- Even $100-200/month plan users hit credit walls 2-3x a day; common frustrations include memory loss between sessions, integration gaps, and no easy skill-sharing across a team. If a user complains about hitting usage limits, that's a known, common pain point, not a sign they're doing something wrong.

## Claude Code Command Cheat Sheet (for GTM operators)

| Command / shortcut | What it does |
|---|---|
| `/init` | Sets up a `CLAUDE.md` file — put ICP, voice rules, and priorities there; Claude reads it every session |
| `/resume` | Picks up a past chat where you left off |
| Drag & drop image (or Ctrl+V) | Shows Claude a screenshot, slide, or profile |
| `@filename` | Pulls a specific file into the conversation |
| `/clear` | Wipes the conversation — do this after each task so context stays clean |
| `/compact` | Summarizes a long session to free up context while keeping the thread |
| `/mcp` | Manage MCP servers — connect tools like Clay, Attio, Miro |
| `/[skill name]` | Invoke a specific skill (Claude usually auto-identifies when one applies) |
| Shift+Tab or `/plan` | Enter Plan Mode — get a plan before Claude touches anything |
| Ctrl+B | Move a task to the background, get notified when done |
| `/model` | Switch models: Opus for demanding tasks, Sonnet for regular work, Haiku for repetitive work |
| `/usage` | Shows usage and spend |
| Esc | Stop the current task |
| Esc Esc | Edit the previous message instead of restarting the conversation |

**Terminal basics** (for non-engineers new to Claude Code): `pwd` (which folder am I in), `ls` (list files/folders), `Ctrl+C` (cancel a running command), `cd ..` (go up one level), `cd foldername` (go into a folder), `open .` (open current folder in Finder), `Tab` (autocomplete file/folder names), `↑` (recall last command), dragging a folder onto the terminal window auto-pastes its full path, `claude` (start a Claude Code session in the current folder).

## International GTM Launch Checklist

Premise: a translated homepage + ads is not a GTM plan. "The translation was fine, the GTM plan didn't exist." Before launching in a new market/language, answer:
- Is there real demand in this market?
- What channels do local B2B buyers actually use? (LinkedIn isn't the answer everywhere)
- What legislation kicks in the moment you're doing business with buyers there?
- What proof points travel across borders, and which ones don't?

**Plan components:**
1. Demand validation checklists (run before committing budget, not after)
2. A localization decision matrix — what to translate now vs. what can wait
3. Channel strategy by region
4. A campaign brief for the first localized launch
5. A monthly tracking framework per market

**How to use:** duplicate as a living planner → customize per market/goals → share with the team to align and track progress, don't treat it as a one-time document. See [aeo-seo.md](aeo-seo.md) for the localization-as-AEO-lever angle (English is native to only 10-15% of the world).

## GTM Strategist "Survival Kit" — curated resources

**Books:** *Go-To-Market Strategist* (Maja Voje), *Playing to Win* (A.G. Lafley & Roger Martin), *Experimentation Works* (Stefan Thomke), *Obviously Awesome* (April Dunford), *Monetizing Innovation* (Madhavan Ramanujam & Georg Tacke), *Lean Analytics* (Alistair Croll & Ben Yoskovitz).

**The 80/20 Focus Rule:** 80% double down on what's already working, 20% reserved for new experiments. "Stop chasing every shiny object. Focus is the edge." — a useful gut-check when a user wants to add yet another channel/tool instead of doubling down on what's already working.

**GTM Must-Have KPIs (by category):**
- GTM Efficiency (North Star): NRR, GRR, logo churn
- Revenue Health: pipeline coverage, win rate, CAC payback, cycle length
- Activation: time-to-first-value, trial-to-paid, feature adoption
- 2026 Signals: AI sentiment/AEO, sales velocity, AI workflow coverage

**GTM Claude Skills worth building** (mirrors the [repo-architecture.md](repo-architecture.md) pattern): Crafting Positioning, Setting Pricing (willingness-to-pay research, packaging), Executing Sales (deck, outbound, ABM), Running Marketing (narrative, content, paid, community), Validating Customers (ICP + persona via experiments).

## Newsletters worth following (for staying current on GTM/AI)

- **Learn GTM & AI:** The Product Compass (Paweł Huryn), Lenny's Newsletter (Lenny Rachitsky), How to AI (Ruben Hassid), GTM AI Podcast & Newsletter (Jonathan M Kvarfordt)
- **PLG:** Growth Unhinged (Kyle Poyar), Elena's Growth Scoop (Elena Verna), MKT1 Newsletter (Emily Kramer), GTMnow (Sophie Buonassisi)
- **RevOps & ABM:** Outbound Kitchen (Elric Legloire), The Revenue Leadership (Kyle Norton), Full-Funnel (Andrei Zinkevich & Vladimir Blagojević), Adam's GTM Report (Adam Schoenfeld)
- **Get it Done:** Dear Stage 2 (Liz Christo & Mandy Cole), The Signal (Brendan Short), The Workflow (Sara Stella Lattanzio & Diandra Escobar), GTM Strategist (Maja Voje)
- **Stay in the Loop:** GTM Engineering School (Matteo Tittarelli & Jared Waxman), Startup Riders (Ivan Landabaso), Cannonball GTM (Jordan Crawford & Doug Bell), GTM Monday (GTM Partners)

Only surface this list if the user is explicitly looking for people/newsletters to follow — it's a resource pointer, not something to recite unprompted.
