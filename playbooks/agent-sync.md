# Playbook: Agent Sync

## When to Use
Running Lewis's 24 AI skills in Claude.ai Projects and importing output to the Command Centre.

## Steps

### 1. Run the Skill
- Open the relevant Claude.ai Project (each of the 24 skills is a separate Project)
- Execute the skill - it will produce structured JSON output
- Copy the JSON

### 2. Import to Command Centre
- Open admin.vyvehealth.co.uk > Settings > Agent Sync
- Paste JSON into the import modal
- Click Import
- Data populates the relevant Intelligence section

### 3. Review
- Navigate to the section the data feeds (Research & Grants, Competitor Watch, etc.)
- Verify the import looks correct
- Flag anything that needs action as a task

### 4. Log
- If the import contained significant intelligence (new competitor, grant opportunity, legislation change), update `brain/master.md` or `brain/changelog.md` via brain sync

## Notes
- The 24 skills run inside Claude.ai subscriptions - no API cost
- Skills are independent of the Lewis Brain system (different Claude sessions)
- Agent Sync is the bridge between the skills and the Command Centre
