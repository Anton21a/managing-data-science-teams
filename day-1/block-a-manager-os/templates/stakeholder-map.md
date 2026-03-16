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
| 1 | **VP of Product** | H | H | Manage Closely | Self-serve dashboards PMs actually trust; rigorous A/B testing platform. | Political capital to defend time spent on infrastructure; enforcement of tool adoption. | Weekly 1:1; monthly metrics review; shared Slack channel. |
| 2 | **CTO** (Your Manager) | H | H | Manage Closely | Rationalized data stack; cost control (staying under $25k/mo); functioning dbt models. | Approval for the 2 new hires; budget sign-off; air cover from board pressure. | Weekly 1:1; monthly budget & vendor review. |
| 3 | **CFO** | H | H | Manage Closely | Unit economics at the market level; integrated product and financial data (BigQuery + NetSuite). | Clear financial formulas; access to baseline NetSuite data models. | Monthly business review (MBR) prep; metric definition sign-offs. |
| 4 | **Head of Growth** | H | H | Manage Closely | Multi-touch attribution models (CAC/LTV); baseline metrics for Atlanta/EU launches. | Clear channel definitions; advance notice of marketing campaigns. | Weekly growth pod sync; campaign performance reviews. |
| 5 | **Legal and Privacy Officer** | H | L | Keep Satisfied | Systematic privacy controls; clear data inventory for GDPR audit; EU data residency compliance. | Clear, upfront constraints (not just end-of-process vetoes); design partnership. | Bi-weekly architecture review; pre-launch privacy sign-offs. |
| 6 | **Backend / Platform Engineering** | H | L | Keep Satisfied | Minimal load on the Postgres read replica; clean tracking implementation specs. | Notifications before database schema changes; timely fixes to broken Fivetran/Segment pipes. | Async Slack channel alerts; Jira tickets for pipeline requests. |
| 7 | **Sales Operations** | L | H | Keep Informed | Reliable joins between their supply-side CRM data and demand-side product data. | Clean Salesforce schema management; documentation of custom fields. | Monthly CRM data mapping sync; Jira alerts for CRM changes. |
| 8 | **Product Managers** | L | H | Keep Informed | Fast turnaround on ad-hoc queries; an analytics tool that matches the database. | Clear hypotheses; willingness to learn self-serve tools instead of filing tickets. | Embedded analyst support; weekly sprint planning. |


#,Stakeholder (Role),Power (H/L),Interest (H/L),Quadrant,What They Need From You,What You Need From Them,Engagement Strategy
1,VP of Product,H,H,Manage Closely,Self-serve dashboards PMs actually trust; rigorous A/B testing platform.,Political capital to defend time spent on infrastructure; enforcement of tool adoption.,Weekly 1:1; monthly metrics review; shared Slack channel.
2,CTO (Your Manager),H,H,Manage Closely,Rationalized data stack; cost control (staying under $25k/mo); functioning dbt models.,Approval for the 2 new hires; budget sign-off; air cover from board pressure.,Weekly 1:1; monthly budget & vendor review.
3,CFO,H,H,Manage Closely,Unit economics at the market level; integrated product and financial data (BigQuery + NetSuite).,Clear financial formulas; access to baseline NetSuite data models.,Monthly business review (MBR) prep; metric definition sign-offs.
4,Head of Growth,H,H,Manage Closely,Multi-touch attribution models (CAC/LTV); baseline metrics for Atlanta/EU launches.,Clear channel definitions; advance notice of marketing campaigns.,Weekly growth pod sync; campaign performance reviews.
5,Legal and Privacy Officer,H,L,Keep Satisfied,Systematic privacy controls; clear data inventory for GDPR audit; EU data residency compliance.,"Clear, upfront constraints (not just end-of-process vetoes); design partnership.",Bi-weekly architecture review; pre-launch privacy sign-offs.
6,Backend / Platform Engineering,H,L,Keep Satisfied,Minimal load on the Postgres read replica; clean tracking implementation specs.,Notifications before database schema changes; timely fixes to broken Fivetran/Segment pipes.,Async Slack channel alerts; Jira tickets for pipeline requests.
7,Sales Operations,L,H,Keep Informed,Reliable joins between their supply-side CRM data and demand-side product data.,Clean Salesforce schema management; documentation of custom fields.,Monthly CRM data mapping sync; Jira alerts for CRM changes.
8,Product Managers,L,H,Keep Informed,Fast turnaround on ad-hoc queries; an analytics tool that matches the database.,Clear hypotheses; willingness to learn self-serve tools instead of filing tickets.,Embedded analyst support; weekly sprint planning.
**Stakeholders you might be missing:** IT/Infrastructure, Legal/Privacy, Finance/FP&A, Customer Success, Sales, HR/People Ops, External vendors, Board members or investors (for startups), Compliance/Audit (for enterprise), AI/ML platform owner or LLM/API budget controller.

---

## Key Relationships

*For your top 3 most critical stakeholders (those in "Manage Closely"), provide a deeper analysis.*

### Stakeholder 1: Head of Sales Operation

- **Why they matter:** They own Salesforce, which houses all the critical supply-side data (service professional profiles, pipelines, availability). If we cannot integrate this data with the product (demand-side) data, MarketBridge cannot provide a reliable analytics as a primary function.
- **Current state of the relationship:** *(Strong / Neutral / Needs work / Unknown)*
- **Their goals:** *(What are they personally measured on?)*
- **Potential friction points:** *(Where might your team's interests conflict with theirs?)*
- **Your strategy:** *(Specific actions you'll take in the first 30 days)*

### Stakeholder 2: Head of Customer Safety & Support

- **Why they matter:** We send basically strangers (like plumbers and cleaners) into people's homes. If safety issues happen or bad reviews pile up, the company's reputation is ruined.
- **Current state of the relationship:**
- **Their goals:** Keep customers happy, ensure high ratings, and quickly kick dangerous or bad professionals off the app.
- **Potential friction points:** They need instant alerts when a pro gets a 1-star review. Our current data pipes are fragile and sometimes break for days, so we can't give them real-time alerts yet.
- **Your strategy:**

### Stakeholder 3: VP of Sales

- **Why they matter:** An app for booking plumbers is useless if there are no plumbers on it. This leader's team is responsible for convincing professionals to join the platform and pay the monthly fee, which is crucial for the new Atlanta and Europe launches.
- **Current state of the relationship:**
- **Their goals:** Hit sign-up targets for the new cities and keep the cost of finding new professionals low.
- **Potential friction points:**
- **Your strategy:**

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
