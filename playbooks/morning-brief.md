# Playbook: Morning Brief

**Trigger:** `run morning brief`
**Purpose:** Generate a focused daily ops summary — what happened, what is on today, blockers

---

## Claude's Instructions

When this playbook is triggered:

### Step 1 — Load Context
Read from:
- `brain/master.md` - pipeline, priorities
- `brain/changelog.md` - last session
- `tasks/backlog.md` - current tasks

### Step 2 — Generate the Brief

**🌅 VYVE Morning Brief — [Today]**

**Yesterday's wins** - [from changelog]
**Today's focus** - [top 3 tasks]
**Pipeline pulse** - [any deadlines due]
**What needs Lewis** - [blockers]
**On the radar** - [next 7 days]

### Step 3 — Ask What We're Working On

### Step 4 — Quick Wins Mode

---

## Notes
- Keep it under 2 minutes to read
- Energising, not bureaucratic
- Always end with "what are we working on?"
