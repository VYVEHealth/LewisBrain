# How to Use the Lewis Brain

> This guide is for Lewis (CEO) — the human operator.

## Daily Workflow

### Starting a Session with Claude
1. Open claude.ai (make sure Composio is connected — see setup guide).
2. Paste your session start prompt (below) as your first message.
3. State your task clearly.

### Session Start Prompt
```
# Lewis Brain — Session Start
Initialise the Lewis External Brain:
1. Read from repo `VYVEHealth/LewisBrain` (main branch):
   - `brain/master.md`
   - `brain/changelog.md`
   - `tasks/backlog.md`
2. Load playbooks from `/playbooks/` only when the task requires one.
3. GitHub access: Composio (full read/write). Use tools directly — don't simulate.
4. The repo is the source of truth, not chat history.
Confirm: brain loaded, tools available (yes/no), then ask what we're working on.
```

### Shortcut Commands
Instead of the full session start, you can say:
- `Load Lewis Brain and run content creation` — writes blog posts, social, copy
- `Load Lewis Brain and run sales pipeline` — pipeline review, outreach drafts
- `Load Lewis Brain and run morning brief` — daily ops summary
- `Load Lewis Brain and run grant application` — grant writing
- `Load Lewis Brain and run investor comms` — investor updates, pitch prep
- `Load Lewis Brain and run brain sync` — save session work back to the repo

### Idea to Execution
```
1. IDEA        > One sentence
2. TASK CARD   > Copy tasks/task-template.md, fill in (2 min)
3. PLAYBOOK    > Pick the right one
4. EXECUTE     > Paste task card into AI session
5. VERIFY      > Check output
6. ARCHIVE     > Move to tasks/completed/
```

## Choosing a Playbook
| Situation | Playbook |
|-----------|----------|
| Writing content (blog, social, scripts) | content-creation.md |
| Working the sales pipeline | sales-pipeline.md |
| Grant research or writing | grant-application.md |
| Investor updates or pitch prep | investor-comms.md |
| Morning ops summary | morning-brief.md |
| Running AI skills + importing to Command Centre | agent-sync.md |
| Partner outreach or management | partnerships.md |
| Saving work back to GitHub | brain-sync.md |

## Reading Dean's Brain
If you need technical context (e.g., "has this feature been built yet?"), tell Claude:
```
Read brain/master.md from VYVEHealth/VYVEBrain
```

## Updating the Brain
After sessions where business context changed, tell Claude:
```
Run brain sync — update the changelog and any files that changed.
```

## Emergency: Lost AI Access
1. Sign up for any AI (ChatGPT, Gemini, anything)
2. Paste `prompts/cold-start.md` contents
3. Resume work. The brain is in GitHub, not in any AI's memory.

## What NOT to Edit
- Don't edit Dean's repo (`VYVEBrain`) — read-only for Lewis
- Don't put credentials or API keys in any brain file
- Don't change pricing without discussing with Dean first
