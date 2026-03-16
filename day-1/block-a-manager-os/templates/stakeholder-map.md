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

Deep dive into the top 3 "Manage Closely" stakeholders.

### Stakeholder 1: CTO

**Why they matter:** Direct manager, controls budget and headcount approvals. Without his cover, nothing gets built.
**Current state:** Neutral / Unknown
**Their goals:** Cost control, maintainable stack, no runaway data spend
**Potential friction points:** Any proposal that adds tooling without sunsetting something else; hire justifications that aren't airtight
**30-day strategy:** Map the $25k/mo spend across Segment, Fivetran, Mixpanel, and BigQuery. Identify the 30% redundant Segment events for immediate deactivation to cut costs.

### Stakeholder 2: VP of Product

**Why they matter:** Most political capital in the building, willing to spend it for you — but only if she sees fast, visible progress
**Current state:** Neutral, leaning positive
**Their goals:** PM self-serve, reliable A/B testing, faster data-driven decisions
**Potential friction points:** She wants dashboards now; you need to fix metric trust first — shipping on a broken foundation will backfire
**30-day strategy:** Standardize the "Active User" definition in dbt. Decide on the Mixpanel renewal within 6 weeks to provide a stable "Single Source of Truth."

### Stakeholder 3: Head of Growth

**Why they matter:** Three market launches this year — he needs attribution and baseline metrics before launch, not after
**Current state:** Unknown, likely skeptical given the long-standing attribution gap
**Their goals:** Reliable CAC by channel, LTV/CAC ratios to justify spend to CFO
**Potential friction points:** Will push for multi-touch attribution faster than it can be responsibly delivered; campaigns launched without analytics notice break tracking retroactively
**30-day strategy:** Prioritize a robust attribution model in the warehouse. Provide "Day 1" dashboards for the Atlanta and EU launches to track early health.

---

## Communication Plan

*How often and through what channels will you communicate with each quadrant?*

| Quadrant | Frequency | Channel | Content | Owner |
|---|---|---|---|---|
| **Manage Closely** <br>*(CTO, VP Product, CFO, Head of Growth)* | Weekly / Monthly | Weekly 1:1s, Monthly Metrics Review, MBRs | Progress on core KPIs, budget updates, EU expansion readiness, and critical blockers. | You (Head of Analytics) |
| **Keep Satisfied** <br>*(Legal/Privacy, Backend Eng)* | Bi-weekly / Ad-hoc | Jira, async Slack | GDPR compliance updates, data residency architecture, schema change notifications, and pipeline health. | You (Head of Analytics) |
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
