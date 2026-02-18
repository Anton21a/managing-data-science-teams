---
marp: true
theme: ceu-analytics
paginate: true
header: "ECBS5256 – Managing Data Science Teams"
footer: "CEU Vienna | Day 1 – Block B"
---
<!-- Talk track: Block B — Hiring and Team Formation. This is the post-lunch block, so bring energy and start with the provocative cost-of-bad-hire framing. -->

<!-- _class: title -->

# Hiring & Team Formation

## Day 1 — Block B | 13:30–15:10

**LO: Produce a structured hiring packet that improves signal and fairness**

<!-- Talk track: Welcome back from lunch. This block is about the single highest-leverage activity you will do as a manager — hiring. A great hire compounds for years; a bad hire compounds damage for months. By the end of this block, you will have a complete hiring packet: job description, work sample exercise, scoring rubric, and interview loop design. Let's get into it. -->

---

# Why Hiring Is Your Highest-Leverage Activity

### The Compounding Effect of Great Hires

- A great **analyst** makes every PM smarter — they reframe questions, surface data no one asked for, and raise the quality of every decision in their orbit
- A great **data engineer** makes every analyst faster — reliable pipelines mean analysts spend time on insight, not cleaning CSVs at 2 AM
- A great **analytics manager** attracts other great people — talent compounds on itself

### The Negative Compounding of Bad Hires

- A bad analyst ships wrong numbers → stakeholders lose trust → the team loses its seat at the table
- A bad data engineer builds fragile pipelines → every analyst inherits tech debt → velocity collapses
- **Trust in analytics is uniquely fragile** — one bad number in a board deck and your credibility is gone for a year

> Hiring is the one activity where the returns — positive or negative — compound long after the decision is made.

<!-- Talk track: I want to start by making the case that hiring is not just important — it is the single highest-leverage thing you do as a manager. Think about compounding. A great analyst does not just produce good analyses. They make every product manager smarter because they reframe questions, surface data nobody thought to ask for, and raise the quality of every decision in their orbit. A great data engineer does not just build pipelines — they make every analyst on the team faster because the data is reliable and well-documented. And it works the other way too. A bad analyst ships a wrong number in a board deck, and suddenly the CFO does not trust anything from your team. Analytics is uniquely fragile here because our product is trust. Engineering ships code — if it breaks, you can see the error. Analytics ships numbers — if they are wrong, sometimes nobody notices for months, and by the time they do, the damage is done. -->

---

# The State of Analytics Hiring

### The Market Reality

- Data roles have grown **~650% in the past decade** — demand has exploded, but hiring practices have not kept up
- Most data job descriptions are **wish lists**, not role designs — "PhD required, 10 years of Python, must know Spark, Tableau, dbt, and also be a people person"
- The majority of analytics interviews are **unstructured** — a casual chat that predicts almost nothing
- Top candidates have **multiple offers** and they are evaluating you as much as you are evaluating them

### What the Best Companies Have Figured Out

- **Stripe** built a structured interview process for data roles with calibrated rubrics and take-home exercises reviewed blind
- **Airbnb** famously invested in making every candidate interaction reflect their values — even rejection emails
- These companies win talent not because they pay the most, but because their process **signals competence and respect**

<!-- Talk track: Let's talk about the hiring market for a moment. Data roles have exploded — something like 650 percent growth over the last decade depending on which report you read. But here is the problem: hiring practices have not kept up with the demand. Most data job descriptions are still wish lists — I have seen JDs that ask for a PhD, ten years of experience, fluency in five programming languages, and "startup mentality," all for a role paying 80K euros. Most analytics interviews are still unstructured — a hiring manager chats with the candidate for 45 minutes and then makes a gut call. Meanwhile, the best candidates have three or four offers. They are interviewing you as much as you are interviewing them. And the companies that figured this out — Stripe, Airbnb, and others — they win talent not by paying the most but by running a process that signals competence and respect. When a candidate goes through a well-structured interview, they think "these people know what they are doing — I want to work here." -->

---

# What We'll Build This Block

### Four Deliverables, Connected

```
  Role Design         Work Sample         Scoring Rubric       Interview Loop
  ───────────    →    ───────────    →    ──────────────   →   ──────────────
  90-day outcomes     Realistic task      Predefined           Who evaluates
  drive the JD        tests real work     dimensions + scale   what, and how
                                                               you decide
```

- The **Job Description** grounds everything in outcomes, not skills
- The **Work Sample** tests whether a candidate can actually do the job
- The **Rubric** ensures consistent, fair evaluation across interviewers
- The **Interview Loop** structures who evaluates what and how you reach a decision

### Looking Ahead to Day 2

Your hiring packet will be used in a **role-play exercise** where you will conduct a structured interview with a classmate acting as a candidate. You will experience both sides — interviewer and candidate — and stress-test your rubric against a real human being.

<!-- Talk track: Let me preview what we are building in the next 100 minutes. You will leave this block with four connected deliverables. First, a job description built around 90-day outcomes — not a skill shopping list. Second, a work sample exercise that simulates the actual job. Third, a scoring rubric with predefined dimensions and a four-point scale. Fourth, an interview loop design that specifies who evaluates what and how you make the final decision. These four things are not independent — they are a system. The outcomes in your JD determine what your work sample tests. Your rubric dimensions map to what the work sample reveals. Your interview loop assigns evaluators to rubric dimensions. And here is why this matters beyond today: on Day 2, you will use this packet in a role-play. You will actually conduct a structured interview with a classmate playing a candidate from a profile card. You will experience both sides. So build something you are willing to use for real. -->

---

# The Cost of a Bad Hire

- Average cost of a mis-hire: **1.5–2x annual salary** (SHRM, Bradford Smart)
- In analytics specifically, a wrong hire means:
  - **6 months of bad dashboards** that erode stakeholder trust
  - Broken credibility with the business — "analytics never delivers"
  - Team morale damage — good people leave when surrounded by poor performers
- The **"brilliant jerk"** problem: technical skill without collaboration destroys team culture faster than incompetence

> "The best thing a manager does is hire well. The second best thing is fire fast when they don't."
> — Ben Horowitz

<!-- Talk track: Let's start with stakes. Why does hiring matter so much in analytics? Because analytics is a trust business. If your first hire ships bad dashboards for six months, the VP of Product stops asking your team for help. They go hire a contractor or build their own spreadsheet. You lose your seat at the table. And the brilliant jerk — the person who is technically excellent but impossible to work with — they will drive away every collaborative person on your team. The cost is not just salary. It is organizational trust. -->

---

# Role Design Before Recruiting

**Don't start with a job description. Start with outcomes.**

### The Role Scorecard Approach

1. **What does this person need to accomplish in their first 90 days?**
2. Define 3–5 concrete outcomes, not a laundry list of skills
3. Work backward from outcomes to required capabilities

### Example — First Analytics Hire at a Seed-Stage Startup

| 90-Day Outcome | Capability Needed |
|:---|:---|
| Instrumented top-3 user flows with event tracking | SQL + analytics engineering |
| Delivered weekly KPI dashboard to founders | Visualization + communication |
| Scoped first A/B test for onboarding | Experimental design basics |

<!-- Talk track: Most hiring processes start wrong. Someone says "we need a data scientist" and the hiring manager opens a Google Doc and starts listing skills — Python, SQL, Tableau, machine learning, PhD preferred. That is a shopping list, not a role design. Instead, start with the question: what does this person need to accomplish in their first 90 days? Three to five concrete outcomes. Then work backward to what capabilities are actually required. You will be shocked at how different the resulting job description looks. -->

---

# The Job Description Anti-Pattern Gallery

### Pattern 1: The 25-Bullet Requirements List

> *"Required: Python, R, SQL, Spark, Hadoop, Tableau, Power BI, Looker, dbt, Airflow, Docker, Kubernetes, AWS, GCP, machine learning, deep learning, NLP, time series forecasting, A/B testing, causal inference, stakeholder management, project management, Agile, Scrum..."*

**What this signals to candidates:** "We do not know what this person will actually do, so we listed everything."

### Pattern 2: The Unicorn

> *"PhD in Statistics or Computer Science required. 10+ years of industry experience. Must thrive in a fast-paced startup environment." — Compensation: €75K–€85K*

**What this signals:** "We want a Staff-level person but will pay Junior-level comp." Senior candidates see this and close the tab.

### Pattern 3: The Copy-Paste

> A JD clearly written for a software engineer, with "data scientist" find-and-replaced in. Mentions "code reviews" and "shipping features" but nothing about analysis or stakeholders.

**What this signals:** "We do not understand what this role is. You will spend your first six months explaining your job to your own manager."

<!-- Talk track: Before you write your JD, let me show you the anti-patterns. I have collected these from real job postings — names removed to protect the guilty. Pattern one: the 25-bullet requirements list. You have seen these. Python, R, SQL, Spark, Hadoop, Tableau, Power BI, Looker, dbt, Airflow, Docker, Kubernetes — it goes on and on. What this tells a candidate is that you have no idea what this person will actually do, so you listed every tool you have ever heard of. Good candidates self-select out because they do not have all 25, even though no human does. Pattern two: the unicorn. PhD required, ten years of experience, startup mentality — for 80K. This tells senior candidates you either do not understand the market or you are hoping to find someone desperate. Pattern three: the copy-paste. This is a software engineering JD with "data scientist" swapped in. It mentions code reviews and sprint velocity but nothing about stakeholders, analysis, or decision support. The candidate reads this and thinks "they do not even know what this role is." Each of these anti-patterns actively repels the candidates you want most. -->

---

# What Level Do You Actually Need?

| Level | What They Do | Autonomy | Scope |
|:---|:---|:---|:---|
| **Junior** | Executes well-defined analyses | Needs clear specs | Single tasks |
| **Mid** | Scopes own work, communicates findings | Self-directed on known problems | Projects |
| **Senior** | Influences strategy, mentors others | Navigates ambiguity | Team-wide |
| **Staff/Principal** | Org-wide impact, shapes practice | Sets direction | Cross-team |

### Common Mistakes

- Hiring **senior** when you need **mid** — you pay for strategy but need execution
- Hiring **mid** when you need **senior** — they cannot navigate the ambiguity you are drowning in
- Writing "senior" in the title but paying mid-level comp

<!-- Talk track: Before you write the job description, get honest about what level you actually need. This is where a lot of managers get it wrong. A seed-stage startup does not need a Staff Data Scientist. They need someone who can write SQL, build dashboards, and communicate clearly — that is a strong mid-level hire. Conversely, if you are at a Series B and your entire analytics function is one person embedded with a product team, you probably need a senior who can navigate ambiguity and influence without authority. Leveling mistakes are expensive because the wrong-level hire will either be bored or overwhelmed, and both lead to attrition. -->

---

# The Leveling Conversation

### Having an Honest Discussion with Your Hiring Partner

The leveling conversation is the one you have with your recruiter, your HR business partner, or your finance lead before you open the role. It is often uncomfortable.

**The tension:**
- You need a Senior Analyst who can navigate ambiguity and influence PMs
- Finance approved headcount for a Mid-level role
- Your recruiter says "let's post it as Senior and see who applies" — this is a trap

### The Pressure to Level Down

- **"We can train them up"** — Sometimes true for Junior → Mid. Rarely true for Mid → Senior. The gap is judgment and influence, not skills.
- **"Let's hire two juniors instead of one senior"** — Two juniors without a senior to mentor them means two people making the same mistakes.
- **The hidden cost:** A mis-leveled hire who cannot do the job costs more than the salary difference between Mid and Senior.

### How to Have the Conversation

1. **Bring the outcomes list** — "Here is what this person needs to accomplish in 90 days. What level can do this?"
2. **Name the trade-offs explicitly** — "If we hire Mid, I need to budget 30% of my time for mentoring. Is that what we want?"
3. **Get alignment in writing** — A verbal "sure, hire a senior" turns into "why did you approve that comp?" without documentation

<!-- Talk track: This is the conversation nobody teaches you to have. You have done your role design, you know you need a Senior Analyst who can navigate ambiguity and influence product managers. You take this to your recruiter or your finance partner and they say "the budget is for a mid-level hire." Now what? Some managers cave and post a mid-level role hoping to find a unicorn. Others post "Senior" in the title but offer mid-level comp, which is the unicorn JD anti-pattern we just talked about. Here is how to handle it. Bring your outcomes list. Say "here is what this person needs to accomplish in their first 90 days — scope their own work, influence product roadmaps, present to the exec team. What level of hire can do this?" Make the trade-offs explicit. If you hire mid-level, you need to budget 30 percent of your own time for mentoring and air cover. Is that what the organization wants? Sometimes the answer is yes and that is fine — just make sure everyone agrees on what they are signing up for. And get the alignment in writing because memory is short when the comp review comes around. -->

---

# The Research on Structured Interviews

### Predictive Validity of Selection Methods

| Method | Correlation with Job Performance |
|:---|:---|
| Unstructured interviews | **~0.20** |
| Structured interviews | **~0.51** |
| Work samples | **~0.54** |
| Cognitive ability tests | **~0.51** |
| Reference checks | **~0.26** |
| Years of experience | **~0.18** |

<small>Source: Schmidt & Hunter (1998), updated meta-analyses</small>

<!-- Talk track: This is the most important table in the deck. These numbers come from decades of industrial-organizational psychology research, primarily Schmidt and Hunter's landmark 1998 meta-analysis and subsequent updates. An unstructured interview — the "let's just chat and see if they are smart" approach — predicts job performance at a 0.20 correlation. That is barely better than flipping a coin. A structured interview, where every candidate gets the same questions evaluated against a rubric, jumps to 0.51. Work samples — give them a realistic task and evaluate the output — hit 0.54. And notice that years of experience is at the very bottom at 0.18. Let that sink in. The thing most JDs filter on first — "5+ years required" — is the worst predictor of job performance in the entire table. -->

---

# What the Research Tells Us

**Key insight: Your gut feeling is mostly noise. Structure = fairness + signal.**

- Moving from unstructured to structured interviews is the **single biggest improvement** you can make to your hiring process — and it costs nothing
- Work samples outperform every other method because they **directly observe** what you care about: can this person do the job?
- Years of experience is the **worst predictor** on the list — yet it is the first filter on most job descriptions
- "I just know a good hire when I see one" is **noise dressed up as intuition**

### Why Structure Also Means Fairness

- Unstructured interviews amplify **affinity bias** — you hire people who remind you of yourself
- Structured interviews force you to evaluate **evidence against criteria**, not vibes
- This is not bureaucracy. This is how you find signal in a process riddled with bias.

<!-- Talk track: So what do we do with this? The takeaway is that moving from unstructured to structured interviews is the single biggest improvement you can make to your hiring process, and it is free. You do not need to buy software or hire a consultant. You need to write down the questions in advance, ask every candidate the same questions, and score the answers against predefined criteria. That is it. And here is the fairness angle — unstructured interviews amplify affinity bias. When you are just chatting, you gravitate toward people who remind you of yourself. Same school, same hobbies, same communication style. A structured process forces you to evaluate evidence against criteria instead of vibes. Some people hear "structure" and think "bureaucracy." I hear "structure" and think "the only way to find signal in a process that is drowning in noise." -->

---

# Designing Work Samples

### What Makes a Good Work Sample?

- **Reflects actual job tasks** — not LeetCode puzzles for analytics roles
- **Has clear evaluation criteria** — defined before candidates see the exercise
- **Respects candidate time** — 2–4 hours maximum, clearly communicated
- **Tests judgment, not just technique** — "What would you do next?" matters more than "Can you write a LEFT JOIN?"

### Analytics Work Sample Example

> *"Here is a messy dataset of user activity logs and a business question from the VP of Product: 'Should we invest in improving our onboarding flow?' Walk us through your approach, your analysis, and your recommendation."*

### What You Are Really Evaluating

How they **frame** the problem > How they **execute** the analysis > How they **communicate** the findings

<!-- Talk track: The work sample is the centerpiece of your hiring process. For analytics roles, this is not a coding test. It is a simulation of the actual job. You give candidates a realistic dataset — messy, with some known issues — and a business question. Then you evaluate three things in order of importance: first, how they frame the problem. Do they ask clarifying questions? Do they identify what is out of scope? Second, how they execute. Is the analysis sound? Do they handle missing data thoughtfully? Third, how they communicate. Can they explain their findings to a non-technical stakeholder? The framing question is the most diagnostic because it reveals whether someone can operate independently or needs everything spelled out for them. -->

---

# Work Sample Design Principles

### Balancing Realism and Respect for Candidate Time

- The work sample should feel like **a real day on the job**, not a homework assignment
- State the expected time commitment upfront: **"This should take 2–4 hours. We do not expect or want you to spend more."**
- Provide the dataset, the business question, and the context — do not make candidates guess what you want

### Making Work Samples Inclusive

- **Do not assume tool access** — "Use whatever tool you are comfortable with: Python, R, Excel, SQL, pen and paper"
- **Provide the rubric upfront** — candidates should know what dimensions they are being evaluated on. This is not a trick.
- **Allow flexible formats** — a slide deck, a written memo, a Jupyter notebook, or a recorded Loom video should all be acceptable
- **Set up for success, not gotchas** — include a data dictionary, note known data quality issues, provide a contact for clarifying questions

### When Candidates Go Above and Beyond

- Some candidates will spend 15 hours on a 4-hour exercise. **Do not reward this.** Score against the rubric dimensions, not effort or volume.
- If a candidate does the minimum well, that is a **signal of prioritization and judgment** — exactly what you want in an analyst.
- Going above and beyond is not a negative, but it should not substitute for quality on the core dimensions.

<!-- Talk track: Let me get specific about work sample design because the details matter a lot. First, respect candidate time. State the expected time commitment upfront and mean it. When someone spends 15 hours on a 4-hour exercise, do not reward that — it actually tells you something concerning about their ability to scope and prioritize. Second, make the exercise inclusive. Do not require a specific tool. Some of the best analysts I have worked with do their exploratory work in Excel before moving to Python. If you require Python, you are filtering for tool familiarity, not analytical ability. Third — and this one surprises people — share the rubric with the candidate. Tell them what dimensions you are evaluating. This is not a trick. You want to see their best work on the things that matter, not watch them guess what you care about. And allow flexible output formats. A clear two-page memo can be more impressive than a 40-slide deck. You are evaluating thinking, not production value. -->

---

# Why a Rubric?

### The Case for Predefined Dimensions

- Score on **predefined dimensions**, not overall impression
- Prevents: halo effect, anchoring, recency bias, "culture fit" as a catch-all
- Forces interviewers to articulate *what* they are evaluating

### What Happens Without a Rubric

- The debrief becomes a **storytelling contest** — whoever tells the most compelling anecdote wins
- Interviewers default to **overall impression**: "I liked them" or "Something felt off"
- **Halo effect** takes over — a candidate who is great at communication gets inflated scores on technical execution
- **"Culture fit"** becomes a catch-all for "I would want to get a beer with this person" — which is affinity bias in disguise

### What Happens With a Rubric

- Each interviewer independently rates **specific dimensions** with **behavioral anchors**
- The debrief becomes a **calibration conversation**: "I gave a 2 on Business Context because they never connected the analysis to a decision"
- Disagreements become **productive** — they reveal information, not just preferences

<!-- Talk track: Let me make the case for why a rubric is not optional. Without a rubric, your debrief meeting becomes a storytelling contest. The most articulate interviewer, or the most senior person in the room, tells a compelling anecdote about the candidate, and everyone else anchors to that story. You end up evaluating the interviewer's narrative skills, not the candidate's abilities. With a rubric, the conversation changes. Instead of "I liked them," it becomes "I gave a 2 on Business Context because when I asked how the analysis would inform a decision, they could not connect the dots." That is a specific, actionable observation. And when two interviewers disagree — one gave a 3 on communication, the other gave a 2 — that disagreement becomes productive. You ask "what did you see?" and you learn something. Without a rubric, disagreements are just opinion collisions. -->

---

# Dimensions for Analytics Roles

### Recommended Rubric Dimensions

| Dimension | What You Are Looking For |
|:---|:---|
| **Technical Execution** | Sound methodology, clean analysis, handles edge cases |
| **Communication Clarity** | Explains findings to non-technical audience |
| **Business Context Awareness** | Connects analysis to decisions and outcomes |
| **Intellectual Curiosity** | Asks good questions, explores beyond the obvious |

### Scale: 1–4 (No Fence-Sitting)

Use a 4-point scale. A 3-point scale lets everyone hide in the middle. A 5-point scale creates the illusion of precision you do not have. Force a meaningful call:

| Score | Meaning |
|:---|:---|
| **1** | Below the bar — significant concerns |
| **2** | Approaching the bar — some gaps |
| **3** | Meets the bar — would be effective in this role |
| **4** | Exceeds the bar — exceptional, raises the team |

<!-- Talk track: For analytics hires, I recommend four dimensions: technical execution, communication clarity, business context awareness, and intellectual curiosity. You can adapt these, but I would not go above five dimensions — more than that and your interviewers lose focus. Now, the scale. Use a four-point scale. Not three, not five. A three-point scale lets everyone pick the middle and avoid making a real evaluation. A five-point scale creates the illusion of precision that does not exist — nobody can reliably distinguish between a 3 and a 4 on a five-point scale in a 45-minute interview. Four points forces a meaningful distinction. A 1 means below the bar, significant concerns. A 2 means approaching but there are gaps. A 3 means they meet the bar and would be effective. A 4 means exceptional — this person would raise the level of the team. Most of your scores should be 2s and 3s. If you are giving a lot of 1s and 4s, either your calibration is off or your candidate pipeline needs work. -->

---

# Calibrating Scorers: The Problem

### Without Calibration, Scores Are Meaningless

Without calibration, interviewers anchor to different standards:
- Interviewer A thinks "3" means "could do the job"
- Interviewer B thinks "3" means "among the best I have seen"

### Real Example

Four interviewers evaluate the same candidate's work sample independently:

| Interviewer | Technical | Communication | Business Context | Curiosity |
|:---|:---|:---|:---|:---|
| Hiring Manager | 3 | 3 | 2 | 3 |
| Tech Peer | 2 | 2 | 2 | 2 |
| PM Partner | 3 | 4 | 3 | 3 |
| Skip-Level | 3 | 3 | 3 | 4 |

**Average score ranges from 2.0 to 3.25 depending on the interviewer.** Is this a hire or not? Without calibration, you cannot tell whether the Tech Peer is a tough grader or whether they saw something the others missed.

<!-- Talk track: Let me show you why calibration matters with a concrete example. Imagine four interviewers evaluate the same candidate. The hiring manager gives mostly 3s. The technical peer gives mostly 2s. The PM partner gives a 4 on communication and 3s elsewhere. The skip-level gives a 4 on curiosity. Now — is this a hire? You cannot answer that question without knowing what each person means by their scores. Is the tech peer a tough grader who gives 2s to everyone, or did they catch a genuine weakness? Is the PM partner's 4 on communication a high bar or a low one? This is the calibration problem. Without norming, your scores are just numbers without a shared reference point, and your debrief becomes an argument about what the numbers mean rather than what the candidate demonstrated. -->

---

# Calibrating Scorers: The Fix

### The Norming Session

**Before the interview loop begins:**
1. Score a **practice candidate** together (use a past work sample or a fabricated one)
2. Discuss every disagreement — "Why did you give a 2 on communication?"
3. Align on what each score means for each dimension
4. Document calibration notes for reference

### Biases Norming Prevents

- **Anchoring** to the first interviewer's opinion
- **Halo effect** — one strong dimension inflates all scores
- **Recency bias** — the last candidate always seems freshest
- **Similarity bias** — rating candidates higher when they remind you of yourself
- **Contrast effect** — a mediocre candidate looks great after a terrible one

### The Investment

- A norming session takes **20–30 minutes**
- It saves **hours of circular debrief arguments**
- It produces **better hires** because you are comparing candidates to a standard, not to each other

<!-- Talk track: The fix is a norming session, and it is simpler than you think. Before your interview loop begins, get all interviewers in a room for 20 to 30 minutes. Show them a work sample — either from a past candidate anonymized, or one you fabricated. Have everyone score it independently. Then discuss. You will be amazed at how different the scores are. One person gave a 4 on communication, another gave a 2, and they were looking at the same work. That is what you need to resolve before real candidates show up. Walk through each disagreement. The person who gave a 2 says "they did not tailor the message to the audience." The person who gave a 4 says "their analysis was clearly explained." Now you can align — communication clarity means tailoring to the audience, not just being clear. Document these calibration notes and share them. Twenty minutes of norming prevents hours of circular debrief arguments later. It is the highest-ROI meeting in your entire hiring process. -->

---

# The Interview Loop: Who Interviews for What

### Structured Assignment of Focus Areas

| Interviewer | Focus Area | Why This Person |
|:---|:---|:---|
| **Hiring Manager** | Role fit + team dynamics | Owns the decision |
| **Technical Peer** | Depth of craft | Can evaluate real skill |
| **Cross-Functional Partner** | Collaboration + communication | Will work with this person daily |
| **Skip-Level Manager** | Judgment + growth potential | Longer-term perspective |

### Why These Four

- **Four interviews** is the sweet spot — fewer than three and you lack signal diversity; more than five and you are wasting everyone's time and the candidate's patience
- Each interviewer has a **distinct focus** — no one evaluates "general impressions"
- The cross-functional partner is often the most diagnostic — a PM or engineer who will work with this analyst daily can evaluate collaboration in a way no hiring manager can

<!-- Talk track: The interview loop is the structure around who evaluates what. Four interviewers, each with a distinct focus. The hiring manager looks at role fit and team dynamics. A technical peer evaluates depth of craft — can this person actually do the work? A cross-functional partner, say a product manager or an engineer, tests collaboration and communication. And a skip-level manager assesses judgment and growth potential over a longer horizon. Four is the right number. Research from Google's People Operations team found that four interviews predict hiring outcomes almost as well as eight or more. Beyond four, you get diminishing returns and a worse candidate experience. The cross-functional partner is often the most revealing interview. A product manager who will work with this analyst daily can tell you things about collaboration and communication that no amount of technical evaluation will surface. -->

---

# The Interview Loop: Independent Scores and Decision-Making

### The Critical Rule: Independent Scores Before Discussion

1. Each interviewer submits scores **before** the debrief meeting
2. No peeking at others' scores
3. Debrief starts with a round-robin: each person shares their scores and top observations
4. Hiring manager makes the final call — this is **not** a consensus vote

### Why Independence Matters

- The first strong opinion in a debrief **anchors everyone else** — if the most senior person says "strong hire," watch how fast everyone agrees
- Independent scoring ensures you get **four genuine data points**, not one opinion amplified by social pressure
- **Disagreements are signal, not noise** — when one interviewer says "strong hire" and another says "no hire," dig into why. That gap often reveals the most important information about a candidate.

<!-- Talk track: The critical rule for the interview loop: everyone submits their scores independently before the debrief. No hallway conversations. No Slack messages saying "what did you think?" before scores are in. Why? Because the first strong opinion in a debrief anchors everyone else. If your VP walks into the room and says "I think she is great," watch how quickly every 2 becomes a 3. Independent scoring ensures you actually get four genuine data points instead of one opinion amplified by social pressure. And here is the nuance — the hiring manager makes the final call. This is not a democracy. Consensus-based hiring selects for "no one objected" rather than "someone was enthusiastic." But the hiring manager should take disagreements seriously. When one interviewer says strong hire and another says no hire, that gap is the most important information in the room. Do not average it away. Dig into it. -->

---

# The Debrief Meeting

### Running an Effective Debrief

1. **Before the meeting:** All scores submitted independently. The hiring manager reviews scores for major disagreements.
2. **Round-robin:** Each interviewer shares their scores and their **top observation** — not a 10-minute monologue, one key insight per dimension.
3. **Discuss disagreements first:** "You gave a 2 on Business Context and you gave a 4. Walk us through what you saw."
4. **Separate signal from preference:** "I did not like their presentation style" is preference. "They could not connect the analysis to a business decision" is signal.

### When Interviewers Disagree

- **Strong Hire vs. No Hire on the same dimension** — this is the most informative signal. Do not average it. Explore it. One interviewer may have probed deeper.
- **Consistent 3s across all dimensions** — this is often a "weak hire" signal. No one is excited, but no one objects. Be cautious.
- **One dimension drags the average down** — ask: is this dimension coachable? A 2 on Technical Execution is harder to fix than a 2 on Communication.

### The Hiring Manager's Call

- You have heard all the data. **You decide.** Do not hide behind consensus.
- A "strong hire" signal from the technical peer is worth more than lukewarm 3s from everyone else.
- When in doubt, do not hire. A false positive (bad hire) is far more expensive than a false negative (missed good candidate).

<!-- Talk track: Let me talk about the debrief meeting because this is where many structured processes fall apart. The debrief should take 30 to 45 minutes, not longer. Start with a round-robin — each interviewer shares their scores and one key insight per dimension. Not a 10-minute narrative. One key insight. Then go straight to the disagreements. If one person gave a 2 on Business Context and another gave a 4, that is the most interesting thing in the room. Have them both explain what they saw. Often one interviewer probed deeper on that dimension, or the candidate performed differently in different interviews — both are useful information. Watch out for the "consistent 3s" pattern. When every interviewer gives 3s across the board, it feels like a hire because the average is above the bar. But what it often means is that nobody is excited. Nobody saw something that made them think "this person would raise the level of our team." That is a weak hire signal, and weak hires are expensive. Finally, the hiring manager makes the call. Do not hide behind consensus. If you are not excited, pass. The cost of a false positive — hiring the wrong person — is much higher than the cost of a false negative. -->

---

# Candidate Experience: Your Employer Brand

### Your Employer Brand Is Built in Rejection Emails

- **Timeline:** < 1 week between stages. Silence is a decision — the decision to lose good candidates.
- **Communication:** Proactive updates even when there is no update. "We are still reviewing" beats silence.
- **Rejection:** Specific, kind, and fast.

### The Math

- You will interview ~20 candidates for each hire
- 19 of them will tell their network about the experience
- **19 negative stories vs. 1 hire** — the ratio matters

<!-- Talk track: Let me give you a number that changes how you think about hiring. For every person you hire, you reject about 19. Those 19 people will tell their friends, their colleagues, their social media followers about their experience with your company. If you ghosted them, or made them wait three weeks for a response, or gave them a take-home that took 20 hours — they will tell everyone. Your employer brand is not built in the offer letter. It is built in the rejection email. The data science and analytics community is small. Embarrassingly small. The analyst you reject today might be the hiring manager you need to impress in two years. Or they might be best friends with the perfect candidate you are trying to recruit next quarter. Every interaction matters. -->

---

# Candidate Experience: Non-Negotiables

### The Minimum Standard

- Acknowledge every application within 48 hours
- Provide a clear timeline at every stage
- Give feedback with rejections (even brief: "We went with a candidate with deeper SQL experience for this specific role")
- Never ghost a candidate who completed a work sample

### Going Beyond the Minimum

- **Send the work sample rubric in advance** — this is not a gotcha, it is a signal that you respect their time
- **Offer a 15-minute feedback call** to any candidate who completed a work sample — even if you do not hire them
- **Close the loop quickly** — the best candidates have other offers. If your process takes 6 weeks, you will lose them.
- **Be honest about the role** — if the team is struggling, if the data infrastructure is a mess, say so. Candidates who join with realistic expectations stay longer.

<!-- Talk track: Here are the non-negotiables. Acknowledge every application within 48 hours — this can be automated. Provide a clear timeline at every stage — "you will hear from us by Friday" and then actually follow up by Friday. Give feedback with rejections. It does not have to be a detailed performance review. "We went with a candidate who had deeper experience in experimental design" is enough. It is specific, it is respectful, and it gives the candidate something to work with. And the big one: never ghost a candidate who completed a work sample. That person invested hours of their life in your process. Ghosting them is how you build a reputation that kills your pipeline for years. If you want to go above the minimum, offer a 15-minute feedback call to anyone who did the work sample. Even candidates you reject will walk away thinking "that was the most professional interview process I have been through." That is your employer brand. -->

---

# Building Your Employer Brand in Analytics

### The Long Game

Your employer brand is not built in a quarter. It is built over years, through consistent signals that your team is a great place for data people.

### How to Be Known as a Great Place for Data People

- **Open-source contributions** — if your team builds internal tools that could help others, open-source them. Nothing says "we do serious data work" like a well-maintained GitHub repo.
- **Blog posts about your stack** — write about the problems you solved, the architecture decisions you made, the mistakes you learned from. Candidates read these.
- **Speaking at meetups and conferences** — encourage your team members to present at local data meetups, PyData, or industry conferences. Visibility attracts talent.
- **Treating rejected candidates well** — every person who goes through your process and thinks "that was fair and respectful" becomes an ambassador for your team.

### The Compounding Effect

- Year 1: Nobody knows who you are. You compete on comp and title.
- Year 2: A few blog posts, a meetup talk, a couple of good rejection experiences. Your inbound pipeline improves.
- Year 3: Candidates apply specifically because they heard your team is well-run. You are now selecting from a stronger pool.

**The best analytics teams spend less time recruiting because their brand does the work for them.**

<!-- Talk track: I want to talk about the long game of employer brand in analytics. This is not something you fix in a quarter. It compounds over time. There are a few things that signal to the market that your team is a great place to work. First, open-source contributions. If your team builds an internal library or tool that could help others, open-source it. Nothing attracts senior data talent like a well-maintained GitHub repo. Second, write about your work. Blog posts about your data stack, your architecture decisions, the mistakes you made and learned from — candidates read these before they apply. Third, encourage your team to speak at meetups. A 20-minute talk at a local PyData meetup costs almost nothing and puts your team on the radar of every data person in the city. And fourth — and this is the one most people miss — treat your rejected candidates well. Every person who goes through your process and thinks "that was the most professional interview I have ever done" becomes an ambassador for your team. They tell their friends. They post on LinkedIn. Over two or three years, this compounds. The best analytics teams I know spend less time recruiting because their brand does the recruiting for them. -->

---

<!-- _class: divider -->

# Activity: Build Your Hiring Packet

## 35 Minutes | Use the Templates

<!-- Talk track: Time to put this into practice. For the next 35 minutes, you will build a complete hiring packet for your first or next analytics hire within your chosen case context. You have four templates to complete: a job description built around 90-day outcomes, a work sample exercise, a scoring rubric, and an interview loop design. Use the templates provided. Work individually but feel free to ask questions. I will circulate. At the end, you will pair up for a role-play exercise using what you have built. -->

---

# Activity Brief: Build Your Hiring Packet

### Your Case Context

Use the company scenario you chose in Block A (small / medium / large)

### Deliverables (35 min)

1. **Job Description** — Role summary, 90-day outcomes, responsibilities, qualifications
2. **Work Sample Exercise** — Realistic task, dataset description, evaluation criteria
3. **Scoring Rubric** — Dimensions, 1–4 scale with behavioral anchors
4. **Interview Loop Design** — Stages, interviewers, focus areas, debrief protocol

### Tips

- Start with the 90-day outcomes — everything else follows
- Be honest about "required" vs. "preferred" qualifications
- Your work sample should take a candidate 2–4 hours, not 20
- Design the rubric so a stranger could use it and reach similar conclusions

<!-- Talk track: Here is the specific breakdown. Start with the job description template and fill in the 90-day outcomes first. That is your anchor. Then design a work sample that tests whether a candidate can actually accomplish those outcomes. Build your rubric next — make sure every dimension on the rubric maps to something you are testing in the work sample or interviews. Finally, design the interview loop. Who interviews, what they evaluate, and how you debrief. A tip: if you are stuck, start with the question "what would make me confident this person can succeed in their first 90 days?" and work backward from there. You have 35 minutes. Go. -->

---

# Role-Play Setup

### In 15 minutes, you will pair up

**Round 1 (10 min):** Person A plays the candidate. Person B runs a structured interview using their rubric.

**Round 2 (10 min):** Swap roles.

### How It Works

1. You will receive a **Candidate Profile Card** — play this person authentically, including their weaknesses
2. The interviewer uses their rubric and asks questions from their interview loop
3. After each round, the interviewer shares scores and explains their reasoning
4. The "candidate" gives feedback: "Here is what felt fair, here is what felt unclear"

### The Goal

Experience both sides of a structured interview. Find where your rubric works and where it breaks down.

<!-- Talk track: After the 35 minutes of building, we are going to do something uncomfortable and valuable. You are going to pair up and run actual structured interviews. One person plays the candidate using a profile card I will give you. The other person runs the interview using the rubric they just built. Then you swap. This is where the rubber meets the road. You will discover whether your rubric actually helps you evaluate someone or whether it falls apart when a real human being is sitting across from you. Play the candidate authentically — do not make it easy for the interviewer. If your profile says you are weak on communication, be weak on communication. The goal is to stress-test the rubric, not to practice being impressive. -->

---

# Candidate Profile Cards

### You Will Receive One of Four Profiles

| Profile | Archetype | Key Trait |
|:---|:---|:---|
| **Profile A** | The Strong Candidate | Solid all-around; might be slightly overqualified |
| **Profile B** | The Borderline | Good technical skills but communication gaps |
| **Profile C** | The Wrong Level | Impressive resume, but too senior/junior for the role |
| **Profile D** | The Culture Fit Trap | Likable and articulate but shallow technical depth |

Each card includes: background, strengths, weaknesses, a "tell" that the interviewer should catch, and suggested responses to common questions.

**Play the profile, not yourself.**

<!-- Talk track: I am going to hand out candidate profile cards. Each profile is a different archetype you will encounter in real hiring. Profile A is the strong candidate — solid all around, maybe a little overqualified. Profile B is the borderline — good technically but struggles to communicate findings. Profile C is the wrong-level candidate — their resume is impressive but they are either too senior or too junior for what you actually need. Profile D is the culture-fit trap — charming, articulate, says all the right things, but if you probe technically, the depth is not there. Each card has suggested responses and a tell — something the interviewer should catch if their rubric and questions are well-designed. Play the profile, not yourself. -->

---

# Debrief

### Reflection Questions

- **What signals were hardest to evaluate?**
  - Where did your rubric give you clear answers? Where did it fail?

- **Where did your rubric break down?**
  - Missing dimensions? Ambiguous score definitions? Too many dimensions?

- **What would you change?**
  - About your questions, your rubric, your scoring process?

- **What surprised you about being the candidate?**
  - What felt fair? What felt arbitrary?

### Key Takeaway

A rubric is a living document. Your first version will be wrong. The goal is to **iterate** after every interview loop.

<!-- Talk track: Let's debrief. I want to hear from both sides. Interviewers first: what was the hardest signal to evaluate? Where did your rubric give you a clear answer and where did it leave you guessing? Now candidates: what felt fair about the process? What felt arbitrary or unclear? This is the most important insight from the exercise — your first rubric will be wrong. Every rubric is wrong the first time. The goal is not perfection, it is iteration. After every real interview loop, you should update your rubric based on what you learned. Add a dimension you were missing. Sharpen a vague score definition. Remove a dimension that was not actually diagnostic. The rubric is a living document, not a form you fill out once and file away. -->

---

# Hiring Anti-Patterns (Part 1)

### Quick Hits — What Not to Do

- **"Culture fit" as a criterion** — This is how you hire clones of yourself. Replace with "culture add" or specific collaboration behaviors. Ask yourself: when someone says "not a culture fit," can they articulate what specific behavior concerned them? If they cannot, it is bias.

- **The 20-hour take-home** — Disrespects candidate time, biases toward people with free time (read: people without caregiving responsibilities), and the best candidates will drop out. A principal engineer at a FAANG company is not going to spend her weekend on your take-home. Two to four hours, clearly scoped.

- **The "rockstar/ninja" JD** — Signals immaturity. Senior candidates run from these because they have seen what "rockstar culture" actually means: no process, no work-life balance, and a founder who thinks management is beneath them.

<!-- Talk track: Before we close, let me walk through the hiring anti-patterns I see most often in analytics. First, culture fit as a criterion. This almost always means "this person is like me" and it is how you build a homogeneous team with blind spots. Ask the interviewer who raises "culture fit" concerns to be specific. What behavior did they observe? If they cannot answer, it is bias, not signal. Replace it with culture add or specific collaboration behaviors you can actually evaluate. Second, the 20-hour take-home. The best candidates have options. They will not spend a weekend on your exercise. And this one has a hidden equity problem — it biases toward people who have free weekends, which means you are selecting against parents, caregivers, and anyone with a life outside work. Two to four hours, clearly scoped. Third, the rockstar or ninja job description. I know it seems fun and edgy, but every experienced person reading it assumes your org has no process and your management is absent. -->

---

# Hiring Anti-Patterns (Part 2)

### More Quick Hits

- **Ghosting candidates** — Especially after a work sample. This is how you build a reputation that kills your pipeline. The analytics community is small — the person you ghost today is the hiring manager you will need to impress in two years.

- **Consensus-based decisions** — "Everyone needs to agree" selects for inoffensive mediocrity. The hiring manager decides. Consensus is how you end up with someone nobody objected to but nobody was excited about. That is not a hire — that is a compromise.

- **Hiring for potential without structure** — "I see myself in them" is bias, not signal. Potential is real, but evaluating it requires structured criteria: learning velocity, ability to operate in ambiguity, trajectory of increasing scope. If you cannot articulate what "potential" means in measurable terms, you are just pattern-matching to your own background.

### The Meta Anti-Pattern

All of these share a common root: **substituting gut feeling for structured evaluation.** The research is clear — structure beats intuition. Every time.

<!-- Talk track: Three more anti-patterns. Ghosting candidates after a work sample is reputation destruction. The analytics community is embarrassingly small. I have seen hiring managers ghost candidates who later became VPs at companies they desperately wanted to partner with. It is a small world and your reputation travels. Consensus-based decisions — if everyone has to agree, you will hire the person nobody objects to, which is not the same as the person someone is excited about. The hiring manager makes the call. Period. And finally, hiring for potential without structure. Potential is a real thing, but "I see myself in them" is not how you evaluate it. If you want to hire for potential, define what that means: learning velocity, ability to navigate ambiguity, trajectory of increasing scope. Put it in the rubric. Make it specific. Otherwise "potential" is just a code word for "they went to the same school I did" or "they remind me of me at that age." Notice the common thread in all of these: substituting gut feeling for structured evaluation. That is the meta anti-pattern. Structure beats intuition. The research is unambiguous. -->

---

# Key Takeaways

1. **Start with outcomes**, not skills — the 90-day scorecard drives everything
2. **Structure beats intuition** — 0.51 vs. 0.20, every time
3. **Work samples are your best tool** — test real judgment, not trivia
4. **Calibrate before you interview** — 20 minutes of norming prevents hours of debate
5. **Candidate experience is employer brand** — 19 rejections for every 1 hire

### Deliverable Reminder

**Hiring Packet DRAFT due Thursday (23:59 Vienna)** for instructor feedback.
It will be used in Day 2 role-plays.

Components: JD + Work Sample + Rubric + Interview Loop

<!-- Talk track: Let me leave you with the five things I want you to remember from this block. First, start with outcomes, not skills. The 90-day scorecard is your anchor. Second, structure beats intuition — the research is unambiguous. Third, work samples are your best tool for analytics hiring because they test real judgment. Fourth, calibrate your scorers before you start interviewing. And fifth, candidate experience is employer brand — treat every candidate like they might be your next hire's best friend, because in data science, they probably are. Your hiring packet draft is due Thursday by midnight Vienna time. I will give written feedback, and you will use the polished version in Day 2 role-plays. -->

---

<!-- _class: divider -->

# Up Next: Block C

## Roadmaps, Bets, and Alignment
### 15:30–17:10

<!-- Talk track: We will take a 20-minute break. When you come back, Block C is about roadmaps, bets, and alignment — how you decide what your analytics team works on, how you communicate priorities to leadership, and how you say no to the 80 percent of requests that do not make the cut. See you at 15:30. -->
