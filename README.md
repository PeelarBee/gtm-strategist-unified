# Unified Go to Market Agent

An industry-agnostic agent combining a structured go-to-market workflow with a reference library of frameworks, prompts and playbooks. Use it for any company's strategy, customer research, pricing, positioning, launch, marketing or sales. Industry-specific requirements belong in separate extensions and project context.

## Start here

1. Open this repository in a file-capable assistant and ask it to read [SKILL.md](SKILL.md). No global installation is required for explicit use.
2. Select a separate working project folder. Use the [context template](sources/gtm-strategist-skills-official/my-gtm-context.md) to capture product, market, customer, evidence and constraints. The agent can interview you and save the answers.
3. Ask for one outcome. The agent selects a relevant workflow and supporting references, builds on previous work, labels assumptions and saves the deliverable to your working project's `outputs/` folder when file access is available.

Example: “Read SKILL.md. Help me develop positioning for my product from the customer evidence I provide. Show confirmed facts, missing inputs, the positioning decision and the next validation action.”

For a focused question: “Use reference mode to explain ECP versus ICP for my product stage.”

## What is included

- **12 connected phases and 100 tasks:** strategy, research, customer validation, product, pricing, positioning, launch assets, communication, launch execution, growth systems, marketing and sales.
- **Nine reference files:** core frameworks, adaptable prompts, AEO/SEO, persistent project context, tools, operational workflows, growth loops, LinkedIn and a context template.
- **One entry point:** use the workflow for deliverable structure and load only the references useful to the selected task.
- **Evidence and human decisions:** missing information stays explicit. Drafting does not authorize sending, publishing, spending or changing external systems.

[FRAMEWORK.md](FRAMEWORK.md) explains the general workflow. [LIBRARY.md](LIBRARY.md) lists every phase, task and reference section. [COMPATIBILITY.md](COMPATIBILITY.md) resolves source filename differences so later phases can find earlier outputs.

## How to see the agent work

Ask for an execution trace showing **input → confirmed facts and unknowns → selected workflow and references → decision alternatives → draft output → questions for human review**. Review a local first run before choosing whether to install it in a host's skill discovery directory.

A 30-minute session should establish context, select one decision, produce one tailored draft and agree its next validation action. Real customer validation and operational execution require evidence and time.

In a chat without filesystem access, attach SKILL.md, the selected workflow and relevant reference files. A folder name does not upload its contents. Do not assume automatic saving or nested skill invocation when the host does not provide those capabilities.

## Separate industry extensions

The core has no default industry, company or product case. A future extension can supply domain terminology, workflows, evidence requirements and specialist review needs without replacing the core. Keep each extension and its product exercises in a separate package or project. No industry extension is included here.

## Project separation

Keep product briefs, customer information, research workbooks, campaign outputs, credentials and local environment files outside this repository. This repository contains only the reusable general agent, workflow, templates and reference library.

Historical tools, prices and claims in the reference library require current verification before recommendations.
