# Playbook: Brain Sync

**Trigger:** `run brain sync`
**Purpose:** Save session work back to GitHub — update master.md, changelog, and backlog

---

## Claude's Instructions

When this playbook is triggered (typically at the end of a session):

### Step 1 — Session Review
Ask Lewis: "Before I sync — is there anything specific from this session you want me to capture?"

Also review what was worked on in this session (from context) and identify:
- Any decisions made
- Any new information about VYVE, the product, the pipeline, etc.
- Any tasks completed
- Any new tasks created
- Any changes to strategy, pricing, or positioning

### Step 2 — Update master.md

For each area that has new information:
- Navigate to the relevant section in `brain/master.md`
- Update or add the information
- Replace any `[LEWIS TO FILL IN]` placeholders that were covered this session

Sections most commonly updated:
- Active Prospects (sales pipeline changes)
- Published Content (new posts or articles)
- Grant Pipeline (new applications or status updates)
- Key Relationships (new contacts or updates)
- Task completion status

### Step 3 — Update tasks/backlog.md

- Mark completed tasks as done (move to Completed table with today's date)
- Add any new tasks that came up during the session
- Reprioritise if Lewis indicated anything has changed in urgency

### Step 4 — Update brain/changelog.md

Add a new entry at the top of changelog.md:

```
## YYYY-MM-DD — [One-line session summary]

**Session:** [Brief description of what was worked on]
**Changes:**
- [File]: [What changed]
- [File]: [What changed]

**Decisions made:**
- [Any key decisions]

**Next action:** [What happens next / what Lewis should do]
```

### Step 5 — Commit to GitHub

Using Composio GitHub tools:
1. Stage all changed files
2. Commit with message: `Brain sync: [date] — [one-line summary]`
3. Push to main branch of VYVEHealth/LewisBrain
4. Confirm: "Brain synced. [X] files updated and committed."

### Step 6 — Confirm
Tell Lewis: "Brain sync complete. Here's what was saved: [summary of changes]. See you next session."

---

## Files Managed by Brain Sync

| File | What it tracks |
|---|---|
| `brain/master.md` | Everything about VYVE and Lewis's operating context |
| `brain/changelog.md` | Running log of sessions and decisions |
| `tasks/backlog.md` | Task list and priorities |
| `playbooks/*.md` | Updated if a new playbook was created or an existing one improved |

---

## Notes for Claude

- Always commit to the `main` branch unless Lewis specifies otherwise
- If GitHub / Composio is unavailable, save the updates locally and tell Lewis to paste them in next time
- Never commit anything confidential that Lewis hasn't explicitly approved (e.g. specific financial figures, client names if Lewis says they're sensitive)
- The sync should take under 2 minutes — keep it efficient
