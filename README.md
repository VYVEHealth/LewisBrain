# Lewis Brain — External Brain (CEO)

Zero-dependency knowledge system for AI-assisted business operations.
Any AI model can load this repo and immediately operate on VYVE Health commercial tasks with Lewis.

---

## TL;DR — How to Start Every Chat

### Option A: With Composio (recommended)
Copy the contents of **`prompts/session-start.md`** and paste as your first message in a new Claude chat.

### Option B: Without Composio (any AI)
Copy the contents of **`prompts/cold-start.md`** and paste into any AI (Claude, ChatGPT, Gemini, etc.).

### Option C: Shortcut commands (with Composio)
Just type one of these as your first message:
- `Load Lewis Brain and run content creation`
- `Load Lewis Brain and run sales pipeline`
- `Load Lewis Brain and run morning brief`
- `Load Lewis Brain and run grant application`
- `Load Lewis Brain and run investor comms`
- `Load Lewis Brain and run brain sync`

---

## Prompts (start here)

| File | When to Use |
|------|-------------|
| `prompts/session-start.md` | Every Claude chat with Composio connected — loads your full brain from GitHub |
| `prompts/cold-start.md` | Any AI without Composio — gives essential context from memory |

## Folder Structure

```
├── README.md
├── brain/
│   ├── master.md              ← Complete business + commercial context
│   ├── how-to-use.md          ← Operator guide for Lewis
│   ├── changelog.md           ← Session log (what changed and when)
│   └── startup-prompt.md      ← Instructions Claude reads on load
├── playbooks/
│   ├── content-creation.md    ← Blog posts, social, video scripts
│   ├── sales-pipeline.md      ← Lead qualification, outreach, follow-up
│   ├── grant-application.md   ← Grant writing and submission
│   ├── investor-comms.md      ← Investor updates, pitch prep
│   ├── morning-brief.md       ← Daily ops summary generation
│   ├── agent-sync.md          ← Running 24 AI skills + CC import
│   ├── partnerships.md        ← Partner outreach and management
│   └── brain-sync.md          ← Saving work back to GitHub
├── prompts/
│   ├── session-start.md       ← Paste into Claude (with Composio)
│   └── cold-start.md          ← Paste into ANY AI (without Composio)
├── tasks/
│   ├── backlog.md             ← Prioritised commercial task list
│   ├── task-template.md       ← Blank task card
│   ├── open/
│   ├── blocked/
│   └── completed/
└── reference/
    └── (brand voice, pricing, contacts — to be populated)
```

## First Time Setup

See `brain/how-to-use.md` for Composio + GitHub connection instructions.

## Updating Your Brain

After any session where business context changed, tell Claude:
```
Run brain sync
```

## Cross-Brain Access

Dean's technical brain: `VYVEHealth/VYVEBrain`
Lewis's commercial brain: `VYVEHealth/LewisBrain` (this repo)

Both can read each other's repos for cross-functional context.

## Sections Lewis Needs to Fill In

The master.md has placeholder sections marked **[LEWIS TO FILL IN]**. These are things only Lewis knows:
- His 24 AI skill names and descriptions
- Active pipeline leads and contacts
- Content calendar and themes
- Make automation scenarios
- Key relationships and partnerships
- Session schedule and delivery format
- Grant contacts and progress

To fill these in, start a brain session and say: "Help me fill in the [LEWIS TO FILL IN] sections in master.md"

## Last Updated

13 April 2026 — initial creation.
