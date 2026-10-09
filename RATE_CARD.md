# Neki rate card

Version 2, 2026-10-08. Every task's Neki price comes from this card, so two people pricing the same task land on the same number. Rules for Neki itself: [`NEKI.md`](https://github.com/kamal0808/topc/blob/master/ecosystem/NEKI.md).

1 Neki = 1 rupee of work at today's market price: what it costs to get the result from a competent mid-level person in India **working with AI**. Most work is now done with an agent like Claude, so pricing it as if done by hand overpays it several times over.

## How the anchors are set

- **Work AI shrinks** (code, design, desk research, writing): the hours a competent person with an AI agent needs for the result, checking and testing included, times that role's market rate below.
- **Work AI barely shrinks** (talking to real people, a lawyer's judgement, real test sessions, running a community, registrations): the sourced market price for the result, as in version 1.

| Role | Rate | Source |
|---|---|---|
| Code | ₹800/hr | Mid-level (3–5 yrs) ₹500–800/hr, [Internshala](https://internshala.com/blog/employer-cost-to-hire-a-web-developer/); mid-level React ₹650–1,300/hr, [secondtalent](https://www.secondtalent.com/developer-rate-card/react-developer-india/) |
| Design | ₹1,500/hr | UI/UX median ₹12,000/day, [FeeBee](https://www.flexingit.com/feebee/freelance-ui_ux-fees-id-128/) |
| Research | ₹950/hr | Consumer research median ₹7,500/day, [FeeBee](https://www.flexingit.com/feebee/freelance-consumer_research-fees-id-46) |
| Testing | ₹1,400/hr | QA median ₹11,400/day, [FeeBee](https://www.flexingit.com/feebee/freelance-quality_assurance_testing-fees-id-87/) |
| Writing | ₹1,000/hr | Mid-level writers ₹1,035–1,786/hr, [solohourly](https://solohourly.com/rates/content-writer-rates-in-india) |

The hours are estimates as of version 2. Real hand-ins will show where they're off; fix them in the next version.

## How to price a task

1. **Find the closest anchor** in the tables below and use its price.
2. **Bundles add up.** A task that is clearly two anchors (say, two small features) is priced as their sum.
3. **Smaller than the smallest anchor:** use half or a quarter of it, nothing finer.
4. **Write the anchor on the issue,** e.g. `Priced against: C2 small feature (rate card v2), 1,500`, so anyone can check the price in one line.
5. **Price the result, never the person or the method.** Same price whoever does it and however they do it.

Pricing reads this file only. No web search per task.

## Changing prices

- **Untaken for 14 days:** an open task that nobody has picked moves up one anchor (or ×1.5 if it's already the top anchor of its role).
- **Customers decide in the end:** once a venture earns money, anchors for the kinds of work customers paid for move toward what they paid (NEKI.md, 2026-10-06).
- **Refresh:** re-check the sources every 6 months, or sooner if an anchor keeps getting bumped.
- **Versioned, never retroactive.** A change is a new version of this file. Accepted tasks keep the price they were accepted at; open tasks can be repriced to the new version.
- **Work done before 2025 uses the hand-work prices** (v1, table below). Agentic AI tools for this kind of work arrived in 2025 (Claude Code launched in February 2025), so earlier work really was done by hand and is priced the way it was made. Work goes by the date it was done, not by who says how it was done.

## Anchors

Rows marked **weak** rest on stand-ins or non-Indian data; replace them first.

### Code (`role:code`), ₹800/hr with AI

| Id | Result | Hours | Neki |
|---|---|---|---|
| C1 | Small bug fix or copy/config change in an existing web app | 1 | 800 |
| C2 | Small feature in an existing app (UI control + API route + DB column), with PR | 2 | 1,500 |
| C3 | Medium feature: new page or flow with backend, migration and email | 8 | 6,500 |
| C4 | Large feature or small app (dashboard, OAuth + webhooks integration) | 40 | 32,000 |

### Design (`role:design`), ₹1,500/hr with AI

| Id | Result | Hours | Neki |
|---|---|---|---|
| D1 | One screen, or a small UI fix, designed in Figma | 1 | 1,500 |
| D2 | User flow of about 5 screens | 4 | 6,000 |
| D3 | Landing page design, or logo + basic brand kit | 8 | 12,000 |
| D4 | Design system, or a full app UI of 15–25 screens | 24 | 36,000 |

### Research (`role:research`)

| Id | Result | Neki | How |
|---|---|---|---|
| R1 | Desk research memo: about 20 sourced items, summarised and checked | 3,000 | 3 hrs × ₹950 |
| R2 | Competitor analysis of 5–10 products | 7,500 | 8 hrs × ₹950 |
| R3 | 5 user interviews: recruit, run, synthesise | 55,000 | **Weak.** Talking to people, not shrunk by AI. Recruiting $49 per participant, [User Interviews via uxtweak](https://blog.uxtweak.com/user-interviews-pricing/), incentives, plus 3 researcher days at FeeBee's median. No Indian source |
| R4 | Market research report with a survey of 100+ responses | 40,000 | Panel of 200 × 15 questions ₹25,000–48,400, [GMO Research India](https://info.gmo-research.ai/en-in/en/quicksurvey-testb-in), plus 1 day of analysis |

### Tester (`role:tester`)

| Id | Result | Neki | How |
|---|---|---|---|
| T1 | One unmoderated test session (15–20 minutes, recorded, with notes) | 850 | **Weak.** A real person's session, not shrunk by AI. Global payouts: $10 per standard test, [UserTesting](https://help.usertesting.com/hc/articles/11880325020317); Testbirds €10–50, Userlytics $5–90, [finder](https://www.finder.com/make-money-online/how-to-earn-money-user-testing) |
| T2 | Exploratory QA of a small web app, with a bug report | 5,500 | 4 hrs × ₹1,400 |
| T3 | Full test plan plus a regression run of a web app | 22,500 | 16 hrs × ₹1,400 |

### People (`role:people`), not shrunk by AI

| Id | Result | Neki | Source |
|---|---|---|---|
| P1 | Community management for one week (Discord, WhatsApp) | 8,000 | **Weak.** Social media manager rates as a stand-in: freelancers ₹25,000–50,000 a month, [upgrowth](https://upgrowth.in/smm-agency-vs-freelancer-vs-inhouse/), ÷ 4.3 |
| P2 | Outreach campaign: 100 personalised messages plus follow-ups | 8,500 | **Weak.** AI drafts, a person sends and follows up. Marketplace outreach gigs $100–200 per project (search result, page not checked) |
| P3 | Recruit 10 people for something (sign-ups, interviewees) | none yet | No Indian source found. Until there is one, price as ½ × P2 and mark the issue `weak price` |

### Legal (`role:legal`), not shrunk by AI

| Id | Result | Neki | Source |
|---|---|---|---|
| L1 | Lawyer's review of a short contract | 5,000 | Average agreement ₹5,000, [LawRato](https://lawrato.com/startup-legal-advice/contarct-drafting-cost-for-a-private-limited-company-160674) (2023, drafting price used as a stand-in) |
| L2 | An agreement plus terms of service and a privacy policy, drafted with AI and reviewed by a lawyer | 10,000 | 2 × L1 |
| L3 | Private limited company incorporation (professional fee) | 10,000 | CA/CS fee ₹5,000–15,000, [Patron Accounting](https://www.patronaccounting.com/blog/private-limited-company-registration-cost-breakdown-government-fees); platforms from ₹2,899, [IndiaFilings](https://www.indiafilings.com/private-limited-company-registration). Government fees extra |

Co-op registration has no full-service price yet (only a ₹4,999 consultation, [SetIndiaBiz](https://www.setindiabiz.com/multi-state-co-operative-society-registration)).

### Writing (no role label yet; use the closest role), ₹1,000/hr with AI

| Id | Result | Hours | Neki |
|---|---|---|---|
| W1 | 1,000-word article or blog post | 2 | 2,000 |
| W2 | Copy for a 5-section landing page | 5 | 5,000 |

## Hand-work prices (v1), for work done before 2025

Same anchors, priced as hand work. Sources are the same as above (v1 in this file's history).

| Code | Neki | Design | Neki | Research | Neki | Writing | Neki |
|---|---|---|---|---|---|---|---|
| C1 | 3,000 | D1 | 3,000 | R1 | 11,000 | W1 | 5,000 |
| C2 | 10,000 | D2 | 15,000 | R2 | 22,500 | W2 | 30,000 |
| C3 | 50,000 | D3 | 25,000 | R3 | 55,000 | | |
| C4 | 1,50,000 | D4 | 40,000 | R4 | 55,000 | | |

Tester v1: T1 850, T2 11,400, T3 57,000. People v1: P1 8,000, P2 17,000, P3 ½ × P2. Legal v1: L1 5,000, L2 18,000, L3 10,000.

## Known gaps (fix in the next version)

- The with-AI hours are estimates; compare them against real hand-ins as tasks get done.
- Fiverr and Upwork blocked automated reading, so there's no per-gig data from India-based sellers yet.
- Weak rows: R3, T1, P1, P2, P3. Old sources (2023): L1.
- FeeBee's day rates average all experience levels, not only mid-level.

## History

- v2.1, 2026-10-09: work done before 2025 is priced on the v1 hand-work prices (Kamal: the 2022 work was built by hand, there was no Claude Code then).
- v2, 2026-10-08: anchors priced as work done with AI (Kamal: the unfollow task is 2–3 prompts, v1 priced it like weeks of hand work). Work AI barely shrinks kept v1 prices.
- v1, 2026-10-08: sourced freelancer prices for hand work. Spot-checked against FeeBee QA, Internshala and growai.

Researched by Claude for Kamal, 2026-10-08.
