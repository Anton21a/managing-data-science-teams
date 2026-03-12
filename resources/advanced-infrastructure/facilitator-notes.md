# Facilitator Notes — Advanced Resources: XFN, Vendor, IT & Data Infrastructure

**Optional self-study module (not scheduled as an in-class block)**

---

## Setup (if taught as a live workshop)

_The guidance below applies if this module is taught as a live session. For self-study, students only need access to the templates and slides._

- **Room:** Ensure projector is working and slides are loaded. Have the data infrastructure blueprint slides (Slides 23–24) ready as a persistent reference — consider printing it or keeping it visible on a secondary screen.
- **Templates:** Confirm both templates (data-infra-blueprint.md, rfp-scoring-matrix.md) are accessible to students via LMS or shared folder.
- **Reference materials:** If possible, have real vendor logos and screenshots ready (Snowflake UI, BigQuery console, dbt Cloud, Metabase dashboard). Concrete visuals help students who haven't used these tools.
- **Vendor pricing pages:** Bookmark current pricing pages for BigQuery, Snowflake, Fivetran, Airbyte, Metabase, Preset, Statsig, Eppo. Students will reference these during the RFP activity.
- Have water available. Consider starting with a brief physical movement exercise (stand up, stretch) before diving in.

---

## Slide Map (65 slides)

| Slide | Title |
|-------|-------|
| 1 | (Marp config) |
| 2 | Title: XFN, Vendor, IT & Data Infrastructure |
| 3–4 | Why Infrastructure Matters for Analytics Managers (1/2, 2/2) |
| 5–6 | The Cross-Functional Reality (1/2, 2/2) |
| 7–8 | What We'll Build This Module (1/2, 2/2) |
| 9–11 | Your Cross-Functional Universe (1/2, 2/2, cont.) |
| 12–13 | The XFN Failure Modes (1/2, 2/2) |
| 14–16 | What Each Team Needs From You (1/2, 2/2, cont.) |
| 17–18 | What You Need From Them (1/2, 2/2) |
| 19–20 | Building Bidirectional SLAs — Template (1/2, 2/2) |
| 21–22 | Building Bidirectional SLAs — Example (1/2, 2/2) |
| 23–24 | The Data Infrastructure Blueprint (1/2, 2/2) |
| 25–27 | Reading an Architecture Diagram (1/2, 2/2, 3/3) |
| 28–31 | Small Org Stack (1/2, 2/2, What to Skip, cont.) |
| 32–34 | Medium Org Stack (1/2, 2/2, cont.) |
| 35–37 | Large Org Stack (1/2, 2/2, cont.) |
| 38–39 | The Migration Trap (1/2, 2/2) |
| 40–41 | Build vs. Buy (Framework, Total Cost of Ownership) |
| 42–44 | The Hidden Costs of "Free" (Comparison 1/2, 2/2, Annual Total) |
| 45 | The RFP Process |
| 46–48 | RFP Scoring Dimensions (1/2, 2/3, 3/3) |
| 49–51 | Working with IT & Procurement (main, cont. 1/2, cont. 2/2) |
| 52–53 | The Procurement Timeline (Phases 1–4, Phases 5–8) |
| 54–56 | Privacy & Governance Basics (main, cont. 1/2, cont. 2/2) |
| 57–58 | Activity: Data Infrastructure One-Pager (main, cont.) |
| 59–60 | Activity: RFP Scoring Matrix (main, cont.) |
| 61 | Debrief |
| 62–63 | Your Infrastructure Toolkit (1/2, 2/2) |
| 64–65 | Next Steps (1/2, 2/2) |

---

## Timing — Reference Pacing (if taught as a live workshop)

_This module is provided as optional self-study material. The timing below is reference pacing for an instructor who chooses to run it as a live ~100-minute workshop._

| Min | Slide(s) | Activity |
|-----|----------|----------|
| 0-2 | 2 (Title) | Welcome, agenda, learning outcomes. Brief energy check. |
| 2-6 | 3–4 | Lecture: Why infrastructure matters. Set the management framing. |
| 6-10 | 5–8 | Cross-functional reality + what we'll build. Connect to Block A stakeholder maps. |
| 10-16 | 9–13 | XFN Universe + Failure Modes. Discussion-friendly — ask for real stories. |
| 16-22 | 14–22 | What teams need, what you need, SLA templates and examples. Move briskly through these. |
| 22-30 | 23–27 | **Anchor slides.** Data Infrastructure Blueprint + Reading an Architecture Diagram. Walk through each layer of the canonical flow. Take questions. This is the conceptual foundation for everything that follows. |
| 30-40 | 28–39 | Small / Medium / Large Stack + Migration Trap. Emphasize these are progressions, not choices. Ask students to identify where their case context sits. |
| 40-48 | 40–44 | Build vs. Buy + Hidden Costs of "Free". Lecture + discussion. Ask for real-world examples. The opportunity cost point resonates most — emphasize it. |
| 48-54 | 45–48 | RFP Process + Scoring Dimensions. Brief — the real learning happens in the activity. |
| 54-60 | 49–56 | Working with IT & Procurement + Privacy & Governance. Move briskly. These are awareness-level, not deep dives. |
| 60-85 | 57–58 | **Activity: Data Infra One-Pager (25 minutes).** Circulate actively. Common questions will be about pricing and tool selection — redirect to the framework, not specific recommendations. |
| 85-105 | 59–60 | **Activity: RFP Scoring Matrix (20 minutes).** Students pick one tool category and evaluate three vendors. Encourage use of real pricing from vendor websites. |
| 105-110 | 61–65 | **Debrief + Toolkit recap (5 minutes).** Pull 2-3 observations from the room. |

**Total: ~100 minutes** (with slight buffer for discussion overflow)

---

## Technical Calibration

Students will have varying levels of technical depth. Some will know what dbt is; others will not. Calibrate accordingly:

- **The blueprint slides (23–24) are your anchor.** Whenever the conversation drifts into tool-specific details ("but what about the difference between Snowflake's micro-partitioning and BigQuery's slot-based pricing?"), bring it back to the blueprint. "That's a great detail — but zoom out. Where does that fit in the flow? What decision does it inform?"
- **Don't go deep on any one tool.** This is a management course, not a data engineering course. Students need to know what categories exist, what questions to ask, and how to evaluate options. They don't need to configure anything.
- **Use the case contexts as leveling.** Small-context students should be thinking simple. If they're proposing Kubernetes and Kafka, gently redirect. Large-context students should be thinking about governance, procurement, and politics, not just tools.
- **Approximate pricing is fine.** Students will stress about getting exact numbers. Reassure them: order of magnitude is what matters. "$500/month" vs. "$50,000/month" is the decision that matters, not "$12,350 vs. $12,800."

---

## Vendor Neutrality

This is critical. Present frameworks, not recommendations.

- **When students ask "should I use X or Y?"** redirect to the scoring matrix. "That's exactly the right question — and the answer depends on your requirements. Let's use the framework. What are your must-haves? How do the two options score on those?"
- **Avoid expressing personal vendor preferences.** Even subtle signals ("I've had good experiences with X") will anchor students on that choice. Instead, share trade-offs: "X is easier to set up but more expensive at scale. Y has a steeper learning curve but lower TCO."
- **Open source is not automatically better or worse.** Some students will have a strong prior that open source = good. Others will assume commercial = better. Neither is universally true. The build-vs-buy framework applies.
- **Cloud provider lock-in** is a real concern but often overweighted by students. Acknowledge it, but note that for most small/medium orgs, the switching cost is lower than the cost of trying to stay provider-agnostic from day one.

---

## Key Teaching Points

### Emphasize
1. **The blueprint is a mental model, not a prescription.** Every org's implementation will differ. The layers are what matter.
2. **Build-vs-buy defaults:** Buy infrastructure, build business logic. This heuristic is right 80% of the time.
3. **Opportunity cost is the hidden killer.** Every hour maintaining open-source infra is an hour not spent on analysis. Make this vivid.
4. **IT is a partner, not a blocker.** The narrative of "IT won't let me do anything" is often a failure of relationship management, not a failure of IT.
5. **Procurement timelines are real.** Students who have never worked in procurement consistently underestimate how long it takes. The 2-6x multiplier is not exaggeration.

### Skip or Minimize
1. **Detailed tool comparisons.** Don't get drawn into "Snowflake vs. BigQuery vs. Databricks" debates. That's what the scoring matrix is for.
2. **Technical architecture details.** No need to explain medallion architecture, star schemas, or ELT vs. ETL in depth. Awareness level only.
3. **Specific GDPR articles.** Students need the concepts (lawful basis, minimization, erasure, consent). They don't need Article 6 subsection analysis.
4. **Data mesh philosophy.** Mention it as a pattern for large orgs. Don't get into Zhamak Dehghani's principles in detail — it's a rabbit hole.
5. **ML/AI infrastructure.** Large-context students may want to go deep here. Keep it at the "you need a platform for model training and deployment" level.

---

## Energy Management (if taught as a live workshop)

_The guidance below applies if this module is taught as a live session. For self-study, skip this section._

Energy will be low if taught after lunch. Strategies:

1. **Start with movement.** Before the first slide, have students stand up and do a 30-second stretch. It sounds silly. It works.
2. **Open with connection to morning.** "This morning you built growth plans. Now we're building the infrastructure those growth plans depend on." Link back to Block D to create continuity.
3. **The XFN slides are discussion-friendly.** Ask students to share their own cross-functional horror stories. "Who has been burned by a surprise schema change?" or "Who has waited months for IT to approve a tool?" These stories wake people up.
4. **Activities are the energy reset.** The two hands-on activities (minutes 60-105) are the core of this module. If lectures are running long, compress them to protect activity time. Students learn more by doing the scoring matrix than by hearing about it.
5. **Circulate during activities.** Don't sit down. Walk around, look over shoulders, ask questions. "What's your biggest gap in the current state?" "Which vendor is winning your scoring matrix so far?" This keeps energy up.

---

## Common Questions and How to Handle Them

### "What if my company can't afford anything?"
Every tool category has a free or open-source option. BigQuery has a generous free tier (1TB queries/month, 10GB storage). dbt Core is free. Metabase is open source. The real cost is your team's time to set it up and maintain it. Redirect to the build-vs-buy framework: "free" tools cost engineering time.

### "How do I convince IT to let me use cloud tools?"
Start by understanding their concerns — they're usually about security, data residency, and compliance, not about being obstructionist. Come to the conversation with answers: "This tool is SOC 2 Type II certified, stores data in EU-West-1, supports SAML SSO, and has audit logging. Here's the vendor's security whitepaper." Make their job easy.

### "What about open source? Isn't it always better?"
Open source is great for flexibility and avoiding vendor lock-in. But "free" software isn't free — it costs engineer time for setup, maintenance, upgrades, and troubleshooting. The question isn't "is it free?" but "what's the total cost of ownership including my team's time?" For small teams, managed services often win.

### "Should we use a data lakehouse instead of a warehouse?"
For most analytics use cases at small/medium scale, a warehouse (BigQuery, Snowflake) is simpler and sufficient. Lakehouses (Databricks) shine when you have large-scale ML workloads, unstructured data, or need to run Spark. Don't choose the lakehouse architecture because it's trendy — choose it because you have lakehouse problems.

### "How do I handle the 'shadow analytics' problem — teams building their own dashboards?"
This is a governance problem, not a technology problem. The solution is a combination of: (1) making your centralized tools easy to use, (2) publishing clear metric definitions, (3) having data owners who care, and (4) not being the analytics police — if teams want to self-serve, enable them with guardrails rather than gates.

### "What's the minimum viable governance for a small team?"
A naming convention document (how tables, columns, and metrics are named), a data dictionary (what each important field means), and a spreadsheet of data owners (who to ask when something breaks). That's it. Don't build a governance bureaucracy until you have the scale to justify it.

### "How do I evaluate vendors when I don't have technical expertise?"
Use the scoring matrix and involve your team. Your data engineer or analytics engineer should evaluate functionality and integration. IT should evaluate security. You evaluate support, cost, and strategic fit. The matrix is designed to combine multiple perspectives.

---

## Connection to the Rest of the Course

If students complete this module (as self-study or as an optional workshop), encourage them to:

1. **Connect to their roadmap** — Does the infrastructure plan support the projects on their Block C roadmap?
2. **Incorporate into QBR** — Infrastructure decisions can strengthen the QBR presentation with concrete technical grounding.
3. **Reflect on stakeholders** — Revisit the Block A stakeholder map. Did this module reveal stakeholders they missed (IT, procurement, security)?

---

## Connection to Portfolio

Both artifacts from this module are optional portfolio additions (not required):

- **Data Infrastructure Blueprint** — If included, should be refined and polished. Encourage students to connect it to their roadmap.
- **RFP Scoring Matrix** — If included, encourage students to do real vendor research to strengthen their evaluation.

Remind students that these are not theoretical exercises — they're practice for real decisions they'll face as analytics managers. Including them in the portfolio demonstrates additional depth.
