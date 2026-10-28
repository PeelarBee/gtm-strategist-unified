---
name: gtm-strategist-unified
description: Develop industry-agnostic go-to-market strategy and deliverables using a connected 12-phase workflow and curated reference library. Use for customer research, ICP, product, pricing, positioning, launch, growth, marketing, sales, or a focused GTM framework question.
---

# Unified Go to Market Agent

This is the reusable general core. Do not assume an industry, business model, jurisdiction, company, buyer or product. Establish the actual context and adapt the task to it. Industry-specific requirements belong to separately supplied extensions, not this default workflow.

## Start a request

Read the active project's `my-gtm-context.md` and relevant prior `outputs/`. Source-workflow context/output paths refer to that active project, never to the archived `sources/` tree. If no context exists, use the supplied [context template](sources/gtm-strategist-skills-official/my-gtm-context.md) to interview for task-critical inputs and save answers when supported. Never invent context or require irrelevant fields.

Choose the smallest mode that satisfies the request:

- **Guided workflow:** for a GTM deliverable or sequential project, read the relevant official phase below and only supporting reference sections needed. Follow the selected task's deliverable and filename, one task at a time. Build on evidence and identify assumptions where prior phases are skipped.
- **Focused reference:** for an explanation, prompt, comparison or narrow applied framework, read the relevant [library file](LIBRARY.md), apply it to the supplied facts, and keep the response proportionate. Do not trigger an entire project for a definition.
- **Short working session:** establish product, buyer, stage, goal and evidence; select one decision; produce one draft and next validation action. Do not claim a brief session established customer validation.

## General workflow and library map

| Phase | Official workflow | Tasks | Supporting library |
|---|---|---:|---|
| 1 | [gtm-foundations](sources/gtm-strategist-skills-official/.claude/skills/gtm-foundations/SKILL.md) | 11 | [frameworks](sources/gtm-strategist-skill/references/frameworks.md), [linkedin-playbook](sources/gtm-strategist-skill/references/linkedin-playbook.md) |
| 2 | [collecting-intelligence](sources/gtm-strategist-skills-official/.claude/skills/collecting-intelligence/SKILL.md) | 9 | [frameworks](sources/gtm-strategist-skill/references/frameworks.md), [prompts](sources/gtm-strategist-skill/references/prompts.md) |
| 3 | [validating-customers](sources/gtm-strategist-skills-official/.claude/skills/validating-customers/SKILL.md) | 7 | [frameworks](sources/gtm-strategist-skill/references/frameworks.md), [prompts](sources/gtm-strategist-skill/references/prompts.md) |
| 4 | [building-product](sources/gtm-strategist-skills-official/.claude/skills/building-product/SKILL.md) | 9 | [frameworks](sources/gtm-strategist-skill/references/frameworks.md) |
| 5 | [setting-pricing](sources/gtm-strategist-skills-official/.claude/skills/setting-pricing/SKILL.md) | 7 | [frameworks](sources/gtm-strategist-skill/references/frameworks.md) |
| 6 | [crafting-positioning](sources/gtm-strategist-skills-official/.claude/skills/crafting-positioning/SKILL.md) | 5 | [frameworks](sources/gtm-strategist-skill/references/frameworks.md), [prompts](sources/gtm-strategist-skill/references/prompts.md) |
| 7 | [preparing-launch-assets](sources/gtm-strategist-skills-official/.claude/skills/preparing-launch-assets/SKILL.md) | 6 | [aeo-seo](sources/gtm-strategist-skill/references/aeo-seo.md), [prompts](sources/gtm-strategist-skill/references/prompts.md) |
| 8 | [building-communication-engine](sources/gtm-strategist-skills-official/.claude/skills/building-communication-engine/SKILL.md) | 9 | [frameworks](sources/gtm-strategist-skill/references/frameworks.md), [linkedin-playbook](sources/gtm-strategist-skill/references/linkedin-playbook.md), [growth-loops](sources/gtm-strategist-skill/references/growth-loops.md) |
| 9 | [executing-launch](sources/gtm-strategist-skills-official/.claude/skills/executing-launch/SKILL.md) | 7 | [claude-workflows](sources/gtm-strategist-skill/references/claude-workflows.md), [prompts](sources/gtm-strategist-skill/references/prompts.md) |
| 10 | [building-gtm-system](sources/gtm-strategist-skills-official/.claude/skills/building-gtm-system/SKILL.md) | 9 | [repo-architecture](sources/gtm-strategist-skill/references/repo-architecture.md), [tool-stack](sources/gtm-strategist-skill/references/tool-stack.md), [growth-loops](sources/gtm-strategist-skill/references/growth-loops.md), [claude-workflows](sources/gtm-strategist-skill/references/claude-workflows.md) |
| 11 | [running-marketing](sources/gtm-strategist-skills-official/.claude/skills/running-marketing/SKILL.md) | 11 | [aeo-seo](sources/gtm-strategist-skill/references/aeo-seo.md), [linkedin-playbook](sources/gtm-strategist-skill/references/linkedin-playbook.md), [prompts](sources/gtm-strategist-skill/references/prompts.md), [growth-loops](sources/gtm-strategist-skill/references/growth-loops.md) |
| 12 | [executing-sales](sources/gtm-strategist-skills-official/.claude/skills/executing-sales/SKILL.md) | 10 | [prompts](sources/gtm-strategist-skill/references/prompts.md), [linkedin-playbook](sources/gtm-strategist-skill/references/linkedin-playbook.md), [tool-stack](sources/gtm-strategist-skill/references/tool-stack.md), [frameworks](sources/gtm-strategist-skill/references/frameworks.md) |

## Decisions and evidence

Distinguish confirmed inputs, source claims, assumptions and unknowns. Adapt institutional, consumer, enterprise, services, software, physical-product or other examples to the actual business; do not silently treat generic benchmarks as targets. Verify current tool/pricing/market claims before recommending them. Do not invent capabilities, integrations, customers, testimonials, competitors, prices or measured results.

For positioning, map actual alternatives before claiming difference. Leave unsupported uniqueness or value claims unresolved. For launches, distinguish product readiness, customer activation and external announcement where those are separate decisions. Identify owners, dependencies, measures, open risks and required human approvals without fabricating approval records.

Drafting is not authorization to send messages, publish, spend, change external systems or make regulated decisions. Use the user's actual scope and authorization for those actions.

## One system with preserved sources

This entry point resolves routing between the two archived source systems. Use the official task for deliverable structure and the curated library as optional support; do not produce duplicate canvases. Original instructions to choose between separate installations or always run a full phase describe those original systems, not two competing agents here.

Read [COMPATIBILITY.md](COMPATIBILITY.md) if a prior output name cannot be found; use existing equivalent content and record its actual filename. Do not create empty artifacts merely to satisfy an alias. Preserve original source files and notices.

## Outputs and inspectable execution

Save substantive artifacts to the active project's `outputs/` using the selected task's filename when applicable. Preserve approved prior work. Include relevant inputs, evidence, assumptions, decision, next action, owner and success measure. If requested, show a concise run trace: input → facts/gaps → selected workflow/reference → alternatives considered → decision → output → review questions.

If file access or nested skill invocation is unavailable, read linked Markdown as instructions and return the result with a suggested filename. Do not claim a save, install, test, approval or external action occurred unless verified.

## Optional extensions

When the user explicitly supplies an industry extension, load it after project context and before the selected task. Record its source/version and apply its domain-specific inputs and checks within the general workflow. Surface conflicts and follow the user's actual constraints. Do not invent or build an extension from an industry label alone. Keep company cases, private inputs and extension-specific outputs outside this reusable core.

[FRAMEWORK.md](FRAMEWORK.md) explains the core flow; [LIBRARY.md](LIBRARY.md) catalogs tasks and references; [NOTICE.md](NOTICE.md) records applicable notices.
