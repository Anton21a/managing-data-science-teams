# Job Description Template

**Student Name:** Anton Shestakov
**Date:** 16/03/2026
**Case Context:** [ ] Small (Seed-Stage) / [ ] Medium (Series B) / [ ] Large (Enterprise)
**Role Title:** Senior Analytics Engineer
**Level:** [ ] Junior / [ ] Mid / [Х] Senior / [ ] Staff/Principal

---

## Role Summary

*Write 2–3 sentences describing what this person does and why the role matters. Focus on impact, not activities.*

**Example:**
> We are hiring our first Analytics Engineer to build the data foundation that powers every product and business decision at [Company]. This person will own the pipeline from raw event data to trusted dashboards, working directly with founders and the product team to turn messy logs into actionable insights. This is a high-autonomy role where your work directly shapes company strategy.

Your Role Summary:

> We are hiring a Senior Analytics Engineer to clean up our messy data and build a single "source of truth" that everyone at MarketBridge can actually trust. You will fix our broken data models, untangle our metrics, and connect our product data with our financial data. By creating reliable, ready-to-use datasets, you will rescue our analysts from endless support tickets and give our leadership the accurate numbers they need to steer the business toward profitability.

---

## 90-Day Outcomes

*List 3–5 specific, measurable things this person will accomplish in their first 90 days. These are outcomes, not responsibilities — they describe results, not activities.*

**Example:**
> 1. Instrumented top-3 user flows with reliable event tracking (validated with product team)
> 2. Shipped a weekly KPI dashboard used by founders in Monday standups
> 3. Completed an audit of existing data sources and documented data quality issues
> 4. Scoped and designed the first A/B test for onboarding flow optimization
> 5. Established a repeatable process for ad-hoc analysis requests with a 48-hour SLA

Your 90-Day Outcomes:

1. Fixed and deployed the abandoned dbt project so that core data models run reliably every day without breaking.
2. Establish official definitions for the terms “active user” and “transaction volume” as the sole authoritative source of information, and secure formal approval from both the product team and the finance team to put an end to the confusion surrounding these metrics.
3. Built an automated dataset combining Salesforce provider profiles with product booking data, completely replacing the previous manual data integration process.
4. Delivered a clean, verified unit economics table in BigQuery that allows the CFO to easily track per-transaction margins by service category.
5. Converted the top 10 most common ad-hoc SQL requests into ready-to-use tables, noticeably reducing the ticket backlog for the existing analytics team.

---

## Key Responsibilities

*List 5–7 bullet points, ordered by priority (most important first). These describe ongoing responsibilities, not one-time tasks.*

**Example:**
> - Build and maintain the analytics data pipeline (event tracking, ETL, data warehouse)
> - Partner with Product to define metrics, instrument features, and analyze experiments
> - Create and maintain dashboards and reports for executive and team consumption
> - Conduct ad-hoc analyses to support business decisions (pricing, growth, retention)
> - Establish data quality standards and monitoring for critical metrics
> - Document data models, definitions, and methodologies for team use
> - Mentor future analytics team members as the team grows

Your Key Responsibilities:
- [ ] Manage the central data models (build and manage data transformation layer (using dbt and BigQuery) so the whole company is pulling from the same clean numbers).
- [ ] Standardize company metrics (act as the referee for our data by working with product, finance, and growth to define, build, and lock down official metrics, like "active user" or "transaction volume").
- [ ] Connect the marketplace (stitch together scattered data sources—specifically joining service provider data in Salesforce with company customer app data—into easy-to-use tables).
- [ ] Expand analytics team’s capabilities (create ready-to-use datasets that free in-house analysts from routine data collection tasks, allowing them to focus on long-term strategic analysis).
- [ ] Maintain quality and documentation (write clear documentation for data tables and set up alerts so we know immediately if a pipeline breaks).

---

## Required Qualifications

*Must-haves only. Be ruthlessly honest: if someone without an advanced degree could do this job, do not require an advanced degree. Each item should be directly tied to a 90-day outcome or key responsibility.*

**Example:**
> - 2+ years of professional experience in analytics, data science, or analytics engineering
> - Proficiency in SQL (complex queries, window functions, CTEs)
> - Experience building dashboards in at least one BI tool (Looker, Tableau, Metabase, etc.)
> - Demonstrated ability to communicate analytical findings to non-technical stakeholders
> - Comfort working with messy, incomplete data and ambiguous requirements

Your Required Qualifications:

- [ ] 3+ years of experience in analytics engineering or a heavy data modeling role, ideally at a fast-growing startup or marketplace.
- [ ] Advanced SQL skills and hands-on experience with dbt (to fix our broken dbt project on day one).
- [ ] Experience with cloud data warehouses (like BigQuery, Snowflake) and extracting data from complex sources like Salesforce, Stripe, or PostgreSQL.
- [ ] Proven ability to bring order to a sea of chaotic metrics. You have experience collaborating with various teams (such as product and finance) and reaching consensus among them on a single, shared definition of business metrics.
- [ ] Comfort with ambiguity and messy data. You don't need a perfect roadmap to get started; you know how to bring order to a patchwork data stack without getting overwhelmed.

---

## Preferred Qualifications

*Nice-to-haves that would accelerate ramp-up but are not dealbreakers. Be explicit that these are not required.*

**Example:**
> - Experience with dbt or similar analytics engineering tools
> - Familiarity with A/B testing methodology and statistical inference
> - Background in Python or R for data analysis
> - Previous experience in [your industry]
> - Experience working in an early-stage / high-growth / enterprise environment

Your Preferred Qualifications:

- [ ] Experience with two-sided marketplaces. If you already understand the dynamics of balancing supply and demand, booking conversion rates, and marketplace unit economics, it brings a big andvantage.
- [ ] Familiarity with GDPR and data privacy. We are launching in Europe soon; any prior experience managing data residency requirements or building privacy-compliant data models is a huge plus.
- [ ] Hands-on experience with Segment or Mixpanel. While your main focus will be the data warehouse, knowing how these specific tracking tools work will help you untangle our messy event logs and product dashboards.

---

## What We Offer

*Describe your compensation philosophy, growth opportunities, and team culture. Be specific rather than generic.*

**Example:**
> - Competitive salary benchmarked to [market/percentile] with equity participation
> - Direct access to founders and leadership — your analyses shape company direction
> - Budget for conferences, courses, and professional development
> - Flexible work arrangement: [remote/hybrid/in-office] with async-first communication
> - Opportunity to build the analytics function from the ground up

Your Offer:

- [ ] Competitive salary and Series B equity in a rapidly growing marketplace that is actively expanding into international markets.
- [ ] High-impact autonomy: You won't just be a ticket-taker maintaining legacy code. You will be the foundational builder of our modern data stack, with the authority to establish our engineering best practices.
- [ ] Direct partnership with firm's leadership: You will work directly with our VP of Product, CFO, and CTO, meaning your data models will directly shape the strategic decisions that drive our path to profitability.
- [ ] Flexible work arrangement: remote/hybrid/in-office with async-first communication


---

## About the Team

*Brief context about the team this person joins. Who will they work with? What is the team's current state? What is the team culture like?*

**Example:**
> You will be the first dedicated analytics hire, joining a product team of 8 engineers and 2 product managers. Today, analytics is done ad-hoc by engineers and founders using raw database queries. You will bring structure to this chaos. The culture values ownership, direct communication, and shipping — we would rather have a good-enough answer today than a perfect answer next month.

Your Team Context:

> You will report directly to the new Head of Analytics and work alongside three dedicated analysts who are currently embedded in our Product, Growth, and Operations teams. Right now, our analysts are bogged down by requests for data on specific queries and are forced to sift through disordered messy data. Your arrival marks a major turning point for us. You will be the technical foundation of the team, bringing engineering rigor to our data stack so our analysts can finally get back to doing deep, strategic work. We are in an active rebuilding phase—meaning you will have a massive amount of influence over our culture, our tooling, and how data gets done at MarketBridge. We value honest communication, practical problem-solving, and building things that last.

---

## Evaluation Criteria

Use these dimensions to self-assess your job description. For official grading criteria, see `assessment/grading-rubrics.md` (Hiring Packet component, 20%).

| Criterion | What We Are Looking For |
|:---|:---|
| **Outcome Orientation** | Are the 90-day outcomes specific, measurable, and realistic? Do they drive the rest of the document? |
| **Honest Scoping** | Are "required" qualifications truly required? Is the level appropriate for the outcomes described? |
| **Case Context Fit** | Does the JD reflect the specific constraints and opportunities of your chosen company context? |
| **Candidate Appeal** | Would a strong candidate reading this JD understand the role and be excited to apply? |
| **Completeness** | Are all sections filled in with thoughtful, specific content (not generic boilerplate)? |
