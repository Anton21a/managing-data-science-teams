# 12-Month Analytics Roadmap with RICE Prioritization

**Student Name:** Anton Shestakov

**Date:** 16.03.2026

**Case Context:** [ ] Small (DataPulse) | [X] Medium (MarketBridge) | [ ] Large (FinGuard)

---

## North Star Metric

**What is your North Star metric?**
_The single number that best captures the value your analytics team delivers to the business._

| Element | Your Answer |
|---------|-------------|
| **Metric name** | Lifetime Value to Customer Acquisition Cost (how much money a customer brings us to how much we spent on ads/sales to get them|
| **Current baseline** | ~1.1x (MarketBridge is cash-flow negative but "approaching breakeven in mature markets," suggesting current unit economics are marginal and heavily dragged down by inefficient acquisition and disconnected tracking) |
| **Target (end of 12 months)** | 2x + |
| **Why this metric?** | It matters because it gives the Board and CFO exactly what they want: proof that we are on track to make profit
| **How is it measured?** | We calculate it every week in our central database. We simply take the total profit a customer brings in and divide it by what we spent on ads and sales to get them.

**Example (DataPulse):** North Star = Monthly Active Paying Users (MAPU). Current baseline: ~1,600 (50K MAU x 3.2% conversion). 12-month target: 5,000+. This is the metric investors care about most and directly drives revenue.

---

## Guardrail Metrics

_Guardrails are metrics that must NOT get worse while you optimize the North Star. List 3-5._

| # | Guardrail Metric | Current Baseline | Threshold (Must Not Fall Below) | Why It Matters |
|---|-----------------|-----------------|-------------------------------|----------------|
| 1 | Total Monthly Data Tooling Cost | ~$25,000 | Max $25,000/month | The CTO has made it clear that costs are heavily scrutinized. We cannot achieve our North Star by simply buying more tools or running expensive, bloated queries |
| 2 | Core Data Pipeline Uptime | Poor (breaks currently go unnoticed for days) | >99% uptime for Tier 1 reports | If we build a brilliant profitability model but let the daily data syncs keep breaking, the Product team will continue to distrust the dashboards and use their own spreadsheets |
| 3 | Analyst Time on Ad-Hoc Requests | ~80%+ of their week | Less than 40% of their week | The team is already treated like "ticket-takers" (according to the business context). So we cannot reach the North Star by burning them out; we must force a shift toward automated data |
| 4 | | | | |
| 5 | | | | |

**Guidance:** Common guardrails for analytics teams include data quality SLAs (e.g., dashboard uptime > 99%), stakeholder satisfaction scores, query performance benchmarks, model fairness metrics, and data freshness guarantees. Choose guardrails that represent real risks of over-optimizing your North Star.

---

## RICE Scoring Table

_Score each initiative using the RICE framework. Then sort by RICE score to inform your Now/Next/Later placement._

**Scoring Guide:**
- **Reach:** Number of people, decisions, or dollars affected per quarter
- **Impact:** 3 = massive, 2 = high, 1 = medium, 0.5 = low, 0.25 = minimal
- **Confidence:** 100% = high certainty, 80% = reasonable, 50% = speculative
- **Effort:** Person-months of work required (include compute costs where significant)
- **RICE Score:** (Reach x Impact x Confidence) / Effort

| # | Initiative | Reach | Impact | Confidence | Effort | RICE Score | Horizon |
|---|-----------|-------|--------|------------|--------|------------|---------|
| 1 | **Standardize Core Metrics** (Define "Active Users" & "Transactions" with leaders) | 100 | 3 | 100% | 0.5 | 600 | **Now** |
| 2 | **Single Data Request Form** (Route all asks via Jira/Slack to protect analysts) | 50 | 2 | 100% | 0.25 | 400 | **Now** |
| 3 | **Segment Event Cleanup** (Delete 30% of unused events to cut costs) | 100 | 2 | 100% | 1.0 | 200 | **Now** |
| 4 | **Mixpanel Renewal Decision** (Evaluate renewal vs. migration before 6-week deadline) | 50 | 3 | 80% | 1.0 | 120 | **Now** |
| 5 | **Atlanta Launch Dashboard** (Automate baseline reports for the new market) | 20 | 2 | 100% | 0.5 | 80 | **Now** |
| 6 | **Fix Core dbt Models** (Repair broken pipelines and map metrics in BigQuery) | 100 | 3 | 80% | 2.0 | 120 | **Next** |
| 7 | **EU GDPR Architecture** (Design compliant data flows for Berlin & Amsterdam) | 100 | 3 | 80% | 2.5 | 96 | **Next** |
| 8 | **Salesforce Data Sync** (Connect supply-side CRM data to product data in BigQuery) | 50 | 2 | 80% | 2.0 | 40 | **Next** |
| 9 | **Multi-Touch Attribution** (Calculate accurate CAC/LTV by marketing channel) | 50 | 3 | 50% | 3.0 | 25 | **Later** |

_Add more rows as needed. You need at least 8 initiatives._

**Note:** The RICE score informs but does not dictate the Horizon. A high-scoring initiative with a critical dependency might be placed in Next rather than Now. A lower-scoring initiative might be in Now because it unblocks higher-value work. Document your reasoning when the placement deviates from the score ranking.

---

## Roadmap Visualization

*Place your initiatives in the appropriate horizon. Include the RICE rank for reference.*

### Now (This Quarter — Committed)
*These are actively staffed and in progress. You are accountable for delivering these.*

| Initiative (RICE Rank) | Size (S/M/L/XL) | Key Dependency | Expected Outcome |
|-------------------------|-----------------|----------------|------------------|
| **1. Standardize Core Metrics** (#1) | S | CFO & VP Product sign-off | Single source of truth for executive reporting. |
| **2. Single Data Request Form** (#2) | S | Stakeholder adoption | 50% reduction in random Slack interruptions. |
| **3. Segment Event Cleanup** (#3) | M | Platform Engineering (to remove code) | Reduced tracking costs and trusted event data. |
| **4. Mixpanel Renewal Decision** (#4) | M | CTO budget approval & Vendor terms | Final decision made before the 6-week deadline. |
| **5. Atlanta Launch Dashboard** (#5) | S | Base event data availability | Day 1 reporting ready for the VP of Sales and Ops. |

### Next (Next Quarter — Planned)
_These are scoped and ready to start. They move into Now when the current quarter's work is complete._

| Initiative (RICE Rank) | Size (S/M/L/XL) | Key Dependency | Expected Outcome |
|-------------------------|-----------------|----------------|------------------|
| **6. Fix Core dbt Models** (#6) | L | Upstream schema stability | Reliable warehouse foundation and automated core metrics. |
| **7. EU GDPR Architecture** (#7) | XL | Legal approval | Unblocked Berlin and Amsterdam launches with full compliance. |
| **8. Salesforce Data Sync** (#8) | L | Sales Ops schema lock | Automated marketplace health tracking (supply vs. demand). ||

### Later (6-12 Months — Exploratory)
*These are directional. Details are intentionally vague. They represent where the team is heading.*

| Initiative (RICE Rank) | Size (S/M/L/XL) | Key Dependency | Expected Outcome |
|-------------------------|-----------------|----------------|------------------|
| **9. Multi-Touch Attribution** (#9) | XL | Clean marketing channel data | Accurate CAC and LTV reporting for the Growth team. |
| **10. Finance NetSuite Integration** | XL | Core dbt metric stabilization | Fully automated unit economics and transaction margins. |
| **11. A/B Testing Platform** | L | Tooling decision (Mixpanel vs. Warehouse) | Product Managers can launch and evaluate experiments self-serve. ||

---

## Dependencies and Sequencing

*What depends on what? Identify the critical path through your roadmap.*

### Key Dependencies

| Initiative | Depends On | Type | Risk if Delayed |
|-----------|-----------|------|----------------|
| **Fix Core dbt Models** | **Standardize Core Metrics** | Data | Dashboards stay broken and leaders keep arguing about the numbers. |
| **Atlanta Launch Dashboard** | **Standardize Core Metrics** | Data | The team launches the new city completely blind without data. |
| **EU GDPR Architecture** | **Legal (Anya) Requirements** | Stakeholder / Technical | EU market launches are blocked by Legal, or we risk huge GDPR fines. |
| **Mixpanel Renewal** | **CTO & VP Product Alignment** | Stakeholder | We overpay for a tool we don't need, or the Product team loses analytics access. |
| **Multi-Touch Attribution** | **Fix Core dbt Models & Salesforce Sync** | Technical / Data | Marketing wastes money because we can't track true customer value (CAC/LTV). |

### Sequencing Notes

* **The Critical Path (Do First):** We cannot write code until leaders agree on what we are measuring. **Standardizing Core Metrics** must happen before we touch the **dbt Models** or build the **Atlanta Launch Dashboard**. The **Mixpanel Renewal Decision** is also on a strict 6-week countdown and must be finalized immediately.
* **Parallel Work:** While leadership is debating metrics and tool contracts, the analyst team can immediately tackle the **Segment Event Cleanup** and roll out the **Single Data Request Form** to stop the daily chaos.
* **Bottleneck Warning:** The Growth team urgently wants **Multi-Touch Attribution**, but we cannot build it until both the **dbt Models** and the **Salesforce Data Sync** are finished. We must explicitly delay this request until the data foundation is stable.

## Metrics Tree

_Draw the connection from business outcome to team activities._

```
Business Outcome:  [What the CEO/board cares about]
                        │
North Star:        [Your North Star metric]
                   ╱              ╲
Input Metrics: [Metric A]      [Metric B]
                   │                │
Team Activities: [Activity 1]   [Activity 3]
                 [Activity 2]   [Activity 4]



Business Outcome:  Market Level Profitability (Breakeven in all 12+ metros)
                        │
North Star:        LTV:CAC Ratio (Target: 2.0x+)
                   ╱            ╲
Input Metrics: [100% Tier 1 Metrics in dbt]   [<40% Time on Ad-Hoc Requests]
                   │                             │
Team Activities: [Standardize Core Metrics]   [Implement an appointment request form]
                 [Fix Core dbt Models]        [Build Self-Serve Dashboards]
                 [Salesforce Data Sync]       [Segment Event Cleanup]
```

_Replace the placeholders above with your actual metrics tree._

---

## Evaluation Criteria

This artifact will be assessed as part of the Roadmap + Exec Narrative portfolio component (20% of course grade). For the Day 1 Checkpoint (10%, pass/fail), only completeness is assessed — all sections must have content.

**For the final portfolio submission, this roadmap will be evaluated on:**

| Criterion | Excellent | Good | Needs Work |
|-----------|-----------|------|------------|
| **North Star & Guardrails** | Clear metric with baseline and target; guardrails protect against obvious over-optimization risks | Metric identified but baseline or target is vague; guardrails present but not well-justified | Missing baseline/target; guardrails absent or unrelated to North Star |
| **RICE Scoring** | 8+ initiatives scored with plausible estimates; scoring drives meaningful prioritization discussion | 8 initiatives scored but estimates feel arbitrary; limited connection between scores and placement | Fewer than 8 initiatives or RICE applied mechanically without judgment |
| **Now/Next/Later Placement** | Placement is defensible; deviations from RICE ranking are explained; realistic given team size | Placement follows RICE scores but lacks nuance about dependencies or team capacity | Placement feels random or disconnected from scores |
| **Dependencies** | Critical path is clear; external dependencies identified; realistic about what blocks what | Some dependencies noted but not systematically mapped | Dependencies not addressed |
| **Business Alignment** | Every initiative connects clearly to business outcomes; a VP could read this and understand why | Most initiatives have business rationale; some feel like internal projects | Roadmap reads like a technical task list, not a business strategy |
