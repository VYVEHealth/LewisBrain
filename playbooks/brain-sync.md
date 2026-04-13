# Playbook: Brain Sync

## When to Use
After any session where business context changed, tasks were completed, or decisions were made.

## Steps

### 1. Identify Changes
What happened in this session that future AI sessions need to know?
- New client or partnership?
- Pricing or strategy change?
- Task completed or new task identified?
- Content published?
- Grant submitted?
- Any business decision?

### 2. Update Files
| Change Type | File to Update |
|-------------|---------------|
| Business context (clients, pricing, team, strategy) | `brain/master.md` |
| Task completed | `tasks/backlog.md` - move to Completed |
| New task identified | `tasks/backlog.md` - add to appropriate priority |
| Any meaningful work | `brain/changelog.md` - new entry at top |

### 3. Write Changelog Entry
Format:
```markdown
## [Date] - [One-line summary]

### What Changed
- [Bullet points of what was done]

### Impact
- [Why it matters / what it unblocks]
```

### 4. Commit to GitHub
- Use Composio GitHub tools to commit all changed files
- Commit message: `brain sync: [date] - [summary]`

### 5. Verify
- Confirm files committed successfully
- Spot-check one file to make sure content is correct

## Rules
- Never remove historical changelog entries - only append at the top
- Keep master.md factual and current - remove stale information
- If unsure whether something is worth logging, log it. Better to have too much history than too little.
