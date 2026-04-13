# Playbook: Sales Pipeline

**Trigger:** `run sales pipeline`
**Purpose:** Review pipeline health, qualify leads, draft outreach, and write proposals

---

## Claude's Instructions

When this playbook is triggered:

### Step 1 — Load Context
Read from master.md:
- Active prospects list
- Pipeline stages
- Ideal Customer Profile (ICP)
- Pricing (B2B: £10/user/month, volume tiers TBD)
- HubSpot Hub ID: 148106724

### Step 2 — Pipeline Review
Ask Lewis: "Do you want a full pipeline review, or are we focusing on a specific prospect or stage?"

**If full review:**
Go through each active prospect and ask Lewis for a status update on any that haven't been updated in 7+ days. Summarise:
- Total active prospects
- Breakdown by stage
- Stalled deals (no activity in 14+ days)
- Deals most likely to close in the next 30 days

**If specific prospect:**
Ask: "Which prospect? What do you need — outreach draft, proposal, follow-up, or something else?"

### Step 3 — Qualify Leads
For any new leads or prospects Lewis mentions, run a quick qualification:

| Question | Why It Matters |
|---|---|
| How many employees? | Determines deal size (£10/user/month) |
| Who is the champion? | Do they have internal buy-in? |
| Who controls budget? | Are we talking to the right person? |
| What pain are they feeling? | Map to VYVE's pillars |
| What does their current wellbeing programme look like? | Gap analysis |
| What is the decision timeline? | Pipeline stage accuracy |
| Any blockers? | Procurement, budget cycles, competing priorities |

### Step 4 — Draft Outreach or Proposals

**Outreach email:**
- Short, personalised, one clear ask
- Reference a specific pain point or news about their organisation
- Suggest a 20-minute call
- Sign off as Lewis from team@vyvehealth.co.uk
- UK English, warm tone, no corporate jargon

**Proposal structure:**
1. Cover — VYVE logo, prospect name, date
2. The Challenge — Mirror their specific pain back to them
3. Our Approach — Three pillars explained simply
4. What Members Get — Features and experience
5. What Employers Get — Dashboard, reporting, aggregate insights
6. Pricing — Tailored to their headcount
7. Why VYVE — CIC advantage, evidence-base, personalisation
8. Next Steps — Pilot proposal or contract discussion

### Step 5 — Follow-Up Sequences
If Lewis needs a follow-up after a meeting:
- Day 1: Send meeting recap + next steps (Lewis sends)
- Day 5: Check-in if no response
- Day 14: Value-add follow-up (share a relevant article or stat)
- Day 30: Final nudge before archiving

Claude will draft any of these on request.

### Step 6 — Update Brain
After the session:
- Update Active Prospects in master.md with any new info
- Run brain sync to commit changes

---

## Pricing Reference

| Tier | Price | Notes |
|---|---|---|
| B2C | £20/month/member | Individual subscription |
| B2B Standard | £10/user/month | Per employee |
| B2B Volume | TBD | For 200+ users |

---

## Key Differentiators (for pitches)

- CIC = public sector procurement advantage
- Proactive, not reactive — intervention before burnout
- 5 AI coaching personas = personalised experience at scale
- Employer dashboard = aggregate insights, zero PII concerns
- Evidence-based — every feature tied to peer-reviewed research
