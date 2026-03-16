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

*For your top 3 most critical stakeholders (those in "Manage Closely"), provide a deeper analysis.*

### Stakeholder 1: Head of Sales Operation

- **Why they matter:** They own Salesforce, which houses all the critical supply-side data (service professional profiles, pipelines, availability). If we cannot integrate this data with the product (demand-side) data, MarketBridge cannot provide a reliable analytics as a primary function.
- **Current state of the relationship:** **Needs work.** Joining supply-side Salesforce data with demand-side product data currently requires fragile, manual mapping that only one analyst knows how to do. The Salesforce data model is complex and poorly documented.
- **Their goals:** Ensuring CRM data hygiene, maximizing sales team productivity, and tracking the supply-side funnel (leads to paying subscribers).
- **Potential friction points:** Analytics needs strict governance over Salesforce schemas to prevent broken pipelines, while Sales Ops often wants to add custom fields or change workflows quickly to support new sales motions.
- **Your strategy:** Set up a bi-weekly CRM sync within the first two weeks. Identify the top 5-10 mission-critical Salesforce fields needed for the marketplace health metrics and lock them down. Establish a mandatory "schema change notification" process via Jira before any custom fields are altered in Salesforce.

### Stakeholder 2: Head of Customer Safety & Support

- **Why they matter:** We send basically strangers (like plumbers and cleaners) into people's homes. If safety issues happen or bad reviews pile up, the company's reputation is ruined.
- **Current state of the relationship:** **Strained.** Fivetran syncs are lightly monitored and breakages sometimes go unnoticed for days, meaning they cannot rely on data for timely interventions.
- **Their goals:** Keep customers happy, ensure high ratings, and quickly kick dangerous or bad professionals off the app. Maintain strict compliance and trust.
- **Potential friction points:** They need instant or near-real-time alerts when a pro gets a 1-star review or safety flag. However, our current batch-based warehouse stack (Fivetran/BigQuery) is not built for real-time operational alerting, and fixing the foundational dbt models will take priority over building new custom alert systems.
- **Your strategy:** In the first 30 days, audit the specific Segment events tied to reviews and safety flags. Implement basic monitoring (like dbt source freshness or Fivetran alerts) to guarantee that critical support data is at least reliably synced daily. Have a candid conversation to set realistic expectations about the timeline for moving from "reliable daily data" to "real-time alerts."

### Stakeholder 3: VP of Sales

- **Why they matter:** An app for booking plumbers is useless if there are no plumbers on it. This leader's team is responsible for convincing professionals to join the platform and pay the monthly fee, which is crucial for the new Atlanta and Europe launches.
- **Current state of the relationship:** **Neutral, but high-pressure.** The rapid expansion into Atlanta, Berlin, and Amsterdam puts immense pressure on this team, and they are flying blind without integrated marketplace metrics.
- **Their goals:** Hit sign-up targets for the new cities, keep the cost of finding new professionals (supply-side CAC) low, and maximize monthly subscription revenue from premium placements.
- **Potential friction points:** They need fast, granular reporting for the new EU and Atlanta markets. However, the EU expansion requires strict GDPR and data residency compliance (storing data in the EU) which will significantly slow down how quickly we can build their dashboards.
- **Your strategy:** During the first 30 days, define exactly what baseline metrics are required for "Day 1" of the Atlanta and EU launches. Work with Legal/Privacy (Anya) immediately to map out how supply-side pipeline data will be legally collected in Berlin and Amsterdam so the Sales team isn't blocked by a last-minute privacy veto.
---

## Communication Plan

*How often and through what channels will you communicate with each quadrant?*

| Quadrant | Frequency | Channel | Content | Owner |
|---|---|---|---|---|
| **Manage Closely** | *(e.g., Weekly)* | *(e.g., 1:1 meeting + Slack DM)* | *(e.g., Progress on key metrics, blockers, decisions needed)* | *(You)* |
| **Keep Satisfied** | *(e.g., Monthly)* | *(e.g., Monthly email digest + quarterly meeting)* | *(e.g., Summary of team output, resource needs, upcoming asks)* | *(You)* |
| **Keep Informed** | *(e.g., Bi-weekly)* | *(e.g., Team newsletter or Slack channel)* | *(e.g., New dashboards, methodology updates, available capacity)* | *(Team member)* |
| **Monitor** | *(e.g., Quarterly)* | *(e.g., All-hands presentation or shared doc)* | *(e.g., Team highlights, impact stories)* | *(You or team member)* |

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
