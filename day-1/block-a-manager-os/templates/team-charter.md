# Team Charter Template

| Field | Your Entry |
|---|---|
| **Student Name** | Anton Shestakov|
| **Date** | 16.03.2026 |
| **Case Context** | Small (Seed-stage) / **Medium (Series B)** / Large (Enterprise) |

---

## Team Purpose & Mission

*Why does this analytics team exist? What value does it create for the organization? Write 2-3 sentences that a non-technical executive would understand.*

> Example (Acme Analytics, Medium — Series B Marketplace): Our team exists to make Acme's product and business decisions evidence-based. We provide trustworthy metrics, experimentation infrastructure, and analytical insights that help the Growth and Monetization pods move faster with less risk. We are the connective tissue between raw data and strategic decisions
> 

**Your purpose:**
The analytics team exists to turn messy data into a single, reliable source of metrics/information so leaders can stop debating numbers and start making profitable decisions.  We provide the map that shows exactly where to invest in customers and professionals to reach breakeven across all 12 markets. Our goal is to ensure every dollar spent on expansion is backed by facts, helping MarketBridge grow faster and more efficiently.

---

## Scope & Boundaries

*What is this team responsible for? Equally important: what is explicitly NOT your responsibility?*

| In Scope | Out of Scope |
|---|---|
| Metric Governance (creating and owning a reliable source of 'truth' for KPIs like Active Users) | Primarly wrangling the data within PostgreSQL or other data tool (incl. fixing bugs, data quality) |
| Self-service infrastructure: enabling project managers to independently manage their sales funnels and A/B testing results. | Operational CRM Management (we are note commited to managing sales workflow) |
| Marketplace Health: Integrating Salesforce (Supply) and Product (Demand) data to track supply-demand balance. | Defining Legal/Privacy Policy (determining GDPR requirements or consent policies) |
| | |
| | |

> **Tip:** Being explicit about what's OUT of scope is often more valuable than defining what's in scope. It prevents scope creep and sets clear expectations with stakeholders.

---

## Team Principles

*List 3-5 operating principles that guide how your team works. Good principles are specific, actionable, and occasionally uncomfortable. Avoid generic platitudes.*

> **Example principles (Acme Analytics):**
> 1. **Insights over outputs.** We measure our success by decisions influenced, not dashboards shipped. If an analysis doesn't lead to action, we ask why before starting the next one.
> 2. **Documented by default.** Every metric has a written definition, an owner, and a review date. Every major analysis has a written summary, not just a Slack message.
> 3. **We say no with context.** When we decline a request, we explain why and offer an alternative (self-serve resource, different timeline, or a scoped-down version).

**Your principles:**

1. Reliability: we turn the messy data into single 'source of trust'

2. One metric - one definition. We end the "my dashboard vs. someone's query" debate. If a core metric (like "active user" or "transaction volume") is not defined , it is not an official company metric. We commit to fixing the underlying data model rather than patching the reporting layer.

3. We do what useful: before strategy implementation we make sure it will be useful for the company by understanding the business problems and conducting a deep validation

4. We build a system and not one-off queries. If a metric or table is needed more than once, it’s captured in dbt, documented, and thoroughly validated.

5. *(optional)*

---

## Key Interfaces

*Who does your team interact with regularly? For each interface, describe the nature of the relationship and the primary mechanism for interaction.*

| Team / Role | Relationship | Interaction Mechanism | Frequency |
|---|---|---|---| 
| Sales Operations | They manage Salesforce and the supply-side data schemas. Because joining this with product data is currently a manual nightmare, we need tight alignment with them to fix the data model at the source. | Monthly CRM review | monthly |
| Raj Malhotra, CTO | Aligns analytics strategy with engineering, approves headcount, and reviews data stack budget. | Weekly 1:1s, monthly budget & vendor review | weekly |
| Diane Osei, VP product| she needs self-service tools and thorough A/B testing. We are bringing analysts on board to transition them from simply handling requests to providing strategic support. | Bi-weekly sprint planning, weekly metric alignment sync, shared Slack channel | weekly |
| Anya Petrov, Legal & Privacy | Critical for EU expansion. We integrate her privacy requirements directly into our data modeling and tracking plans. | pre-launch privacy sign-offs | *(Quarterly + ad-hoc)* | weekly
| 

---

## Success Metrics

*How will you know if your team is succeeding? Define 3-5 KPIs or OKRs for your team's first year. Mix leading indicators (process metrics) with lagging indicators (outcome metrics).*

> **Example (Acme Analytics):**
> - **Stakeholder NPS > 8** — Quarterly survey of primary stakeholders on analytics team effectiveness
> - **Time-to-insight < 2 days** for standard queries (current baseline: 5 days)
> - **80% of A/B tests** have a pre-registered analysis plan before launch
> - **Zero critical metric errors** in executive reporting (measured by corrections issued)

| # | Metric | Target | Current Baseline | Measurement Method |
|---|---|---|---|---|
| 1 | | | | |
| 2 | | | | |
| 3 | | | | |
| 4 | | | | |
| 5 | *(optional)* | | | |

---

## Cadences & Rituals

*What recurring meetings and practices will your team follow? Adapt to your case context — a 3-person startup team needs different cadences than a 15-person enterprise team.*

| Cadence | Ritual | Duration | Purpose | Attendees |
|---|---|---|---|---|
| **Daily** | *(e.g., Async standup in Slack)* | *(5 min)* | *(Visibility on blockers)* | *(Full team)* |
| **Weekly** | *(e.g., 1:1s)* | *(30 min each)* | *(Coaching, feedback, alignment)* | *(Manager + each report)* |
| **Weekly** | *(e.g., Team sync)* | *(45 min)* | *(Share learnings, coordinate)* | *(Full team)* |
| **Monthly** | *(e.g., Metrics review)* | *(60 min)* | *(Are we on track?)* | *(Team + stakeholders)* |
| **Quarterly** | *(e.g., Planning)* | *(Half day)* | *(Set priorities for next quarter)* | *(Team + sponsor)* |

---

## Evaluation Criteria

Use these dimensions to self-assess the quality of your Team Charter. For official grading criteria, see `assessment/grading-rubrics.md` (Manager OS component, 15%).

| Criterion | Weight | What "Good" Looks Like |
|---|---|---|
| **Specificity to case context** | 25% | The charter clearly reflects the constraints and opportunities of your chosen context (Small/Medium/Large). A reader could identify which context you chose without being told. |
| **Actionability of principles** | 20% | Principles are specific enough that a team member could use them to make a daily decision. No generic platitudes. |
| **Completeness of scope** | 20% | Both in-scope and out-of-scope are clearly defined. Key boundaries are drawn. |
| **Quality of success metrics** | 20% | Metrics are specific, measurable, and tied to business outcomes. Mix of leading and lagging indicators. |
| **Clarity of interfaces** | 15% | Key interfaces are identified with interaction mechanisms and frequency. No major stakeholders missing. |

**Note:** This is a draft artifact. You will refine it throughout the course and submit a polished version in your Manager Portfolio. The draft is assessed on completeness and thoughtfulness, not perfection.
