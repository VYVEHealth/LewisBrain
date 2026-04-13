# Playbook: Agent Sync

**Trigger:** `run agent sync`
**Purpose:** Guide the workflow for syncing AI Skill outputs into the VYVE Command Centre

---

## Claude's Instructions

When this playbook is triggered:

### Step 1 — Load Context
Read from master.md:
- The 24 AI Skills list (names, output formats, Command Centre sections they feed)
- Command Centre structure
- Make automation scenarios related to agent outputs

### Step 2 — Ask Lewis
"Which skills are we syncing today? Options:
1. All skills — full sync run
2. Specific skill(s) — tell me which ones
3. Check what's unsynced — review what outputs are waiting to be imported"

### Step 3 — Run the Sync

For each skill being synced:

**Step 3a — Retrieve Output**
Ask Lewis: "Do you have the output ready, or do we need to run the skill first?"
- If the skill needs running, trigger it and capture the output
- If Lewis has the output, ask them to paste or describe it

**Step 3b — Map to Command Centre**
Using the skill-to-section mapping from master.md:
- Identify which Command Centre section this output feeds
- Check if there's a Make automation that handles this import automatically
- If yes: confirm it ran / prompt Lewis to trigger it
- If no: guide Lewis through the manual import steps

**Step 3c — Validate**
Ask: "Has the data appeared in the Command Centre correctly?"
- If yes: mark as synced, proceed to next skill
- If no: troubleshoot — is it a format issue, a mapping issue, or an automation error?

### Step 4 — Automation Health Check
If running a full sync, also check:
- Are all Make scenarios that feed the Command Centre active?
- Any scenarios paused or throwing errors?
- Any data that should have been auto-synced but wasn't?

### Step 5 — Update Brain
After the session:
- Note any sync issues or changes to Make automations in master.md
- Update the Make Automations section if anything changed
- Run brain sync

---

## Sync Mapping Reference

[LEWIS TO FILL IN during first brain session]

> This table should map each AI Skill to its Command Centre destination:
>
> | Skill Name | Output Format | Command Centre Section | Sync Method |
> |---|---|---|---|
> | [Skill 1] | [Format] | [Section] | [Auto / Manual] |
> | [Skill 2] | [Format] | [Section] | [Auto / Manual] |
> | ... | | | |

---

## Common Sync Issues

[LEWIS TO FILL IN as issues arise]

> Document recurring issues and their fixes here so Claude can troubleshoot them automatically in future sessions.
