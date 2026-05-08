# <Automation Name> Plan

Status: Draft for review
Owner/requester: <name or team>
Date: <date>

## Plain-English Summary

<Describe the repeated task and the smallest useful automation in 2 to 4 sentences.>

## Current Manual Workflow

<Explain what the person does today, step by step, without technical jargon.>

## Shared Workflow Language

Terms:

- `<Term the user uses>`: <Plain-English meaning future agents should reuse.>

Flagged ambiguities:

- <Term or phrase that could mean multiple things, or "None".>

## First Version Scope

<List what this first version will do. Keep it narrow.>

## Out Of Scope

<List tempting but intentionally excluded features.>

## Working Location And Version Control

Current workspace/repo:

- <Where the agent started and what this repo appears to be for.>

Plan/code/docs destination:

- <Where the plan, implementation, and recipe card will live.>

Version control:

- <Whether the destination is already a git repo. If not, say whether to initialize one before implementation.>

## Apps, Files, And Systems Touched

<Name every app, spreadsheet, folder, API, inbox, or system involved.>

## Data, Permissions, And Secrets

Data sensitivity:

- <Public/internal/customer data/PII/financial/compliance-sensitive/unknown.>

Access and permissions:

- <Who must grant access, what level is needed, and what the automation must not be able to do.>

Secrets:

- <Credential or environment variable names needed, without secret values.>

## Inputs And Outputs

Inputs:

- <What the automation starts with.>

Outputs:

- <What the automation produces or changes.>

## Human Approval Points

<Describe anything the user must review before the automation sends, deletes, publishes, charges, updates important records, or contacts customers.>

## Risks And Safeguards

<Describe what could go wrong and how the first version reduces that risk.>

## Chosen Build Shape

Recommended shape: <prompt/checklist, spreadsheet, no-code integration, script, scheduled script, Slack/email bot, web page, durable workflow, agent, MCP/API>

Why this is the simplest good option:

<Explain in plain language.>

## How It Will Run

<Describe whether the user runs a command, opens a page, fills a form, sends a Slack message, waits for a schedule, or uses another trigger.>

## Run Mode

Mode: <manual/supervised/scheduled/autonomous>

Why this mode is safe for the first version:

- <Plain-English reason.>

What would need to change before more autonomy:

- <Examples, safeguards, approvals, monitoring, or ownership needed.>

## Rollout Plan

Dry run or preview:

- <How to test without sending, deleting, charging, publishing, or changing important records.>

First real run:

- <Who will watch it, what small batch or low-risk case to start with, and what success looks like.>

Status and failures:

- <Where logs/status will appear and who is notified if it fails.>

Rollback or disable:

- <How to stop it safely and undo reversible changes.>

## What The User Needs To Provide

- <Example files, app access, API keys, approval rules, or sample inputs.>

## Success Metric

<A concrete sign that the automation is worth keeping, such as time saved per week, fewer missed steps, or faster response time.>

## Definition Of Done

- <Plan approved by the owner.>
- <Dry run or preview tested with representative examples.>
- <Human approval rules are implemented for high-impact actions.>
- <Logs, status, or failure notification are visible to the owner.>
- <Recipe card is written with run, test, rollback, and repair notes.>

## Maintenance Notes For Future Agents

<Describe where the code will live, what future agents should read first, what not to change casually, and what tests/examples should keep working.>

## Open Questions

- <Question 1, or "None".>

## Review Request

Please review this plan and say whether to approve it, revise it, or stop here.
