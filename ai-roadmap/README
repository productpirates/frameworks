# How to Use the 4-Filter AI Roadmap

**Author:** Carlos Oliveira — Product Pirates  
**Framework:** The 4-Filter AI Roadmap  
**Purpose:** Turn an AI wish list into a strategy that creates real alignment across executives, engineers, and users.

---

## What This Framework Is For

Most AI roadmaps fail not because the engineering is bad, but because they were built as feature lists — not as alignment tools. The 4-Filter AI Roadmap fixes this by separating your strategy into four distinct layers, each answering a different question for a different audience.

Use this framework when:
- You're starting an AI initiative and need to align stakeholders from day one
- Your existing AI roadmap is generating disagreement instead of momentum
- Your team is shipping AI features but can't tell whether they're working
- Executives and engineers are interpreting the roadmap differently

---

## The Four Filters at a Glance

| # | Filter | Core Question | Primary Audience |
|---|--------|--------------|-----------------|
| 01 | **Vision** | What does success look like in 12 months? | Executives, Board, CFO |
| 02 | **Outcomes** | How do we know the AI is working? | Product, Data, Exec |
| 03 | **Bets** | What must be true for this to succeed? | Engineering, ML, PM |
| 04 | **Delivery** | What ships and what do we learn? | Engineering, Design, Exec |

Each filter builds on the previous. Don't skip ahead — the order matters.

---

## Filter 01 — Vision

### What it does
Defines where you're going in terms that both a CFO and a customer can understand. It anchors all downstream decisions and prevents the roadmap from becoming a technology mandate in disguise.

### How to write it
Write exactly two sentences:
1. **Business outcome sentence** — what changes for the company in 12 months, expressed in measurable terms (revenue, retention, cost, speed).
2. **User experience sentence** — what becomes concretely different for the user.

> **Rule:** If the word "AI" appears in either sentence, rewrite it. AI is the *how*, not the *where*.

### Template
```
In 12 months, [business outcome in measurable terms].  
Users will be able to [specific experience change that wasn't possible before].
```

### Example
> *"Every new user reaches conversational fluency benchmarks 40% faster than our current onboarding path allows. Users practice real conversations on demand, without waiting for a human tutor."*

### Questions to pressure-test your Vision
- Could a CFO hold you accountable to this outcome?
- Would a user recognize the experience change you're describing?
- Is this still meaningful if you achieved it without AI?

---

## Filter 02 — Outcomes

### What it does
Defines the specific, measurable signals that prove your Vision is being achieved. This layer protects you from tracking the wrong things — namely, model metrics instead of behavior metrics.

### How to write it
For each major AI capability, define three things:

1. **Behavior metric** — a user action that changes as a result of the AI (not a model performance number).
2. **Success range** — a realistic floor and ceiling that respects the probabilistic nature of AI.
3. **Quality floor** — the threshold below which the feature is actively harmful, not just underperforming.

> **Rule:** Model accuracy, inference latency, and precision/recall are *engineering* metrics. They don't belong in your Outcomes layer. Ask: *is the AI changing what users do?*

### Template
```
We expect [AI capability] to [behavior change] for users who [qualifying condition].  
Success = [floor metric] improvement.  
Failure = more than [quality floor] of users reporting [negative signal].
```

### Example
> *"We expect AI conversation practice to increase weekly session frequency to 3+ per active user. Success = 15% higher month-3 retention among users who complete 10+ AI sessions. Failure = session abandonment rate exceeding 20% above baseline."*

### Questions to pressure-test your Outcomes
- Is every metric a user behavior, not a model property?
- Does the success range acknowledge that AI works on a spectrum?
- Have you defined what failure looks like, not just success?

---

## Filter 03 — Bets

### What it does
Documents the specific AI capabilities you're committing to — and, crucially, the assumptions that must hold for each one to deliver the outcome you promised. This is the most skipped layer and the most important one.

### How to write it
For every AI capability on the roadmap, write all three of the following. If you can't complete all three, the capability isn't ready to be committed.

1. **The Bet** — "We believe AI can do X."
2. **The Assumption** — "This only works if Y is true." (Name the two assumptions that would kill this bet if false.)
3. **The Validation** — "We will know the assumption holds by doing Z."

> **Rule:** A bet without assumptions is a wish. The goal of this layer is not to be right — it's to be explicit about what must be true, so engineers can challenge assumptions and the team can validate them early.

### Template
```
Bet: We believe [AI capability] can [specific outcome].  
Assumption 1: This only works if [condition A is true].  
Assumption 2: This only works if [condition B is true].  
Validation: We will know by [specific method or experiment] before [date/milestone].
```

### Example
> *"Bet: AI-generated conversation scenarios can replace 80% of what structured exercises currently do for vocabulary retention.*  
> *Assumption 1: Users tolerate occasional AI errors in low-stakes practice if correction feedback is immediate.*  
> *Assumption 2: Our content library is large enough for meaningful scenario variation.*  
> *Validation: Error tolerance survey at week 4, abandonment rate benchmarked against static exercise completion."*

### Questions to pressure-test your Bets
- Can you name the two assumptions that would kill each bet if false?
- Have you assigned someone to validate each assumption before the feature ships at scale?
- Would your engineers agree that these are the real risks?

---

## Filter 04 — Delivery

### What it does
Defines what ships in each 30-day cycle — and what the team will *learn* from it. The key distinction from a traditional delivery plan is that learning commitments are treated as equally important as shipping commitments.

### How to write it
For each 30-day window, define two things side by side:

1. **Shipping commitment** — what feature or increment goes to users and at what scope (e.g., 5% rollout, internal beta, full release).
2. **Learning commitment** — the specific question this cycle will answer. Phrase it as: *"By day 30, we will know ___."*

At the end of each cycle, add a **decision point**: expand rollout, pivot the approach, or rethink the assumption.

> **Rule:** Budget explicitly for model retraining and feedback loop work in every cycle. If it's not in the plan, it will disappear in sprint planning — and you'll end up with a stale model in production wondering why metrics plateaued.

### Template
```
Days 01–30:
  Ship: [Feature or increment] to [scope — % of users or cohort].
  Learn: By day 30, we will know [specific question].
  Decision point: If [condition], then [action].

Days 31–60:
  Ship: [Next increment], informed by cycle 1 findings.
  Learn: By day 60, we will know [next question].
  Decision point: If [condition], then [action].

Days 61–90:
  Ship: [Expanded or revised increment].
  Learn: By day 90, we will know [question that validates the original Bet].
  Decision point: If [condition], proceed to full rollout / return to Bets layer.
```

### Example
> *"Days 01–30: Ship beta AI conversation feature to 5% of users. By day 30, we will know whether session abandonment rate with AI conversations is within 15% of static exercise abandonment. Decision point: if abandonment is within range, expand to 20%; if not, rethink error-handling UX before scaling.*
>
> *Days 31–60: Expand to 20% of users with improved error feedback. By day 60, we will know whether AI session frequency is trending toward 3+ per week. Decision point: if yes, proceed to full rollout; if not, review Assumption 1 from Bets layer."*

### Questions to pressure-test your Delivery
- Does every 30-day cycle have both a shipping *and* a learning commitment?
- Have you budgeted time for model retraining in the 60–90 day window?
- Is there a decision point at the end of each cycle with a clear trigger?

---

## Putting It All Together

The four filters form a single coherent narrative. Here's how they connect:

```
VISION         →   sets the 12-month destination
    ↓
OUTCOMES       →   defines the behavioral proof that you're heading there
    ↓
BETS           →   names the capabilities and assumptions required to hit those outcomes
    ↓
DELIVERY       →   sequences what ships and what you learn in 30-day cycles
```

Every stakeholder should be able to find themselves in the document:
- **Executive** → reads Vision and the 30-day proof point in Delivery
- **Engineer** → reads Bets to understand the assumptions they're being asked to validate
- **Designer** → reads the UX constraints embedded in the Bets assumptions
- **PM** → owns the connection between all four layers and ensures they stay coherent as the product evolves

---

## Monday Morning Checklist

Run your current AI roadmap through these four questions before your next stakeholder meeting:

- [ ] Can you state your 12-month Vision without using the word "AI"?
- [ ] Are your success metrics user behaviors, not model properties?
- [ ] For each major AI capability, can you name the two assumptions that would kill it?
- [ ] Does your 30/60/90 plan include a "what we'll know" line alongside every shipping commitment?

If you can answer yes to all four, you have a roadmap that creates alignment. If not, start with question 3 — that's where the most uncomfortable and useful conversations live.

---

## Common Mistakes to Avoid

**Skipping Filter 03 (Bets).** This is the most common failure mode. Without documented assumptions, engineers receive an unrealistic roadmap and executives lose trust when features underdeliver. The Bets layer converts that dynamic into a validation conversation.

**Treating Delivery as a feature list.** A 30/60/90 plan full of features and dates with no learning commitments is just a wish list with deadlines. Every cycle needs a question it's answering.

**Using model metrics as Outcomes.** Precision, recall, and accuracy don't tell you whether the AI is changing user behavior. Swap every model metric for a behavior metric before sharing the roadmap with non-technical stakeholders.

**Writing Vision in tech language.** If your Vision mentions LLMs, model providers, or AI capabilities, it's a technology mandate — not a product vision. Rewrite it until it describes a world that's better for users and the business, with no mention of how you'll get there.

**Launching and moving on.** AI products degrade silently. Model drift, data distribution shifts, and changing user behavior will erode performance over time. Build retraining cycles into your Delivery layer from day one, or you'll be troubleshooting a stale model eight months after launch.

---

*Framework by Carlos Oliveira — Product Pirates*  
*Original post: "How to Escape AI Pilot Purgatory: The 90-Day Roadmap to Real Value"*
