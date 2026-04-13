# Lewis Brain — Master Document

> This document gives any AI everything it needs to operate on VYVE Health business and commercial tasks with Lewis Vines (CEO).
> Last verified: 13 April 2026.

---

## 1. What Is VYVE Health?

VYVE Health CIC is a UK-based Community Interest Company building a proactive wellbeing platform for individuals and employers. Three pillars: Physical, Mental, Social health. AI coaching personas personalise the member experience.

**Stage:** Pre-revenue, MVP, validation.
**Members:** 11 (verified 11 April 2026).
**Legal:** ICO registered (00013608608). CIC = 6-8 point advantage in public sector procurement.

### Team
| Role | Person | Email | Focus |
|------|--------|-------|-------|
| CEO / Founder | Lewis Vines | lewisvines@hotmail.com | Commercial, sales, content, AI ops |
| CTO / Co-Founder | Dean Brown | deanonbrown@hotmail.com | Technical (part-time until 6K/month revenue) |

**Business email:** team@vyvehealth.co.uk — always use this for external comms, never personal emails.

---

## 2. Product — What Members Get

- 5 AI coaching personas (NOVA, RIVER, SPARK, SAGE, HAVEN)
- 8-week personalised workout programmes
- Daily habit tracking with monthly themes
- Weekly and monthly wellbeing check-ins with AI reports
- AI-generated running plans
- Nutrition logging (TDEE, macros, food diary)
- Live sessions with real-time chat
- Certificate system with charity donation mechanic
- Leaderboards and engagement scoring
- Web push notifications (habit + streak reminders)

### What Makes VYVE Different
- CIC structure = public sector procurement advantage + social impact story
- AI personas provide personalised coaching at scale (not one-size-fits-all)
- Three-pillar approach (Physical, Mental, Social) — not just fitness
- Employer dashboard with aggregate anonymised data (no PII) — HR gets ROI visibility
- Certificate + charity mechanic = tangible social impact per member

---

## 3. Pricing

| Channel | Price | Notes |
|---------|-------|-------|
| B2C | GBP20/month | Individual subscription |
| B2B | GBP10/user/month | Advertised at GBP20, discount applied. Volume tiers TBD for 200+ seats |
| Stripe checkout | buy.stripe.com/00wfZicla1Em0NnaIB93y00 | |
| Coupons | VYVE15, VYVE10 | Active |

---

## 4. Key URLs & Accounts

| Reference | Value |
|-----------|-------|
| Member portal | online.vyvehealth.co.uk |
| Marketing site | www.vyvehealth.co.uk |
| Command Centre | admin.vyvehealth.co.uk |
| Onboarding form | www.vyvehealth.co.uk/welcome |
| Strategy dashboard | online.vyvehealth.co.uk/strategy.html (password: vyve2026) |
| HubSpot Hub ID | 148106724 |
| Sage Deal | 495586118853 |
| Stripe checkout | buy.stripe.com/00wfZicla1Em0NnaIB93y00 |

### Accounts / Tools
| Tool | Used By | Purpose |
|------|---------|---------|
| Supabase | Dean (primary), Lewis (Command Centre) | Backend, DB, auth |
| Brevo | Lewis + Dean | Transactional + marketing email (free tier, 300/day) |
| HubSpot | Lewis | CRM, contact management |
| Make | Lewis only | Social media automation |
| PostHog | Dean (primary) | Product analytics |
| Stripe | Lewis + Dean | Payments |
| Claude.ai | Both | AI assistant (Projects for Lewis's 24 skills) |
| Anthropic API | Dean (via Edge Functions) | AI in the product (server-side only) |

---

## 5. AI Personas — What Lewis Needs to Know

| Persona | Character | When Assigned |
|---------|-----------|---------------|
| NOVA | High-performance coach. Data-led. Precision. | High scores + 1-2 performance-focused goals only |
| RIVER | Mindful guide. Calm, empathetic. | Low wellbeing/energy or high stress (stressed) |
| SPARK | Motivational powerhouse. Energetic accountability. | Mixed goals, consistency focus, busy lifestyles. DEFAULT for most. |
| SAGE | Knowledge-first mentor. Evidence-based. | Knowledge-seekers |
| HAVEN | Mental health companion. | NOT LIVE — needs professional review before activation |

### Critical: Stress Scale
- 1 = Very stressed, 10 = Very calm
- This is inverted from intuition — a HIGH stress score means the person is CALM
- This matters when Lewis discusses personas or member assignments in sales contexts

---

## 6. Sales & Pipeline

### Target Segments
1. **SMEs (10-200 employees)** — Decision maker: HR Manager or MD. Pain: absenteeism, retention, wellbeing duty of care.
2. **Public sector** — CIC status = procurement advantage. NHS, councils, universities.
3. **Charities / third sector** — Social impact alignment.
4. **B2C individuals** — Direct via marketing site + social.

### Employer Value Proposition
- Aggregate wellbeing dashboard (no individual PII)
- Measurable ROI: engagement scores, check-in trends, activity levels
- Duty of care compliance
- CIC structure = social value scoring in tenders

### Current Pipeline
> Maintained in Command Centre (admin.vyvehealth.co.uk) > Sales Pipeline page.
> Also tracked in HubSpot.

---

## 7. Content Strategy

### Lewis's 24 AI Skills (Claude.ai Projects)
Lewis runs 24 AI skills inside Claude.ai Projects (subscription, no API cost). Each skill produces structured JSON output that gets imported into the Command Centre via Agent Sync.

Skills cover: market research, competitor analysis, grant scouting, legislation tracking, content generation, social media, investor prep, and more.

### Content Channels
| Channel | Frequency | Owner |
|---------|-----------|-------|
| LinkedIn (company) | 3-5x/week | Lewis |
| LinkedIn (Lewis personal) | 2-3x/week | Lewis |
| Blog (marketing site) | 1-2x/month | Lewis |
| Email newsletter | Monthly | Lewis (via Brevo) |
| Podcast | TBD | Lewis |

### Brand Voice Rules
- Warm, human, evidence-based — never corporate jargon
- "Wellbeing" not "wellness" (UK English)
- "Members" not "users" or "customers"
- Never say "Corporate Wellness" as a tagline
- CIC = Community Interest Company (explain on first use in external comms)
- Always UK English spelling (colour, programme, organisation)

---

## 8. VYVE Command Centre

### What It Is
Internal ops dashboard for VYVE leadership. Browser-based, hosted at admin.vyvehealth.co.uk. Separate from the member portal.

### How to Access
- URL: admin.vyvehealth.co.uk
- Login: Supabase Auth — team@vyvehealth.co.uk
- All data now persists in Supabase (as of 13 April 2026 — no more localStorage loss)

### Pages (27 across 5 sections)
**Intelligence:** Morning Brief, Research & Grants, Competitor Watch
**Business:** Dashboard, Finance & Funding, Clients, Sales Pipeline, Investor Relations, Partner Network, Invoicing, Sessions, Tasks, Compliance
**Content & Growth:** Content, Performance, Podcast, Brand & Voice
**Strategy:** Strategy Room (OKRs/Decisions/Learnings/SWOT), Documents, Knowledge Base
**Team:** Team Hub
**System:** Settings

### Agent Sync (Lewis's workflow)
1. Run an AI skill in Claude.ai Projects
2. Skill outputs structured JSON
3. Open Command Centre > Settings > Agent Sync
4. Paste JSON > Import
5. Data populates the relevant Intelligence section

---

## 9. Grants & Funding

### Target Grants
| Grant | Amount | Deadline | Status |
|-------|--------|----------|--------|
| National Lottery | TBD | June/July 2026 | Research phase |
| The Fore | Up to GBP30K | June/July 2026 | Research phase |

### CIC Advantages for Funding
- Asset lock = credibility with funders
- Social mission alignment
- Public sector procurement scoring bonus
- Can still generate revenue (CIC is not a charity)

---

## 10. App Store Status

| Platform | Status | Notes |
|----------|--------|-------|
| Android (Google Play) | Submitted 12 April 2026 | Awaiting review (1-3 days) |
| iOS (App Store) | Submitted 13 April 2026 | Awaiting review (24-48 hours) |

Old Kahunas app (com.kahunas.io.VYVE) still on Play Store — deprecate after new app approved.

---

## 11. Hard Rules (NEVER BREAK)

1. **Business email only** for external comms: team@vyvehealth.co.uk
2. **Never say "Corporate Wellness"** as a tagline
3. **UK English** always (programme, colour, organisation)
4. **"Members"** not users or customers
5. **HAVEN persona is NOT live** — never promise mental health counselling in sales materials
6. **Employer dashboard = aggregate only, no PII** — this is a selling point AND a compliance requirement
7. **CIC is not a charity** — can generate revenue, has asset lock, social mission
8. **API keys never in sales decks or external docs** — if a prospect asks about security, refer to Dean
9. **Dean is part-time until GBP6K/month revenue** — scope technical promises accordingly
10. **Pricing is GBP10/user/month B2B** (advertised at GBP20 with discount) — don't go below without discussing with Dean
11. **ICO registration: 00013608608** — include in data protection responses
12. **Stress scale: 1 = very stressed, 10 = very calm** — if discussing personas externally, get this right

---

## 12. Technical Context (Light — For Sales Conversations)

Lewis doesn't need deep technical knowledge, but should be able to speak to these in sales:

- **Data hosting:** Supabase, West EU/Ireland. GDPR-compliant region.
- **Auth:** Supabase Auth (industry standard). MFA available.
- **AI:** Anthropic (Claude) — server-side only, no data leaves to train models.
- **Analytics:** PostHog (EU endpoint). Identity linked to auth.
- **Architecture:** Progressive Web App (works offline, installable). Native apps in review.
- **Security:** Full audit completed 11 April 2026. RLS on all tables. No PII in employer dashboard.
- **Compliance:** ICO registered. Privacy policy live. External DPO planned before 500 members.

For anything deeper, tag Dean.

---

## 13. Dean's Brain (Cross-Reference)

Dean's technical brain is at `VYVEHealth/VYVEBrain`. Lewis can read it when needed:
- `brain/master.md` — full technical architecture, DB schema, Edge Functions, auth patterns
- `brain/changelog.md` — technical change log
- `tasks/backlog.md` — technical backlog
- `playbooks/` — technical playbooks (debug, build, refactor, etc.)

**When to read Dean's brain:** Before a technical sales question you can't answer, or when you need to confirm what's been built vs what's planned.
