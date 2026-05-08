# <Automation Name> Recipe Card

Owner: <name or team>
Last reviewed: <date>

## Purpose

<What repeated workflow this automation helps with.>

## Shared Workflow Language

- `<Term the user uses>`: <Plain-English meaning future agents should reuse.>

## Trigger

<What starts the automation: command, schedule, form submission, Slack message, email, file drop, manual button, etc.>

## What It Does

<Step-by-step summary of the automation's actions.>

## Where This Lives

Plan:

- <Path to the approved plan.>

Implementation:

- <Repo/folder/file paths for the code or app configuration.>

Version control:

- <Git repo, branch, commit, or "Not versioned yet because...".>

## What It Touches

Apps/files/systems:

- <App, file path, folder, API, inbox, spreadsheet, database, or service.>

Data sensitivity:

- <Public/internal/customer data/PII/financial/compliance-sensitive/unknown.>

Access and permissions:

- <Who owns access, what permissions are required, and what the automation is not allowed to do.>

Credentials or environment variables:

- `<NAME>`: <what it is used for, without including the secret value.>

## How To Run

```bash
<command or "No command: runs through <app/schedule/page>.">
```

## Run Mode

Mode: <manual/supervised/scheduled/autonomous>

What this means:

<Whether a person runs it, approves each run, monitors a schedule, or allows low-risk autonomous work.>

## Human Approval Rules

<What must be reviewed before the automation sends, deletes, publishes, charges, changes permissions, contacts customers, or updates important records.>

## How To Test Safely

<Describe the dry run, sample file, staging account, preview mode, or test command.>

## Status, Logs, And Failure Notifications

Status/log location:

- <File path, app page, Slack channel, email, dashboard, or command output.>

Failure notification:

- <Who gets notified, where, and what message/action they should expect.>

## Example Inputs And Expected Outputs

Example input:

```text
<small representative input>
```

Expected output:

```text
<small representative output or behavior>
```

## Known Limits

- <Limit or edge case.>

## Failure Modes And Troubleshooting

- Symptom: <what the user or future agent sees>
  Likely cause: <why it happens>
  Fix: <what to check or change>

## Rollback Or Disable

<How to stop the automation safely and undo any reversible changes.>

## Future Agent Notes

<Where the implementation lives, what files to read first, what tests to run, and what assumptions should not be changed without user review.>
