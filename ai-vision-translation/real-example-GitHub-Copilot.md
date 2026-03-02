# **QUICK FRAMEWORK SUMMARY**

• Translates executive AI ambition into shippable product features through 4 sequential filters 

• Moves from business metric → user problem → AI necessity check → 90-day scope 

• Prevents "pilots that impress execs but never ship" by forcing execution constraint upfront 

• Each filter acts as a filter: skip one, you build AI that doesn't move metrics, earn trust, or ship 

• Requires one 90-minute session with exec sponsor, product lead, engineering lead, domain expert 

• Output: one-page document defining what ships to real users in 90 days with kill switches


**COMPANY EXAMPLE**

**COMPANY:** GitHub (Microsoft subsidiary)

**INDUSTRY:** Developer Tools / Software Development

**INITIATIVE / PRODUCT:** GitHub Copilot

**YEAR(S):** 2021 (private beta) – 2022 (general availability)

**WHY THIS FITS:** 

• Started with broad AI ambition ("AI pair programmer"), executed through incremental scope 

• Shipped constrained v1 (autocomplete only) in aggressive timeline vs. building comprehensive coding assistant 

• Clear user friction (context-switching during coding), measurable outcome (completion acceptance rate), human override built-in


## **FILLING THE FRAMEWORK**

## **Filter 1: What the Business Actually Wants**

**Underlying Business Intention:** Revenue growth \+ Competitive pressure

**One-Sentence Business Objective:** • Increase GitHub user engagement and justify premium pricing tier by reducing developer coding friction by 30%+ within 12 months

**Business Metric at Risk (if nothing built):** 

• Developer migration to emerging AI-augmented IDEs (Replit, Cursor, Tabnine gaining traction in 2020–2021) 

• Stagnant conversion from free to paid GitHub tiers

**Number Attached:** 

• Target: 1M+ paid Copilot subscribers within 18 months of GA 

• Reality: Reached 1M paid seats June 2023 (\~12 months post-GA)


## **Filter 2: What User Problem That Solves**

**Current-State User Frustration:** 

• Developers interrupt flow state every 2–5 minutes to look up syntax, API documentation, or boilerplate patterns 

• Typing repetitive code structures (loops, error handling, CRUD operations) consumes 20–30% of coding time 

• Context-switching to Stack Overflow/docs breaks concentration, adds 30–90 seconds per lookup

**Before/After:** 

• **Before:** Developer stops coding, searches "python read csv pandas," scans Stack Overflow, copies snippet, adapts to context (avg 45 seconds) 

• **After:** Developer types function name, Copilot suggests complete implementation inline, developer accepts/edits (avg 3 seconds)

**User Outcome (No AI Jargon):** 

• Stay in flow state longer by eliminating documentation lookups for routine code patterns 

• Complete boilerplate tasks 40–50% faster (measured by time-to-first-commit in internal studies)


## **Filter 3: Where AI Genuinely Helps vs. Where It's Forced**

**AI Genuinely Required Because:** 

• Too many variables for deterministic rules: Suggestions must adapt to 50+ programming languages, frameworks, coding styles, and project context 

• Answer depends on context: Same function name needs different implementations based on surrounding code, imports, and repository patterns 

• Handles unstructured data at scale: Learns from billions of lines of public code to predict developer intent

**Where AI Overkill Was Avoided:** 

• Syntax highlighting, linting, error detection remained rule-based (deterministic, zero-tolerance-for-error) 

• Code execution/testing stayed in traditional compiler/interpreter (no AI in critical path) 

• Version control, diffs, merge conflicts handled by Git (proven non-AI solutions)

**Specific AI Capability with Handoff Points:** 

• LLM (Codex/GPT-3.5 variant) generates code suggestions based on context window 

• **Handoff to non-AI logic:** Developer always has edit/reject control; traditional IDE features (autocomplete, IntelliSense) run in parallel as fallback 

• **Confidence threshold:** Low-confidence suggestions suppressed (no guess presented as fact)

**Not "AI for coding"—Specific Application:** 

• Context-aware autocomplete for multi-line code blocks, function implementations, and comments-to-code translation 

• Explicitly NOT: full program generation, architecture decisions, security review, or testing (kept human-in-loop)


## **Filter 4: What Can Ship in 90 Days**

**Smallest Version That Proves Value:**

**One Specific Use Case:** 

• Inline code completion for Python and JavaScript in VSCode only (not multi-IDE, not all languages)

**Human-in-the-Loop Fallback:** 

• Developer must explicitly accept suggestion (Tab key) or reject (Esc/keep typing) 

• No auto-commit of AI-generated code; all suggestions are transparent grey text, never executed automatically 

• Traditional IDE autocomplete remains active as parallel safety net

**Observable Metrics:** 

• **Business outcome:** % of code accepted from Copilot suggestions (target: \>25%) 

• **Model behavior:** Suggestion latency (\<300ms), relevance score per suggestion, hallucination rate 

• **User trust:** Accept rate, time-to-edit after acceptance, disable rate

**Kill Switch for When Things Go Wrong:** 

• Per-file disable (// copilot: disable) 

• Per-session toggle (status bar icon) 

• Confidence threshold adjustable server-side without client update 

• Rollback to prior model version if acceptance rate drops \>15% week-over-week

**Clear Success Criteria:** 

• \>1,000 technical preview users actively coding daily with \>30% suggestion acceptance rate within 90 days 

• \<5% of users disabling Copilot permanently due to poor suggestions 

• P95 latency \<500ms for suggestion delivery

**What Shipped (Reality Check):** 

• Technical Preview: June 2021 (VSCode only, Python/JS/TS/Go focus) 

• Constraint: Invite-only, developers pre-screened for tolerance of imperfect suggestions 

• Scope: Code completion only—no chat interface, no explain-code, no debugging assistance (added 18+ months later)

**What Did NOT Ship in First 90 Days (Deferred):** 

• Multi-language support beyond core 4 

• IDE integrations beyond VSCode 

• Enterprise admin controls, audit logs, IP indemnification 

• "Copilot Chat" conversational interface (shipped Oct 2023\)


## **STRATEGIC REALITY CHECK**

**Where It Strongly Aligns:** 

• GitHub explicitly started with narrow scope (VSCode \+ 4 languages) vs. "AI coding assistant for everything"—matches Filter 4 incremental philosophy 

• Measurable user pain (context-switching) translated directly into AI capability (inline suggestions)—clean Filter 2 → 3 transition 

• Human-in-loop design (Tab to accept) and kill switches baked in from day 1—Filter 4 requirements met

**Where Alignment Is Partial:** 

• 90-day constraint inference: Technical Preview took \~4 months from Codex GPT-3 access (March 2021\) to June launch, but GitHub internal development likely started earlier 

• Business metric precision: No public evidence of "25% doc time reduction" target format—company communicated "10x developer productivity" aspiration (vaguer than framework prescribes)

**Key Risk/Assumption:** 

• Framework assumes 90 minutes produces one-page alignment doc; GitHub/OpenAI partnership likely involved months of negotiation on model access, data usage, IP liability—single-session facilitation may not apply to AI requiring external model dependencies 

• "Innovation theater" check: Copilot had revenue model clarity from start (paid tier)—framework's Filter 1 filter less critical when business model is obvious

