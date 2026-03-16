# Stakeholder Map Template

| Field | Your Entry |
|---|---|
| **Student Name** | Anton Shestakov|
| **Date** | 16/03/2026 |
| **Case Context** | Small (Seed-stage) / **Medium (Series B)** / Large (Enterprise) |

---

## Power/Interest Grid

*Place each stakeholder's number (from the registry below) into the appropriate quadrant.*
List: 

1. Diane Osei (VP of Product)
2. Raj Malhotra (CTO)
3. Marco Reyes (Head of Growth)
4. Christine Park (CFO)
5. Anya Petrov (Legal and Privacy Officer)
6. Product Managers (Diane's team)
7. Sales Operations Team
8. Backend/Platform Engineering
```
                        INTEREST IN ANALYTICS
                    Low                     High
                ┌───────────────────┬───────────────────┐
                │                   │                   │
   High         │  KEEP SATISFIED   │  MANAGE CLOSELY   │
                │                   │                   │
                │  Strategy: Meet   │  Strategy: Regular │
 POWER          │  their needs,     │  engagement, deep  │
                │  minimal noise    │  relationship      │
                │                   │                   │
                │  Stakeholders: 5    │  Stakeholders:   |
                |                   |        1,2,3,4     │
                │                   │                   │
                ├───────────────────┼───────────────────┤
                │                   │                   │
   Low          │  MONITOR          │  KEEP INFORMED    │
                │                   │                   │
                │  Strategy:        │  Strategy: Regular │
                │  Periodic check,  │  updates, leverage │
                │  low effort       │  their enthusiasm  │
                │                   │                   │
                │  Stakeholders: 8   │  Stakeholders: 6, 7 │
                │                   │                   │
                └───────────────────┴───────────────────┘
```

---

## Stakeholder Registry

## Stakeholder Registry

*List at least 6 stakeholders. Use roles, not names (e.g., "VP of Product" not "Sarah"). For each, assess their power over your team and their interest in your work.*

| # | Stakeholder (Role) | Power (H/L) | Interest (H/L) | Quadrant | What They Need From You | What You Need From Them | Engagement Strategy |
|---|---|---|---|---|---|---|---|
| 1 | **VP of Product** | H | H | Manage Closely | Self-serve dashboards PMs actually trust; rigorous A/B testing platform. | Political capital to defend time spent on infrastructure | Weekly 1:1; monthly metrics review; shared Slack channel. |
| 2 | **CTO**  | H | H | Manage Closely | Rationalized data stack; cost control (staying under $25k/mo); functioning dbt models. | Approval for the 2 new hires; budget sign-off; air cover from board pressure. | Weekly 1:1; monthly budget & vendor review. |
| 3 | **CFO** | H | H | Manage Closely | Unit economics at the market level; integrated product and financial data (BigQuery + NetSuite). | Access to baseline NetSuite data models. | Monthly business review prep |
| 4 | **Head of Growth** | H | H | Manage Closely | Multi-touch attribution models; baseline metrics for Atlanta/EU launches. | Clear channel definitions; advance notice of marketing campaigns. | Weekly growth pod sync; campaign performance reviews. |
| 5 | **Legal and Privacy Officer** | H | L | Keep Satisfied | Systematic privacy controls; clear data inventory for GDPR audit | Clear, upfront constraint; design partnership. | Bi-weekly architecture review; pre-launch privacy sign-offs. |
| 6 | **Backend / Platform Engineering** | H | L | Keep Satisfied | Minimal load on the Postgres read replica; clean tracking implementation specs. | Notifications before database schema changes; timely fixes to broken Fivetran/Segment pipes. | Async Slack channel alerts; Jira tickets for pipeline requests. |


**Stakeholders you might be missing:** IT/Infrastructure, Legal/Privacy, Finance/FP&A, Customer Success, Sales, HR/People Ops, External vendors, Board members or investors (for startups), Compliance/Audit (for enterprise), AI/ML platform owner or LLM/API budget controller.

---

## Key Relationships

*Deep dive into the top 3 "Manage Closely" stakeholders.*

### 1. Head of Sales Operations
- **Why they matter:** Owns Salesforce. Crucial for full marketplace analytics.
- **Current state:** **Needs work.** Data mapping is highly manual, complex, and poorly documented.
- **Their goals:** CRM data hygiene, sales productivity, tracking the supply funnel.
- **Friction points:** We need strict schema governance; they want flexibility to change CRM fields quickly.
- **Your strategy:** Set up a bi-weekly sync. Lock down the top 5-10 critical Salesforce fields. Implement a mandatory Jira approval process for any CRM schema changes.

### 2. Head of Customer Safety & Support
- **Why they matter:** Protects company reputation by ensuring professionals in homes are safe and vetted.
- **Current state:** **Strained.** Unmonitored pipeline breakages delay critical safety data.
- **Their goals:** High customer ratings, user safety, and swift removal of bad actors.
- **Friction points:** They want real-time alerts; our current batch-based warehouse (BigQuery) can only guarantee daily updates until the foundation is fixed.
- **Your strategy:** Audit safety-related events in Segment. Set up daily data freshness alerts. Have a candid talk to manage expectations regarding the timeline for real-time reporting.

### 3. VP of Sales
- **Why they matter:** Responsible for acquiring professionals, which is the lifeblood of our new Atlanta and EU market launches.
- **Current state:** **Neutral, but high-pressure.** They are launching new markets while flying blind without metrics.
- **Their goals:** Hit sign-up targets, lower acquisition costs, and maximize subscription revenue.
- **Friction points:** They need fast dashboards; strict EU GDPR and data residency rules will slow us down.
- **Your strategy:** Define "Day 1" baseline metrics for the new markets immediately. Partner with Legal to map out compliant data collection in the EU so privacy rules don't block the sales rollout.
---

## Communication Plan

*How often and through what channels will you communicate with each quadrant?*

| Quadrant | Frequency | Channel | Content | Owner |
|---|---|---|---|---|
| **Manage Closely** | *(e.g., Weekly)* | *(e.g., 1:1 meeting + Slack DM)* | *(e.g., Progress on key metrics, blockers, decisions needed)* | *(You)* |
| **Keep Satisfied** | *(e.g., Monthly)* | *(e.g., Monthly email digest + quarterly meeting)* | *(e.g., Summary of team output, resource needs, upcoming asks)* | *(You)* |
| **Keep Informed** | *(e.g., Bi-weekly)* | *(e.g., Team newsletter or Slack channel)* | *(e.g., New dashboards, methodology updates, available capacity)* | *(Team member)* |
| **Monitor** | *(e.g., Quarterly)* | *(e.g., All-hands presentation or shared doc)* | *(e.g., Team highlights, impact stories)* | *(You or team member)* |



| Quadrant | Frequency | Channel | Content | Owner |
|---|---|---|---|---|
| **Manage Closely** <br>*(CTO, VP Product, CFO, Head of Growth)* | Weekly / Monthly | Weekly 1:1s, Monthly Metrics Review, MBRs | Progress on core KPIs, budget updates (e.g., Mixpanel), EU expansion readiness, and critical blockers. | You (Head of Analytics) |
| **Keep Satisfied** <br>*(Legal/Privacy, Backend Eng)* | Bi-weekly / Ad-hoc | Architecture syncs, Jira tickets, async Slack | GDPR compliance updates, data residency architecture, schema change notifications, and pipeline health. | You (Head of Analytics) |
| **Keep Informed** <br>*(PMs, Sales Ops)* | Bi-weekly | Sprint reviews, `#data-updates` Slack channel | Releases of new self-serve dashboards, dbt model updates, metric definition changes, and CRM mapping fixes. | Embedded Analysts |
| **Monitor** <br>*(General Managers, Broad Company)* | Monthly / Quarterly | Automated Slack alerts, Quarterly All-Hands | High-level marketplace health metrics (supply/demand balance), major data team wins, and system uptime. | You or Senior Analyst |
---

## Evaluation Criteria

Use these dimensions to self-assess the quality of your Stakeholder Map. For official grading criteria, see `assessment/grading-rubrics.md` (Manager OS component, 15%).

| Criterion | Weight | What "Good" Looks Like |
|---|---|---|
| **Completeness** | 25% | At least 6 stakeholders identified, covering multiple functions (not just Product). Includes non-obvious stakeholders (IT, Legal, Finance, etc.). |
| **Accuracy of power/interest assessment** | 20% | Power and interest levels are realistic for the case context. A startup CEO is high power; a junior PM is not. Assessments are justified. |
| **Quality of needs analysis** | 20% | "What they need from you" and "What you need from them" are specific and actionable, not vague. |
| **Engagement strategy specificity** | 20% | Strategies include concrete actions (frequency, channel, content), not just "build relationship." |
| **Key relationship depth** | 15% | Top 3 stakeholder analyses show genuine strategic thinking — friction points, personal goals, specific 30-day actions. |

**Note:** This is a draft artifact. You will refine it throughout the course and submit a polished version in your Manager Portfolio. The draft is assessed on completeness and thoughtfulness, not perfection.
