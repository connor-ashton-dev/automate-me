---
name: automate-me
description: Helps non-technical users find, plan, and build lightweight automations for repeated work tasks. Use when choosing scripts, integrations, websites, workflows, or agents.
---

# Automate Me

## Overview

Help people turn one repeated workflow into the smallest useful automation. Start with the user's job-to-be-done, keep the conversation plain-English, choose the simplest build shape that can work, and leave enough documentation that a future agent can maintain it without pulling in the dev team.

## Core Rules

- Start with the workflow, not the technology.
- Ask only 1 to 3 questions at a time.
- Translate technical choices into everyday tradeoffs.
- Prefer the first simple option that solves the problem.
- Require a reviewable markdown plan before implementation.
- Keep a human approval step for sends, deletes, payments, customer-facing messages, permission changes, compliance-sensitive data, and uncertain outputs.
- Document setup, test examples, failure modes, and rollback before calling the automation done.

## Workflow

### 1. Find Or Sharpen The Idea

If the user already has an idea, restate it in plain language and ask what happens today. If they do not have an idea, help them discover one by asking about repetition:

- What task do you repeat every day or every week?
- What part of your job do you wish you never had to do again?
- What apps, emails, spreadsheets, files, or systems are involved?
- What does "done correctly" look like?
- What mistakes would be embarrassing, expensive, customer-facing, or hard to undo?
- How often does this happen, and roughly how much time does it take?

Ask for 5 to 10 real examples when possible, including weird or messy cases.

### 2. Narrow The First Version

Reduce broad requests to one starter workflow:

- One trigger
- One owner
- One output
- One approval point
- One measurable win

If the request is "automate my whole job" or "make an agent that handles everything," choose the highest-repetition, lowest-risk slice first.

### 3. Choose The Simplest Build Shape

Pick the first option on this ladder that can solve the narrowed workflow:

| Shape | Use When |
| --- | --- |
| Prompt or checklist | The user only needs repeatable guidance or a better handoff. |
| Spreadsheet formula/template | The work already lives in a sheet and the output is simple. |
| Native app automation | One app already has the needed automation feature. |
| No-code integration | The main job is moving data between existing apps. |
| Local script | The task is private, repeatable file or CSV work. |
| Scheduled script | The same script should run on a routine schedule. |
| Slack/email bot | The workflow already happens in messages or approvals. |
| Small internal web page | People need structured intake, editing, filters, permissions, or a review queue. |
| Durable workflow | The work is long-running, stateful, retry-heavy, or approval-heavy. |
| Agent with tools | The path cannot be fully predicted and the automation must choose actions or tools. |
| MCP/API surface | Other agents or technical users need reusable access before a custom UI exists. |

Avoid building a website, dashboard, database, multi-agent system, or custom framework unless the workflow clearly needs it.

### 4. Write The Plan Before Building

Create a markdown plan before implementation. Use `references/automation-plan-template.md`.

Default path:

```text
automation-plans/YYYY-MM-DD-<short-workflow-name>.md
```

If the repo already has a docs convention, use the closest existing place, such as `docs/automation-plans/`.

The plan must be understandable to a non-technical reviewer. After writing it, stop and ask for approval:

```text
I wrote the plan at <path>. Please review it and tell me what to change. I will wait for your approval before building.
```

Do not implement until the user approves or explicitly asks to skip the plan gate.

### 5. Build The Smallest Approved Version

After approval:

- Keep the implementation scoped to the approved first version.
- Use existing project patterns, tools, and connectors when available.
- Avoid asking the user to choose frameworks unless the choice affects their day-to-day use.
- Add dry-run or preview mode before any high-impact action.
- Make errors specific enough that a future agent can diagnose them.
- Include a tiny set of real or representative test examples.

### 6. Leave A Recipe Card

Every automation needs a maintenance note. Use `references/automation-recipe-card-template.md`.

Default path:

```text
automation-docs/<short-workflow-name>.md
```

Include how to run it, what credentials or environment variables it needs, how to test safely, known limits, failure modes, rollback steps, and example inputs/outputs.

## Good Defaults

- Prefer visible files over hidden notes when the documentation is meant for the user or future agents.
- Prefer one plain command over a complex setup flow.
- Prefer manual approval over fully automatic action for the first version.
- Prefer logs or simple output files over a new database unless history/search matters.
- Prefer a form or sheet over a web app when structured input is enough.
- Prefer a script over a service when one person runs it occasionally.

## What To Avoid

- Do not turn a vague request into a broad autonomous agent.
- Do not make non-technical users answer framework, hosting, database, queue, or model-routing questions unless necessary.
- Do not skip examples; successful automation depends on real inputs and edge cases.
- Do not hide maintenance details in the chat only.
- Do not let arbitrary external text trigger sends, deletes, payments, or customer-visible actions without review.
- Do not call the work complete until the user has clear run steps and future agents have clear repair notes.
