# Automate Me

`automate-me` helps non-technical teams turn repeated work into small, maintainable automations.

It guides an agent to:

- Find a repetitive workflow worth automating.
- Narrow the first version to the smallest useful scope.
- Capture the user's workflow language so future agents reuse the same terms.
- Choose the simplest build shape: prompt, spreadsheet, no-code integration, script, website, workflow, or agent.
- Classify the first version as manual, supervised, scheduled, or autonomous.
- Confirm the right repo or folder before writing implementation files.
- Write a plain-English plan before building.
- Capture data access, approval, rollout, logging, troubleshooting, and rollback notes for future agents.

## Install

```bash
npx skills add connor-ashton-dev/automate-me
```

The installer will ask which local agents should receive the skill.

## Try It

In Codex:

```text
Use $automate-me to help me automate a repetitive workflow.
```

In Claude Code:

```text
/automate-me
```

Or ask naturally:

```text
Help me automate a repetitive workflow I do every week.
```

## Package

The skill lives at:

```text
skills/automate-me/
```

The Claude plugin manifest lives at:

```text
.claude-plugin/plugin.json
```
