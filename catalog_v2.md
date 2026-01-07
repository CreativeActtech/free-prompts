# Prompt Catalog V2

### Overview

The Prompt Catalog v2.0 is a comprehensive collection of 250 specialized prompts designed to facilitate high-precision results across diverse professional and personal categories. Each prompt utilizes expert personas and structured frameworks to transform raw information into actionable insights, covering everything from technical data engineering to strategic business planning and personal wellness.

---

```markdown
## Prompt 1: Blog Post Expansion (Architect Mode)

**Role:** Senior Content Strategist & Editor

**Instruction:** Expand a skeleton outline into a high-authority blog post adhering to the provided `<tone>`.

**Process:**
1. **Audience Analysis:** Briefly define pain points of `<target_audience>`
2. **Drafting:** Expand `<outline>` section by section; ensure each has a clear "takeaway"
3. **Review:** Verify consistent tone throughout

**Data:**
- `<outline>[OUTLINE]</outline>`
- `<target_audience>[AUDIENCE]</target_audience>`
```

```markdown
## Prompt 2: Style Transformer (Semantic Preservation)

**Role:** Linguistic Specialist

**Instruction:** Rewrite `<original_text>` to strictly match `<target_style>` while preserving 100% semantic meaning.

**Constraint:** Do not add new facts or remove key information

**Data:**
- `<original_text>[TEXT]</original_text>`
- `<target_style>[STYLE]</target_style>`
```

```markdown
## Prompt 3: SEO Metadata Engineer

**Role:** Technical SEO Specialist

**Instruction:** Generate Title Tag and Meta Description optimized for high CTR and `<primary_keyword>`.

**Constraints:**
- Title: Max 60 characters; place `<keyword>` near front
- Meta Description: Max 160 characters; include CTA

**Data:**
- `<content_summary>[CONTENT]</content_summary>`
- `<primary_keyword>[KEYWORD]</primary_keyword>`
```

```markdown
## Prompt 4: Headline A/B Tester (Psychological Triggers)

**Role:** Direct Response Copywriter

**Instruction:** Generate 5 high-converting headlines for `<topic>` using angle `<angle>`.

**Reasoning:** Each headline must use a different psychological hook (Urgency, Curiosity, Social Proof, Specificity, Negative Bias)

**Data:**
- `<topic>[TOPIC]</topic>`
- `<angle>[ANGLE]</angle>`
```

```markdown
## Prompt 5: Intro Hook Generator

**Role:** Investigative Journalist

**Instruction:** Write three distinct opening hooks for an article on `<subject>`.

**Variations:**
1. **The Statistic:** Start with shocking hypothetical data
2. **The Story:** Start with a micro-narrative
3. **The Contrarian:** Challenge a common belief held by `<audience>`

**Data:**
- `<subject>[SUBJECT]</subject>`
- `<audience>[AUDIENCE]</audience>`
```

```markdown
## Prompt 6: Active Voice Refactor

**Role:** Book Editor

**Instruction:** Rewrite `<text>` to eliminate passive voice.

**Rule:** Replace "to be" verbs with energetic transitive verbs; infer missing subjects using "we/they"

**Data:**
- `<text>[TEXT]</text>`
```

```markdown
## Prompt 7: Concise Paraphraser (Density Optimization)

**Role:** Technical Communicator

**Instruction:** Rewrite `<source>` text to be 50% shorter.

**Success Criteria:**
- Retain 100% of factual data points
- Remove filler words, adverbs, and redundant transitions

**Data:**
- `<source>[SOURCE]</source>`
```

```markdown
## Prompt 8: Newsletter Subject Line Optimizer

**Role:** Email Marketing Specialist

**Instruction:** Suggest 10 subject lines for a newsletter about `<update>`.

**Strategy:**
- Lines 1-3: Direct/Benefit-driven
- Lines 4-6: Curiosity/Open-loop
- Lines 7-10: Urgency/Scarcity

**Data:**
- `<update>[UPDATE]</update>`
```

```markdown
## Prompt 9: Fact-Check Protocol

**Role:** Lead Fact Checker

**Instruction:** Analyze `<text>` and isolate primary claims.

**Output Format:** Markdown table with columns:
- Claim Made
- Data Needed for Verification
- Potential Bias Source

**Data:**
- `<text>[CLAIMS]</text>`
```

```markdown
## Prompt 10: CTA (Call-to-Action) Architect

**Role:** CRO (Conversion Rate Optimization) Expert

**Instruction:** Create 3 distinct CTAs for `<offer>`.

**Tones:**
1. **Standard:** Clear and direct (e.g., "Sign Up")
2. **Benefit:** Focus on result (e.g., "Get Higher Rankings")
3. **Friction-Reduction:** Address anxiety (e.g., "No Credit Card Required")

**Data:**
- `<offer>[OFFER]</offer>`
- `<tone>[TONE]</tone>`
```

```markdown
## Prompt 11: Meeting Minutes Executive Summary

**Role:** Chief of Staff

**Instruction:** Synthesize raw `<notes>` into structured summary.

**Output Sections:**
1. **Executive Abstract:** 2-sentence summary of purpose and outcome
2. **Key Decisions:** Bullet points of agreed items
3. **Action Plan:** Table format `[Task] | [Owner] | [Deadline]`

**Data:**
- `<notes>[NOTES]</notes>`
```

```markdown
## Prompt 12: Professional Email Drafter

**Role:** Executive Assistant

**Instruction:** Draft professional email to `<recipient>` based on `<context>`.

**Goal:** Achieve `<outcome>` with minimal back-and-forth

**Data:**
- `<context>[CONTEXT]</context>`
- `<outcome>[OUTCOME]</outcome>`
- `<recipient>[RECIPIENT]</recipient>`
```

```markdown
## Prompt 13: Benefit-Centric Product Description

**Role:** Product Marketing Manager

**Instruction:** Write product description for `<name>`.

**Constraint:** For every `<feature>`, explain "What this means for the user" (The Benefit)

**Data:**
- `<name>[NAME]</name>`
- `<features>[FEATURES]</features>`
```

```markdown
## Prompt 14: Policy-Compliant Support Response

**Role:** Senior Customer Support Agent

**Instruction:** Draft response to customer `<inquiry>`.

**Guardrails:** Strictly adhere to `<policy>`; emphasize empathy without promising beyond policy limits

**Data:**
- `<inquiry>[INQUIRY]</inquiry>`
- `<policy>[POLICY]</policy>`
```

```markdown
## Prompt 15: Strategic SWOT Analysis

**Role:** Management Consultant

**Instruction:** Perform detailed SWOT analysis for `<idea>`.

**Thinking Process:**
- Identify Internal factors (Strengths/Weaknesses)
- Identify External factors (Opportunities/Threats)
- Synthesis: Suggest one strategy to leverage Strength to maximize Opportunity

**Data:**
- `<idea>[IDEA]</idea>`
```

```markdown
## Prompt 16: OKR Architect (Objectives & Key Results)

**Role:** Agile Coach

**Instruction:** Draft 3 Objectives and 3 Key Results (per objective) for `<goal>`.

**Constraint:** All Key Results must be numerically measurable (%, $, count) and time-bound by `<timeline>`

**Data:**
- `<goal>[GOAL]</goal>`
- `<timeline>[TIMELINE]</timeline>`
```

```markdown
## Prompt 17: Project Brief Generator

**Role:** Project Manager (PMP)

**Instruction:** Convert raw `<requirements>` into structured Project Brief.

**Required Sections:**
1. **Project Goal:** (1 sentence)
2. **Scope In/Out:** What is included vs excluded
3. **Stakeholder Analysis:** Roles of listed `<stakeholders>`

**Data:**
- `<requirements>[REQUIREMENTS]</requirements>`
- `<stakeholders>[STAKEHOLDERS]</stakeholders>`
```

```markdown
## Prompt 18: Executive Report Condenser

**Role:** Board Advisor

**Instruction:** Summarize `<report>` into 1-page "BLUF" document for leadership.

**Focus:** Highlight financial impact, risks, and required decisions; ignore operational minutiae

**Data:**
- `<report>[REPORT]</report>`
```

```markdown
## Prompt 19: Risk Assessment Matrix

**Role:** Risk Analyst

**Instruction:** Analyze `<initiative>` and list 5 potential risks.

**Output Format:** Table with columns:
- Risk Description
- Likelihood (Low/Med/High)
- Impact (Low/Med/High)
- Mitigation Strategy

**Data:**
- `<initiative>[INITIATIVE]</initiative>`
```

```markdown
## Prompt 20: Structured Meeting Agenda

**Role:** Facilitator

**Instruction:** Design 30-minute agenda for `<discussion_points>`.

**Structure:**
- 0-5 min: Intro & Context
- (Allocate specific time blocks per point)
- 25-30 min: Review Action Items

**Data:**
- `<discussion_points>[POINTS]</discussion_points>`
```

```markdown
## Prompt 21: UVP (Unique Value Proposition) Designer

**Role:** Brand Strategist

**Instruction:** Differentiate `<product>` from `<competitors>`.

**Output:**
1. **The "Only" Statement:** "We are the only [Category] that [Benefit] for [Customer]."
2. **Feature Gap:** One specific thing competitors cannot do

**Data:**
- `<product>[PRODUCT]</product>`
- `<competitors>[COMPETITORS]</competitors>`
```

```markdown
## Prompt 22: ICP (Ideal Customer Profile) Builder

**Role:** Head of Growth

**Instruction:** Build rich ICP for `<service>` in `<market>`.

**Details Required:**
- **Demographics:** Role, Company Size, Revenue
- **Psychographics:** Fears, Aspirations, "Job to be Done"
- **Buying Trigger:** Specific event causing solution search

**Data:**
- `<service>[SERVICE]</service>`
- `<market>[MARKET]</market>`
```

```markdown
## Prompt 23: AIDA Framework Ad Copy

**Role:** Advertising Copywriter

**Instruction:** Write ad for `<product>` using AIDA formula.

**Structure:**
- **Attention:** Hook with `<pain_point>`
- **Interest:** Agitate problem with facts
- **Desire:** Present solution benefits
- **Action:** Direct next-step instruction

**Data:**
- `<product>[PRODUCT]</product>`
- `<pain_point>[PAIN_POINT]</pain_point>`
```

```markdown
## Prompt 24: Tagline Brainstorming Session

**Role:** Creative Director

**Instruction:** Generate 15 taglines for `<brand_name>` embodying `<values>`.

**Categories:**
- 5 Literal (Descriptive)
- 5 Abstract (Emotive)
- 5 Short (3 words or less)

**Data:**
- `<brand_name>[NAME]</brand_name>`
- `<values>[VALUES]</values>`
```

```markdown
## Prompt 25: Cold Outreach Sequence (LinkedIn)

**Role:** SDR (Sales Development Rep) Coach

**Instruction:** Draft LinkedIn connection message for `<prospect_role>` at company focused on `<company_focus>`.

**Strategy:**
1. **The Hook:** Reference specific company focus
2. **The Bridge:** Connect focus to `<my_value>`
3. **The Ask:** Low friction (e.g., "Open to 5-min chat?")

**Data:**
- `<prospect_role>[ROLE]</prospect_role>`
- `<company_focus>[FOCUS]</company_focus>`
- `<my_value>[VALUE]</my_value>`
```

```markdown
## Prompt 26: Content Pillar Strategist

**Role:** Social Media Manager

**Instruction:** Define 4 "Content Pillars" for brand in `<niche>` aiming to achieve `<goals>`.

**For each pillar:**
- Name the Pillar
- List 3 example post ideas
- Explain how it serves the goal

**Data:**
- `<niche>[NICHE]</niche>`
- `<goals>[GOALS]</goals>`
```

```markdown
## Prompt 27: Competitor Gap Analyst

**Role:** Market Researcher

**Instruction:** Compare `<our_specs>` vs `<their_specs>`.

**Output:** Identify 3 "Gaps" where we are superior; write legally defensible marketing claims for each

**Data:**
- `<our_specs>[OURS]</our_specs>`
- `<their_specs>[THEIRS]</their_specs>`
```

```markdown
## Prompt 28: Lead Magnet Generator

**Role:** Inbound Marketing Expert

**Instruction:** Suggest 5 high-value lead magnets for `<target_audience>` in `<industry>`.

**Criteria:** Each must solve a specific, immediate problem (calculator > whitepaper)

**Data:**
- `<industry>[INDUSTRY]</industry>`
- `<target_audience>[TARGET]</target_audience>`
```

```markdown
## Prompt 29: Testimonial Request Script

**Role:** Client Success Manager

**Instruction:** Draft polite email to `<client_name>`.

**Method:** Remind them of specific result `<project_success>`, then request 2-sentence quote; provide draft testimonial for editing

**Data:**
- `<client_name>[NAME]</client_name>`
- `<project_success>[SUCCESS]</project_success>`
```

```markdown
## Prompt 30: Landing Page Hero Designer

**Role:** UX Copywriter

**Instruction:** Write "Above the Fold" copy for `<product>`.

**Components:**
- **H1 (Headline):** Must mention `<main_benefit>`
- **H2 (Subhead):** Explain how it works or who it's for
- **Button Text:** High-agency text (avoid "Submit")

**Data:**
- `<product>[PRODUCT]</product>`
- `<main_benefit>[BENEFIT]</main_benefit>`
```

```markdown
## Prompt 31: Code Logic Explainer

**Role:** Senior Developer Mentor

**Instruction:** Explain functionality of `<code_block>`.

**Analysis Steps:**
1. **Identify Language:** Confirm `<language>`
2. **Flow Analysis:** Walk through execution path step-by-step
3. **Summary:** Explain intent in plain English

**Data:**
- `<code_block>[CODE]</code_block>`
- `<language>[LANGUAGE]</language>`
```

```markdown
## Prompt 32: SQL Query Architect

**Role:** Database Administrator (DBA)

**Instruction:** Construct SQL query to achieve `<goal>` based on `<schema>`.

**Reasoning:**
- Identify necessary tables and keys
- Determine Join types (Inner vs Left)
- Write query using best practices (aliasing, capitalization)

**Data:**
- `<schema>[SCHEMA]</schema>`
- `<goal>[GOAL]</goal>`
```

```markdown
## Prompt 33: Unstructured Text to JSON Converter

**Role:** Data Engineer

**Instruction:** Parse `<text>` and extract data into valid JSON object.

**Schema Definition:** JSON must strictly contain keys defined in `<fields>`; handle missing data with null

**Data:**
- `<fields>[FIELDS]</fields>`
- `<text>[TEXT]</text>`
```

```markdown
## Prompt 34: Debugging & Remediation

**Role:** QA Automation Engineer

**Instruction:** Analyze `<code_block>` for specific `<error>`.

**Output:**
1. **Diagnosis:** Why it's failing
2. **The Fix:** Provide corrected code block
3. **Prevention:** How to catch earlier next time

**Data:**
- `<code_block>[CODE]</code_block>`
- `<error>[ERROR]</error>`
```

```markdown
## Prompt 35: Regex Pattern Generator

**Role:** DevOps Engineer

**Instruction:** Create Regular Expression to match `<requirement>`.

**Verification:**
- Explain pattern token breakdown
- Prove it matches `<examples>`

**Data:**
- `<requirement>[REQUIREMENT]</requirement>`
- `<examples>[EXAMPLES]</examples>`
```

```markdown
## Prompt 36: API Documentation Specialist

**Role:** Technical Writer

**Instruction:** Document `<endpoint>` based on logic `<logic>`.

**Format:** OpenAPI/Swagger style description
- Method/Path
- Parameters (Query/Body)
- Response Codes (200, 400, 500)

**Data:**
- `<endpoint>[ENDPOINT]</endpoint>`
- `<logic>[LOGIC]</logic>`
```

```markdown
## Prompt 37: Bash Automation Script

**Role:** SysAdmin

**Instruction:** Write Bash script to automate `<task>`.

**Constraints:**
- Target Environment: `<env>` (e.g., Ubuntu, macOS)
- Include error handling (`set -e`)
- Comment every major step

**Data:**
- `<task>[TASK]</task>`
- `<env>[ENV]</env>`
```

```markdown
## Prompt 38: Unit Test Generator

**Role:** Software Engineer in Test

**Instruction:** Write unit test suite for `<function>` using `<framework>`.

**Coverage:**
- Happy Path (Expected input)
- Edge Cases (Nulls, empty strings, limits)
- Error Handling (Expected exceptions)

**Data:**
- `<function>[FUNCTION]</function>`
- `<framework>[FRAMEWORK]</framework>`
```

```markdown
## Prompt 39: Markdown Formatter

**Role:** Technical Editor

**Instruction:** Convert `<raw_text>` into clean, semantic Markdown.

**Rules:**
- Use H1/H2/H3 for hierarchy
- Use Bullet points for lists
- Use Code blocks ``` for technical strings

**Data:**
- `<raw_text>[TEXT]</raw_text>`
```

```markdown
## Prompt 40: Conventional Commits Generator

**Role:** Lead Developer

**Instruction:** Analyze `<changes>` and generate Git commit message following Conventional Commits standards.

**Format:** `type(scope): subject` followed by body explaining "Why" (not just "What")

**Data:**
- `<changes>[CHANGES]</changes>`
```

```markdown
## Prompt 41: Database Schema Designer

**Role:** Data Architect

**Instruction:** Design relational schema for `<app_concept>`.

**Output:** List of Tables. For each table, list:
- Primary Key
- Foreign Keys (and relationships)
- Core Columns

**Data:**
- `<app_concept>[CONCEPT]</app_concept>`
```

```markdown
## Prompt 42: Code Refactoring (Tech Debt)

**Role:** Principal Engineer

**Instruction:** Review `<code_block>` for "Code Smells."

**Analysis:**
1. Identify anti-patterns (tightly coupled logic, magic numbers)
2. Provide refactored version adhering to CLEAN code principles

**Data:**
- `<code_block>[CODE]</code_block>`
```

```markdown
## Prompt 43: CLI Command Retriever

**Role:** Linux Guru

**Instruction:** Provide exact terminal command to perform `<action>` on OS `<os>`.

**Detail:** If command is dangerous (e.g., `rm`, `dd`), add warning and explain flags

**Data:**
- `<action>[ACTION]</action>`
- `<os>[OS]</os>`
```

```markdown
## Prompt 44: Log Extraction Logic

**Role:** DevOps Engineer

**Instruction:** Write regex or script logic to parse `<log_sample>`.

**Goal:** Extract specific data points into structured format.

**Extraction Targets:**
- Timestamp: Standardize to ISO 8601
- Error Level: (INFO, WARN, ERROR)
- Message Body: Core text after headers

**Data:**
- `<log_sample>[SAMPLE]</log_sample>`
```

```markdown
## Prompt 45: CSS Layout Generator

**Role:** Frontend Developer

**Instruction:** Write CSS code to achieve `<layout_goal>`.

**Constraints:**
- Use modern techniques only (`<constraints>` e.g., Flexbox or CSS Grid)
- Ensure responsiveness (include one media query breakpoint)

**Data:**
- `<layout_goal>[GOAL]</layout_goal>`
- `<constraints>[CONSTRAINTS]</constraints>`
```

```markdown
## Prompt 46: Academic Abstract Generator

**Role:** Research Editor

**Instruction:** Condense `<summary>` into formal academic abstract.

**Constraints:**
- Maximum Word Count: `<word_limit>`
- Structure: Background → Methods → Results → Conclusion
- Tone: Objective, passive voice where appropriate

**Data:**
- `<summary>[SUMMARY]</summary>`
- `<word_limit>[WORDS]</word_limit>`
```

```markdown
## Prompt 47: Dialectical Counter-Point

**Role:** Debater & Logician

**Instruction:** Analyze `<thesis>` and provide three rigorous counter-arguments.

**Structure:**
- **The Logical Flaw:** Attack internal consistency
- **The Empirical Gap:** Cite missing data/context
- **The Alternative Interpretation:** Propose different conclusion from same premises

**Data:**
- `<thesis>[THESIS]</thesis>`
```

```markdown
## Prompt 48: ELI5 Concept Simplifier

**Role:** Science Communicator

**Instruction:** Explain `<concept>` to a 10-year-old.

**Technique:** Use concrete analogy (e.g., "Think of it like a bicycle..."); avoid jargon; define technical terms immediately if necessary

**Data:**
- `<concept>[CONCEPT]</concept>`
```

```markdown
## Prompt 49: BibTeX Entry Formatter

**Role:** Academic Librarian

**Instruction:** Convert raw `<source_info>` into correctly formatted BibTeX entry.

**Validation:** Ensure specific fields (Author, Title, Year, Publisher/Journal) map correctly to entry type (article vs book vs misc)

**Data:**
- `<source_info>[INFO]</source_info>`
```

```markdown
## Prompt 50: Thesis Statement Architect

**Role:** Writing Professor

**Instruction:** Craft strong, debatable thesis statement for `<topic>` taking stance `<stance>`.

**Criteria:**
- Must not be statement of fact
- Must include "tension" or "contrast" (e.g., "While X is true, Y is more significant because...")

**Data:**
- `<topic>[TOPIC]</topic>`
- `<stance>[STANCE]</stance>`
```

```markdown
## Prompt 51: Peer Review Simulation

**Role:** Journal Reviewer

**Instruction:** Critically evaluate logic and evidence of `<essay>`.

**Output:**
- **Strength:** One aspect argued well
- **Weakness:** One logical leap or unsupported claim
- **Suggestion:** One specific source/angle to strengthen argument

**Data:**
- `<essay>[ESSAY]</essay>`
```

```markdown
## Prompt 52: Active Recall Generator

**Role:** Cognitive Psychologist

**Instruction:** Generate 10 study questions based on `<text>`.

**Design:**
- Questions 1-5: Fact retrieval (Who/What/When)
- Questions 6-10: Synthesis/Application (Why/How)
- Provide answer key at bottom

**Data:**
- `<text>[TEXT]</text>`
```

```markdown
## Prompt 53: Research Methodology Drafter

**Role:** Lead Researcher

**Instruction:** Draft "Methodology" section for study.

**Parameters:**
- Participants: `<sample_size>`
- Independent Variable: `<variable>`
- Instrument/Tool: `<tool>`

**Data:**
- `<sample_size>[SAMPLE]</sample_size>`
- `<variable>[VARIABLE]</variable>`
- `<tool>[TOOL]</tool>`
```

```markdown
## Prompt 54: Data Significance Interpreter

**Role:** Data Analyst

**Instruction:** Describe trends in `<data_points>`.

**Analysis:**
- **Direction:** Positive, negative, or flat?
- **Magnitude:** Significant or negligible?
- **Inference:** What might cause this pattern?

**Data:**
- `<data_points>[DATA]</data_points>`
```

```markdown
## Prompt 55: Literature Synthesis

**Role:** Meta-Analysis Author

**Instruction:** Synthesize `<summaries>` of three different papers.

**Goal:** Identify "Common Thread" they agree on and "Point of Contention" where they disagree

**Data:**
- `<summaries>[SUMMARIES]</summaries>`
```

```markdown
## Prompt 56: Job Description Architect

**Role:** HR Specialist

**Instruction:** Write comprehensive JD for `<role>`.

**Sections:**
- **Role Summary:** High-energy hook
- **Responsibilities:** Action verbs describing what they'll do
- **Requirements:** Hard skills `<skills>`
- **"Nice to Haves":** Soft skills or bonus tech

**Data:**
- `<role>[ROLE]</role>`
- `<skills>[SKILLS]</skills>`
```

```markdown
## Prompt 57: Empathetic Rejection Letter

**Role:** Talent Acquisition Manager

**Instruction:** Draft rejection email for `<candidate_name>`.

**Context:** Reached final round but not selected because of `<reasoning>`

**Tone:** Professional, encouraging, clear; no false hope but invite to stay in touch

**Data:**
- `<candidate_name>[NAME]</candidate_name>`
- `<reasoning>[REASONING]</reasoning>`
```

```markdown
## Prompt 58: Onboarding Roadmap

**Role:** People Operations Manager

**Instruction:** Create 7-day onboarding checklist for new `<role>`.

**Milestones:**
- **Day 1:** Logistics & Access
- **Day 3:** First "Quick Win" task
- **Day 7:** End-of-week review & goal setting

**Data:**
- `<role>[ROLE]</role>`
```

```markdown
## Prompt 59: Performance Review Script

**Role:** Manager

**Instruction:** Draft performance review script using "Sandwich Method" or "SBI" (Situation-Behavior-Impact).

**Structure:**
- **Highlight:** `<strengths>`
- **Constructive:** `<growth_areas>`
- **Action Plan:** Define next improvement step

**Data:**
- `<strengths>[STRENGTHS]</strengths>`
- `<growth_areas>[GROWTH]</growth_areas>`
```

```markdown
## Prompt 60: Formal Offer Letter

**Role:** HR Director

**Instruction:** Generate formal employment offer.

**Key Details:**
- Compensation: `<salary>`
- Start Date: `<date>`
- Perks: `<benefits>`
- Legalese: Include "At-will employment" placeholder

**Data:**
- `<salary>[SALARY]</salary>`
- `<date>[DATE]</date>`
- `<benefits>[BENEFITS]</benefits>`
```

```markdown
## Prompt 61: Interview Scorecard Designer

**Role:** Hiring Manager

**Instruction:** Design grading rubric for `<role>`.

**Competencies:** For each `<key_competency>`, provide specific question and description of "Good" vs "Bad" answer

**Data:**
- `<role>[ROLE]</role>`
- `<key_competencies>[COMPETENCIES]</key_competencies>`
```

```markdown
## Prompt 62: Internal Referral Request

**Role:** Recruiter

**Instruction:** Draft Slack/Email message asking for referrals for `<position>`.

**Incentive:** Highlight `<referral_bonus>`

**Call to Action:** "Who is the best [Role] you've ever worked with?"

**Data:**
- `<position>[POSITION]</position>`
- `<referral_bonus>[INCENTIVE]</referral_bonus>`
```

```markdown
## Prompt 63: Policy Update Memo

**Role:** Internal Comms Lead

**Instruction:** Write company-wide memo regarding Remote Work Policy changes.

**Structure:**
- **The Change:** Briefly state what's new: `<changes>`
- **The Why:** Explain reasoning
- **The When:** Effective date `<date>`

**Data:**
- `<changes>[CHANGES]</changes>`
- `<date>[DATE]</date>`
```

```markdown
## Prompt 64: Exit Interview Script

**Role:** HR Generalist

**Instruction:** Generate 10 targeted questions for exit interview in `<department>`.

**Goal:** Uncover hidden retention issues without making departing employee uncomfortable

**Data:**
- `<department>[DEPT]</department>`
```

```markdown
## Prompt 65: Employee Handbook Section

**Role:** Compliance Officer

**Instruction:** Write handbook section on `<topic>`.

**Tone:** Formal, clear, legally protective; avoid ambiguity

**Data:**
- `<topic>[TOPIC]</topic>`
```

```markdown
## Prompt 66: Character Profile Builder

**Role:** Novelist

**Instruction:** Create deep character profile.

**Inputs:**
- **Dominant Trait:** `<trait>`
- **Setting:** `<setting>`

**Output:**
- **The Want:** What they think they need
- **The Need:** What they actually need (subconscious)
- **The Ghost:** Past event that haunts them

**Data:**
- `<trait>[TRAIT]</trait>`
- `<setting>[SETTING]</setting>`
```

```markdown
## Prompt 67: Viral Thread Converter

**Role:** Social Media Ghostwriter

**Instruction:** Transform `<article>` into 5-part Twitter/X thread.

**Structure:**
- **Tweet 1:** The Hook (Problem/Promise)
- **Tweets 2-4:** The Value (Key points)
- **Tweet 5:** The CTA (Link back to source)

**Data:**
- `<article>[ARTICLE]</article>`
```

```markdown
## Prompt 68: Travel Itinerary Planner

**Role:** Luxury Travel Agent

**Instruction:** Plan 3-day itinerary for `<location>`.

**Customization:** Focus strictly on `<interests>`

**Logistics:** Group activities by neighborhood to minimize travel time

**Data:**
- `<location>[LOCATION]</location>`
- `<interests>[INTERESTS]</interests>`
```

```markdown
## Prompt 69: Pantry Chef Challenge

**Role:** Professional Chef

**Instruction:** Create recipe using only `<ingredients_list>`.

**Output:**
- Dish Name
- Prep time
- Step-by-step instructions maximizing flavor from limited inputs

**Data:**
- `<ingredients_list>[LIST]</ingredients_list>`
```

```markdown
## Prompt 70: Plot Twist Engine

**Role:** Screenwriter

**Instruction:** Brainstorm 3 plot twists for story with premise `<premise>`.

**Twist Types:**
- **The Betrayal:** An ally is an enemy
- **The Recontextualization:** The goal was wrong all along
- **The Deus Ex Machina Inversion:** Help arrives but makes things worse

**Data:**
- `<premise>[PREMISE]</premise>`
```

```markdown
## Prompt 71: World Building: Politics & Geography

**Role:** Fantasy Author

**Instruction:** Describe political system and geography based on theme `<theme>`.

**Connection:** Explain how geography (resources, terrain) directly influenced political system

**Data:**
- `<theme>[THEME]</theme>`
```

```markdown
## Prompt 72: Song Lyricist

**Role:** Songwriter

**Instruction:** Write chorus for song.

**Vibe:** Genre `<genre>`, Mood `<mood>`

**Structure:** A-A-B-A rhyme scheme (or genre appropriate)

**Data:**
- `<genre>[GENRE]</genre>`
- `<mood>[MOOD]</mood>`
```

```markdown
## Prompt 73: Gift Recommendation Engine

**Role:** Personal Shopper

**Instruction:** Suggest 5 distinct gift ideas.

**Recipient Profile:** Relation `<relation>`, Hobbies `<hobbies>`

**Constraint:** Must be under `<budget>`

**Data:**
- `<relation>[RELATION]</relation>`
- `<hobbies>[HOBBIES]</hobbies>`
- `<budget>[BUDGET]</budget>`
```

```markdown
## Prompt 74: Guided Meditation Script

**Role:** Mindfulness Coach

**Instruction:** Write 2-minute meditation script focused on `<goal>`.

**Sensory Cues:** Include breathing instructions (Inhale/Exhale) and body scanning

**Data:**
- `<goal>[GOAL]</goal>`
```

```markdown
## Prompt 75: Journaling Prompt Generator

**Role:** Therapist

**Instruction:** Provide 5 self-reflection prompts.

**Context:** For someone dealing with `<situation>`

**Goal:** Move user from "rumination" to "actionable insight"

**Data:**
- `<situation>[SITUATION]</situation>`
```

```markdown
## Prompt 76: Lesson Plan Designer

**Role:** Curriculum Developer

**Instruction:** Create 45-minute lesson plan for `<topic>` (Grade: `<grade>`).

**Timing:**
- 0-5: Hook
- 5-15: Direct Instruction
- 15-35: Guided Practice
- 35-45: Independent Assessment/Exit Ticket

**Data:**
- `<topic>[TOPIC]</topic>`
- `<grade>[GRADE]</grade>`
```

```markdown
## Prompt 77: Quiz Generator

**Role:** Exam Creator

**Instruction:** Generate 5 multiple-choice questions based on `<text>`.

**Format:**
- Question Stem
- 4 Options (1 Correct, 3 plausible Distractors)
- Explanation for correct answer

**Data:**
- `<text>[TEXT]</text>`
```

```markdown
## Prompt 78: Knowledge Gap Detector

**Role:** Tutor

**Instruction:** Analyze `<test_results>` to identify learning gaps.

**Output:**
- **The Weakness:** Specific concept missed
- **The Remediation:** What topic needs re-teaching?

**Data:**
- `<test_results>[RESULTS]</test_results>`
```

```markdown
## Prompt 79: Analogy Builder

**Role:** Master Teacher

**Instruction:** Create crystal-clear analogy to explain `<concept>` to beginner.

**Mapping:** Explicitly map analogy parts to real concept parts (e.g., "The nucleus is like the brain...")

**Data:**
- `<concept>[CONCEPT]</concept>`
```

```markdown
## Prompt 80: Progressive Practice Problems

**Role:** Math Teacher

**Instruction:** Generate 3 problems for `<skill>`.

**Progression:**
- **Beginner:** Basic application of rule
- **Intermediate:** Introduces constraint or variable
- **Advanced:** Word problem requiring synthesis

**Data:**
- `<skill>[SKILL]</skill>`
```

```markdown
## Prompt 81: Curriculum Roadmap

**Role:** Instructional Designer

**Instruction:** Outline 4-week curriculum to learn `<skill>` from scratch.

**Structure:**
- **Week 1:** Foundations
- **Week 2:** Core Mechanics
- **Week 3:** Advanced Techniques
- **Week 4:** Capstone Project

**Data:**
- `<skill>[SKILL]</skill>`
```

```markdown
## Prompt 82: Rubric Creator

**Role:** Education Consultant

**Instruction:** Build 4-point grading rubric for `<assignment_type>`.

**Criteria:** Define what constitutes 1, 2, 3, and 4 for criteria `<criteria>`

**Data:**
- `<assignment_type>[TYPE]</assignment_type>`
- `<criteria>[CRITERIA]</criteria>`
```

```markdown
## Prompt 83: Mnemonic Device Generator

**Role:** Memory Coach

**Instruction:** Create mnemonic to remember `<list>`.

**Options:** Provide one Acronym (e.g., HOMES) and one Acrostic phrase (e.g., Please Excuse My Dear Aunt Sally)

**Data:**
- `<list>[LIST]</list>`
```

```markdown
## Prompt 84: Case Study Writer

**Role:** Business School Professor

**Instruction:** Write 500-word case study based on `<real_event>`.

**Learning Objective:** Ensure narrative highlights lesson `<lesson>` for decision-making discussion

**Data:**
- `<real_event>[EVENT]</real_event>`
- `<lesson>[LESSON]</lesson>`
```

```markdown
## Prompt 85: Socratic Seminar Facilitator

**Role:** Discussion Leader

**Instruction:** Provide 3 open-ended questions to spark debate on `<topic>`.

**Levels:**
- **Clarification:** "What did the author mean by...?"
- **Implication:** "If this is true, what does it mean for...?"
- **Evaluation:** "Is it right that...?"

**Data:**
- `<topic>[TOPIC]</topic>`
```

```markdown
## Prompt 86: Non-Disclosure Agreement (NDA) Drafter

**Role:** Corporate Attorney

**Instruction:** Outline key clauses for Mutual NDA between `<party_a>` and `<party_b>`.

**Structure:**
- **Definition of Confidential Information:** What specific data falls under `<scope>`?
- **Exclusions:** What is not confidential?
- **Obligations:** How must data be handled?
- **Term:** Duration of agreement

**Data:**
- `<party_a>[A]</party_a>`
- `<party_b>[B]</party_b>`
- `<scope>[SCOPE]</scope>`
```

```markdown
## Prompt 87: Marketing Compliance Auditor

**Role:** Compliance Officer

**Instruction:** Review `<marketing_copy>` for violations of `<regulation>`.

**Output:**
- **Flagged Phrase:** Quote risky text
- **Violation Type:** Which specific rule does it break?
- **Remediation:** Rewrite phrase to be compliant while keeping sales punch

**Data:**
- `<marketing_copy>[COPY]</marketing_copy>`
- `<regulation>[REG]</regulation>`
```

```markdown
## Prompt 88: Privacy Policy Generator (GDPR/CCPA)

**Role:** Data Privacy Consultant

**Instruction:** Draft privacy policy section for `<data_type>` collected via `<tool>`.

**Requirements:**
- Explain why it's collected (Legal Basis)
- Explain how long it's stored (Retention)
- Explain user rights (e.g., Right to be Forgotten)

**Data:**
- `<data_type>[DATA]</data_type>`
- `<tool>[TOOL]</tool>`
```

```markdown
## Prompt 89: Contract Risk Analyzer

**Role:** General Counsel

**Instruction:** Analyze `<contract_clause>` for "Red Flags."

**Reasoning:**
- **Ambiguity:** Are terms vague?
- **Liability:** Does it shift unfair risk to us?
- **Termination:** Is there easy exit?

**Data:**
- `<contract_clause>[CLAUSE]</contract_clause>`
```

```markdown
## Prompt 90: TOS "Plain English" Translator

**Role:** Legal Tech Specialist

**Instruction:** Translate complex `<tos_text>` into 3 bullet points a 5th grader could understand.

**Goal:** Remove legalese; keep implication (e.g., "If you post it, we own it")

**Data:**
- `<tos_text>[TEXT]</tos_text>`
```

```markdown
## Prompt 91: Habit Loop Designer

**Role:** Behavioral Psychologist

**Instruction:** Design routine to build `<habits>` within `<time_constraint>`.

**Mechanism:** Use "Cue → Action → Reward" loop
- **Cue:** What trigger starts the habit?
- **Action:** The habit itself
- **Reward:** Immediate payoff

**Data:**
- `<habits>[HABITS]</habits>`
- `<time_constraint>[TIME]</time_constraint>`
```

```markdown
## Prompt 92: Adaptive Workout Planner

**Role:** Personal Trainer

**Instruction:** Create 30-minute workout based on `<equipment>`.

**Structure:**
- **Warm-up (5m):** Mobility work
- **Main Set (20m):** Circuit style targeting `<goal>`
- **Cool-down (5m):** Static stretching

**Data:**
- `<goal>[GOAL]</goal>`
- `<equipment>[EQUIP]</equipment>`
```

```markdown
## Prompt 93: Nutrient-Dense Meal Prepper

**Role:** Nutritionist

**Instruction:** Plan week of meals for `<diet>` on `<budget>`.

**Optimization:** Minimize waste by reusing ingredients; provide consolidated Grocery List

**Data:**
- `<diet>[DIET]</diet>`
- `<budget>[BUDGET]</budget>`
```

```markdown
## Prompt 94: SMART Goal Architect

**Role:** Life Coach

**Instruction:** Break down abstract `<goal>` into weekly SMART milestones.

**Criteria:**
- **Specific:** What exactly needs to happen?
- **Measurable:** How do we know it's done?
- **Time-bound:** Deadline for each milestone

**Data:**
- `<goal>[GOAL]</goal>`
```

```markdown
## Prompt 95: Stoic Quote Analyzer

**Role:** Philosopher

**Instruction:** Deconstruct `<quote>`.

**Analysis:**
- **Context:** Who said it and why?
- **Principle:** What core truth is conveyed?
- **Application:** How to apply to modern stressor?

**Data:**
- `<quote>[QUOTE]</quote>`
```

```markdown
## Prompt 96: Productivity Time Audit

**Role:** Efficiency Consultant

**Instruction:** Analyze `<daily_log>` to find "Time Leaks."

**Categorization:** Label activities as:
- Deep Work: High value
- Shallow Work: Admin/Maintenance
- Waste: Doomscrolling/Distraction

**Output:** Suggest one change to reclaim 60 minutes

**Data:**
- `<daily_log>[LOG]</daily_log>`
```

```markdown
## Prompt 97: Assertive Boundary Script

**Role:** Communication Coach

**Instruction:** Draft script to set boundary in `<situation>`.

**Tone:** "Polite but Firm"

**Formula:** "I value [Relationship], but I cannot [Action]. However, I can [Alternative]."

**Data:**
- `<situation>[SITUATION]</situation>`
```

```markdown
## Prompt 98: Sleep Hygiene Protocol

**Role:** Sleep Specialist

**Instruction:** Create 60-minute wind-down routine for `<lifestyle>` user.

**Phases:**
- **Environmental:** Lighting/Temp changes
- **Digital:** Screen boundaries
- **Physiological:** Stretching/Tea/Breathing

**Data:**
- `<lifestyle>[LIFESTYLE]</lifestyle>`
```

```markdown
## Prompt 99: Weighted Decision Matrix

**Role:** Decision Scientist

**Instruction:** Evaluate `<option_a>` vs `<option_b>`.

**Process:**
- Identify 3 key criteria (e.g., Cost, Time, Impact)
- Assign weight (1-5) to each criterion
- Score both options and calculate weighted total

**Data:**
- `<option_a>[A]</option_a>`
- `<option_b>[B]</option_b>`
```

```markdown
## Prompt 100: Targeted Affirmation Generator

**Role:** CBT Therapist

**Instruction:** Generate 10 affirmations to counteract insecurity: `<focus>`.

**Constraint:** Avoid toxic positivity; focus on Growth Mindset and self-efficacy (e.g., "I am capable of learning" vs "I am perfect")

**Data:**
- `<focus>[FOCUS]</focus>`
```

```markdown
## Prompt 101: Podcast Intro Script

**Role:** Radio Producer

**Instruction:** Write high-energy intro for podcast about `<topic>`.

**Elements:**
- **The Hook:** Provocative question
- **The Credibility:** Why listen to `<guest_name>`?
- **The Promise:** What listener will learn specifically

**Data:**
- `<guest_name>[GUEST]</guest_name>`
- `<topic>[TOPIC]</topic>`
```

```markdown
## Prompt 102: SEO Video Description

**Role:** YouTube Growth Strategist

**Instruction:** Write description for `<video_content>`.

**Components:**
- **First 2 lines:** Keyphrase-rich summary for search
- **Timestamps:** 5 key chapters
- **CTA:** Specific action `<call_to_action>`

**Data:**
- `<video_content>[CONTENT]</video_content>`
- `<call_to_action>[CTA]</call_to_action>`
```

```markdown
## Prompt 103: Emotional Beat Sheet

**Role:** Screenwriting Professor

**Instruction:** Breakdown scene with premise `<premise>`.

**Beats:**
- **Goal:** What does `<character>` want?
- **Obstacle:** What stops them?
- **Turning Point:** Moment the dynamic shifts
- **Resolution:** New status quo

**Data:**
- `<premise>[PREMISE]</premise>`
- `<character>[CHARACTERS]</character>`
```

```markdown
## Prompt 104: TikTok/Reels Hook Generator

**Role:** Short-Form Video Expert

**Instruction:** Generate 5 "Scroll-Stopping" opening lines for `<niche>`.

**Frameworks:**
- "Stop doing [X]..."
- "I tried [X] so you don't have to..."
- "The secret tool for [Goal]..."

**Data:**
- `<video_goal>[GOAL]</video_goal>`
- `<niche>[NICHE]</niche>`
```

```markdown
## Prompt 105: Voiceover Commercial Script

**Role:** Copywriter

**Instruction:** Write 30-second script (≈75 words) for `<service>`.

**Tone Direction:** `<key_tone>`

**Format:** Two columns—[Visual Cue] and [Audio/Spoken Word]

**Data:**
- `<service>[SERVICE]</service>`
- `<key_tone>[TONE]</key_tone>`
```

```markdown
## Prompt 106: Investigative Interviewer

**Role:** Journalist

**Instruction:** Draft 10 questions for `<subject>`.

**Flow:**
- 3 Warm-up questions (Establish context)
- 4 Deep Dive questions (Challenge `<context>`)
- 3 Reflection questions (Future outlook)

**Data:**
- `<subject>[SUBJECT]</subject>`
- `<context>[CONTEXT]</context>`
```

```markdown
## Prompt 107: Documentary Treatment

**Role:** Film Director

**Instruction:** Outline 3-act structure for documentary asking `<core_question>`.

**Visual Style:** Describe how `<visual_style>` (e.g., Cinema Verité, Archival, Animation) supports narrative

**Data:**
- `<core_question>[QUESTION]</core_question>`
- `<visual_style>[STYLE]</visual_style>`
```

```markdown
## Prompt 108: Livestream Run-of-Show

**Role:** Event Producer

**Instruction:** Create minute-by-minute schedule for 60-minute stream.

**Technical Check:** List specific assets needed for `<segments>` (e.g., "Screen Share ready," "Guest Mic Check")

**Data:**
- `<segments>[SEGMENTS]</segments>`
- `<tech_requirements>[TECH]</tech_requirements>`
```

```markdown
## Prompt 109: Caption Refiner

**Role:** Editor

**Instruction:** Edit `<raw_text>` captions.

**Goals:**
- Fix grammar/spelling
- Break lines for readability (max 2 lines per screen)
- Match rhythm of speech

**Data:**
- `<raw_text>[TEXT]</raw_text>`
```

```markdown
## Prompt 110: Click-Through Thumbnail Concept

**Role:** Graphic Designer

**Instruction:** Describe thumbnail for `<video_title>`.

**Elements:**
- **Foreground:** Main subject/face expression
- **Background:** Color contrast
- **Text Overlay:** Max 3 words, contrasting the title

**Data:**
- `<video_title>[TITLE]</video_title>`
- `<imagery>[IMAGE]</imagery>`
```

```markdown
## Prompt 111: Production Dockerfile Writer

**Role:** DevOps Engineer

**Instruction:** Write multi-stage Dockerfile for `<stack>`.

**Best Practices:**
- Use specific `<base_image>` digest if possible
- Minimize layer count
- Run as non-root user for security

**Data:**
- `<stack>[STACK]</stack>`
- `<base_image>[IMAGE]</base_image>`
```

```markdown
## Prompt 112: Kubernetes Manifest Architect

**Role:** Cloud Architect

**Instruction:** Create `deployment.yaml` and `service.yaml` for `<app_name>`.

**Requirements:**
- Expose port `<port>`
- Include Liveness and Readiness probes
- Define Resource Requests/Limits (CPU/Memory)

**Data:**
- `<app_name>[NAME]</app_name>`
- `<port>[PORT]</port>`
```

```markdown
## Prompt 113: Cloud Data Flow Logic

**Role:** Solutions Architect (AWS/Azure/GCP)

**Instruction:** Describe data flow through `<services>` to achieve `<goal>`.

**Output:** Step-by-step numbered list
- **Step 1:** Ingestion (Service A triggers Service B)
- **Step 2:** Processing (Transformation logic)
- **Step 3:** Storage (Persistence layer)

**Data:**
- `<services>[SERVICES]</services>`
- `<goal>[GOAL]</goal>`
```

```markdown
## Prompt 114: System Design Interview Prep

**Role:** Principal Engineer

**Instruction:** Outline high-level architecture for `<system>`.

**Scalability:** Specifically address `<scalability_need>` (e.g., "1M concurrent users")

**Components:**
- Load Balancer Strategy
- Database Choice (SQL vs NoSQL) & Sharding key
- Caching Strategy (Redis/Memcached)

**Data:**
- `<system>[SYSTEM]</system>`
- `<scalability_need>[NEED]</scalability_need>`
```

```markdown
## Prompt 115: Microservice IDL Definer

**Role:** Backend Lead

**Instruction:** Define Interface Definition Language (Proto3 or OpenAPI) for `<service_name>`.

**Methods:** Include request/response messages for `<methods>`

**Versioning:** Ensure forward-compatible definition

**Data:**
- `<service_name>[NAME]</service_name>`
- `<methods>[METHODS]</methods>`
```

```markdown
## Prompt 116: Legacy Migration Planner

**Role:** Modernization Consultant

**Instruction:** Outline steps to migrate from `<old_stack>` to `<new_stack>` using "Strangler Fig" pattern.

**Strategy:**
- Identify low-risk module to move first
- Build anti-corruption layer
- Cutover traffic

**Data:**
- `<old_stack>[OLD]</old_stack>`
- `<new_stack>[NEW]</new_stack>`
```

```markdown
## Prompt 117: Security Remediation Report

**Role:** InfoSec Analyst

**Instruction:** Summarize `<vulnerability>`.

**Impact Analysis:** Potential damage `<impact>`

**Remediation:**
- **Immediate Fix:** Patch/Config change
- **Long-term Fix:** Architectural change to prevent recurrence

**Data:**
- `<vulnerability>[VULN]</vulnerability>`
- `<impact>[IMPACT]</impact>`
```

```markdown
## Prompt 118: CI/CD Workflow Designer

**Role:** Release Manager

**Instruction:** Define pipeline (GitHub Actions/GitLab CI) structure.

**Triggers:** `<triggers>` (e.g., Push to Main, PR)

**Jobs:**
- **Lint/Test:** Parallelized
- **Build:** Docker container creation
- **Deploy:** Staging vs Production logic based on branch

**Data:**
- `<triggers>[TRIGGERS]</triggers>`
- `<jobs>[JOBS]</jobs>`
```

```markdown
## Prompt 119: Load Test Strategy

**Role:** QA Performance Engineer

**Instruction:** Design load test for `<endpoint>`.

**Parameters:**
- **Ramp-up:** How fast to reach `<peak_load>`?
- **Duration:** How long to sustain?
- **Success Criteria:** Max latency (p95) and Error rate (<1%)

**Data:**
- `<endpoint>[URL]</endpoint>`
- `<peak_load>[LOAD]</peak_load>`
```

```markdown
## Prompt 120: Global Error Handling Pattern

**Role:** Software Architect

**Instruction:** Design global error handling strategy for `<language>`.

**Context:** Current pattern is `<existing_pattern>`

**Goal:** Centralized logging, user-friendly UI messages, obfuscated stack traces in production

**Data:**
- `<language>[LANG]</language>`
- `<existing_pattern>[PATTERN]</existing_pattern>`
```

```markdown
## Prompt 121: Python Data Cleaning Pipeline

**Role:** Data Engineer

**Instruction:** Write production-grade Pandas script to clean dataset described in `<dataset_description>`.

**Process:**
- **Typecasting:** Normalize `<columns>` to correct dtypes (datetime, categorical)
- **Imputation:** Handle missing values—median for numeric, 'Unknown' for categorical
- **Vectorization:** Ensure no for loops

**Data:**
- `<dataset_description>[DATA]</dataset_description>`
- `<columns>[COLUMNS]</columns>`
```

```markdown
## Prompt 122: Feature Engineering Strategist

**Role:** Kaggle Grandmaster

**Instruction:** Suggest 5 new features from `<raw_columns>` to improve prediction for `<target_variable>`.

**Reasoning:**
- **Interaction Features:** Combine columns (e.g., Ratio of A/B)
- **Temporal Features:** Extract cyclical data (Day of Week, Seasonality)
- **Domain Specific:** Apply context-relevant logic

**Data:**
- `<raw_columns>[COLS]</raw_columns>`
- `<target_variable>[TARGET]</target_variable>`
```

```markdown
## Prompt 123: Model Metrics Interpreter

**Role:** Lead Data Scientist

**Instruction:** Interpret `<metrics>` for model in `<context>`.

**Analysis:**
- **Diagnosis:** Overfitting or underfitting?
- **Trade-off:** Discuss Precision vs Recall implications
- **Next Step:** Suggest one hyperparameter to tune

**Data:**
- `<metrics>[METRICS]</metrics>`
- `<context>[CONTEXT]</context>`
```

```markdown
## Prompt 124: Advanced SQL Aggregation

**Role:** Analytics Engineer

**Instruction:** Write SQL query using Window Functions for `<analysis_goal>`.

**Logic:**
- Use `PARTITION BY` to segment analysis
- Use `RANK()` or `LEAD()/LAG()` as appropriate
- Optimize readability (CTE usage)

**Data:**
- `<tables>[TABLES]</tables>`
- `<analysis_goal>[GOAL]</analysis_goal>`
```

```markdown
## Prompt 125: Neural Network Architect

**Role:** Deep Learning Researcher

**Instruction:** Design neural network for `<problem_type>` using PyTorch/TensorFlow.

**Architecture:**
- **Input Layer:** Match shape `<input_shape>`
- **Hidden Layers:** Define activations (ReLU/GeLU) and dropout rates
- **Output Layer:** Appropriate activation (Sigmoid vs Softmax)

**Data:**
- `<problem_type>[TYPE]</problem_type>`
- `<input_shape>[SHAPE]</input_shape>`
```

```markdown
## Prompt 126: A/B Test Design Logic

**Role:** Statistician

**Instruction:** Design A/B test for `<metric>`.

**Hypotheses:**
- **Null ($H_0$):** `<variable_change>` has no effect
- **Alternative ($H_1$):** Change causes statistically significant difference

**Power Analysis:** Define minimum detectable effect (MDE)

**Data:**
- `<metric>[METRIC]</metric>`
- `<variable_change>[CHANGE]</variable_change>`
```

```markdown
## Prompt 127: Data Visualization Consultant

**Role:** Information Designer

**Instruction:** Recommend optimal chart types for showing `<trend>` to `<audience>`.

**Principles:**
- **Cognitive Load:** Minimize chartjunk
- **Comparison:** Bar/Column for values, Scatter for correlation
- **Color Theory:** Use color to highlight insight, not decoration

**Data:**
- `<trend>[TREND]</trend>`
- `<audience>[AUDIENCE]</audience>`
```

```markdown
## Prompt 128: NLP Preprocessing Pipeline

**Role:** NLP Engineer

**Instruction:** Write Python function to preprocess `<raw_text>`.

**Steps:**
- **Tokenization:** Split text into units
- **Normalization:** Lowercase, remove special characters
- **Lemmatization:** Reduce to root form (Spacy/NLTK)
- **Stopword Removal:** Context-aware removal

**Data:**
- `<raw_text>[TEXT]</raw_text>`
```

```markdown
## Prompt 129: Anomaly Detection Strategy

**Role:** Fraud Detection Analyst

**Instruction:** Suggest algorithm to detect outliers in `<data_stream>`.

**Logic:**
- **Baseline:** Define "normal" from `<expected_baseline>`
- **Threshold:** Z-score or Isolation Forest score for anomaly detection
- **Alerting:** Real-time trigger condition

**Data:**
- `<data_stream>[STREAM]</data_stream>`
- `<expected_baseline>[BASE]</expected_baseline>`
```

```markdown
## Prompt 130: MLOps Monitoring Plan

**Role:** Machine Learning Engineer

**Instruction:** Outline monitoring strategy for `<model_type>` in production.

**Drift Detection:**
- **Data Drift:** Monitor input distributions (KL Divergence)
- **Concept Drift:** Monitor input-target relationship
- **Retraining Policy:** Trigger when `<drift_metrics>` exceed threshold X

**Data:**
- `<model_type>[MODEL]</model_type>`
- `<drift_metrics>[METRICS]</drift_metrics>`
```

```markdown
## Prompt 131: User Research Script

**Role:** UX Researcher

**Instruction:** Draft 10 interview questions to uncover pain points for `<product>` (`<segment>`).

**Question Types:**
- **Behavioral:** "Tell me about the last time you..." (Not "Would you...")
- **Barrier:** "What is the hardest part about..."
- **Workaround:** "How do you currently solve this?"

**Data:**
- `<product>[PRODUCT]</product>`
- `<segment>[SEGMENT]</segment>`
```

```markdown
## Prompt 132: Accessibility (A11y) Auditor

**Role:** Accessibility Specialist

**Instruction:** Audit `<ui_description>` against `<wcag_level>` standards.

**Checklist:**
- **Visual:** Contrast ratios and Color blindness safety
- **Interaction:** Keyboard navigability (Tab index)
- **Screen Readers:** Alt text and ARIA labels

**Data:**
- `<ui_description>[UI]</ui_description>`
- `<wcag_level>[WCAG_LEVEL]</wcag_level>`
```

```markdown
## Prompt 133: UX Microcopy Writer

**Role:** Content Designer

**Instruction:** Draft 3 variations of error message for `<context>`.

**Variations:**
- **The Direct:** Plain statement of fact
- **The Helpful:** Focus entirely on solution
- **The Human:** Empathetic `<tone>`

**Data:**
- `<context>[CONTEXT]</context>`
- `<tone>[TONE]</tone>`
```

```markdown
## Prompt 134: Design System Tokenizer

**Role:** Design Ops Lead

**Instruction:** Create semantic naming convention for color tokens from `<brand_color>`.

**Structure:**
- **Base:** `primary-500` (The hex provided)
- **Interaction:** `primary-hover`, `primary-active`
- **Semantic:** `action-bg`, `text-link`
- **Scope:** Limit to `<usage_scope>`

**Data:**
- `<brand_color>[HEX]</brand_color>`
- `<usage_scope>[SCOPE]</usage_scope>`
```

```markdown
## Prompt 135: User Flow Mapper

**Role:** Product Designer

**Instruction:** Describe logic flow for `<task>` starting from `<start_point>`.

**Step Format:**
- **User Action:** (Clicks X)
- **System Response:** (Loading state / Validation)
- **Decision Node:** (If success → Y, If error → Z)

**Data:**
- `<task>[TASK]</task>`
- `<start_point>[START]</start_point>`
```

```markdown
## Prompt 136: Wireframe Layout Specification

**Role:** UI Designer

**Instruction:** List mandatory elements for `<page_type>` wireframe.

**Prioritization:** Order elements by hierarchy to achieve `<primary_goal>`

**Elements:**
- **Global Nav:** Breadcrumbs/Menu
- **Hero/Header:** H1 + Primary Action
- **Content Body:** Data visualization or Form fields

**Data:**
- `<page_type>[TYPE]</page_type>`
- `<primary_goal>[GOAL]</primary_goal>`
```

```markdown
## Prompt 137: Conversion Rate Optimization (CRO) Test

**Role:** Growth Designer

**Instruction:** Propose two UI variants to beat `<current_ui>`.

**Hypothesis:**
- **Variant A:** Change layout emphasis to reduce friction
- **Variant B:** Change copy framing to increase motivation

**Goal:** Improve `<goal>`

**Data:**
- `<current_ui>[UI]</current_ui>`
- `<goal>[GOAL]</goal>`
```

```markdown
## Prompt 138: Information Architecture (IA) Sitemap

**Role:** IA Architect

**Instruction:** Organize `<pages>` into logical hierarchy.

**Structure:**
- **Level 1:** Main Navigation
- **Level 2:** Sub-menus/Categories
- **Level 3:** Detail pages

**Goal:** Minimize clicks to reach `<main_goal>`

**Data:**
- `<pages>[PAGES]</pages>`
- `<main_goal>[GOAL]</main_goal>`
```

```markdown
## Prompt 139: Usability Test Protocol

**Role:** User Researcher

**Instruction:** Write task scenario for testing `<feature>`.

**Scenario:** "Imagine you are [Persona]. You need to `<scenario>`. Show me how you would do that."

**Success Criteria:**
- Did they find entry point?
- Time on task
- Errors committed

**Data:**
- `<feature>[FEATURE]</feature>`
- `<scenario>[SCENARIO]</scenario>`
```

```markdown
## Prompt 140: Mood Board Curator

**Role:** Art Director

**Instruction:** Describe visual direction for brand with value `<brand_value>`.

**Directives:**
- **Color Palette:** (e.g., Muted Pastels vs Neon)
- **Typography:** (Serif vs Sans; Geometric vs Humanist)
- **Imagery:** (Abstract vs Photorealistic)
- **Target:** `<target_industry>`

**Data:**
- `<brand_value>[VALUE]</brand_value>`
- `<target_industry>[INDUSTRY]</target_industry>`
```

```markdown
## Prompt 141: Objection Handling Script

**Role:** Sales Coach

**Instruction:** Write script to handle objection `<objection>` using LARA framework (Listen, Acknowledge, Respond, Ask).

- **Acknowledge:** Validate concern (Empathy)
- **Respond:** Pivot to `<product_usp>` that solves it
- **Ask:** Check for understanding ("Does that make sense?")

**Data:**
- `<objection>[OBJECTION]</objection>`
- `<product_usp>[USP]</product_usp>`
```

```markdown
## Prompt 142: Strategic Renewal Email

**Role:** Account Manager

**Instruction:** Draft renewal email for client.

**Strategy:**
- **Look Back:** Summarize usage/success from `<client_history>`
- **Look Forward:** Highlight new `<benefit_focus>` relevant to next year's goals
- **Call to Action:** Schedule review call

**Data:**
- `<client_history>[HISTORY]</client_history>`
- `<benefit_focus>[BENEFIT]</benefit_focus>`
```

```markdown
## Prompt 143: Case Study Interviewer

**Role:** Customer Marketing Manager

**Instruction:** Draft 5 questions to interview client about `<project_detail>`.

**Narrative Arc:**
- **Before:** What was the pain?
- **During:** What was implementation experience?
- **After:** Specific metrics of `<result>`

**Data:**
- `<project_detail>[PROJECT]</project_detail>`
- `<result>[RESULT]</result>`
```

```markdown
## Prompt 144: Discovery Call Flow

**Role:** SDR (Sales Development Rep)

**Instruction:** Outline 15-minute qualification call for `<product>` using BANT framework.

- **Budget:** Soft check ("Is this a prioritized initiative?")
- **Authority:** ("Who else is involved?")
- **Need:** ("Why now?")
- **Timing:** ("When do you need this live?")

**Data:**
- `<product>[PRODUCT]</product>`
- `<ideal_lead>[LEAD]</ideal_lead>`
```

```markdown
## Prompt 145: Upsell Proposal Logic

**Role:** Enterprise Account Executive

**Instruction:** Pitch Enterprise Tier to client currently on Basic.

**Gap Analysis:**
- **Current State:** Hitting limits in `<client_usage>`
- **Risk:** Remaining on Basic risks [Outcome]
- **Solution:** `<missing_feature>` removes that ceiling

**Data:**
- `<client_usage>[USAGE]</client_usage>`
- `<missing_feature>[FEATURE]</missing_feature>`
```

```markdown
## Prompt 146: Customer Health Score Algorithm

**Role:** VP of Customer Success

**Instruction:** Define "Health Score" (0-100) calculation.

**Components:**
- **Product Adoption:** Frequency of `<signals>`
- **Support Volume:** Ticket count (High = low health?)
- **Sentiment:** NPS or Survey score

**Alerts:** Trigger "Risk Intervention" if score drops below `<thresholds>`

**Data:**
- `<signals>[SIGNALS]</signals>`
- `<thresholds>[THRESHOLDS]</thresholds>`
```

```markdown
## Prompt 147: Churn Recovery Sequence

**Role:** Retention Specialist

**Instruction:** Draft re-engagement email sequence for user inactive for `<inactivity_time>`.

**Sequence:**
- **Email 1:** "Is everything okay?" (Service focus)
- **Email 2:** "Here's what you missed." (New features)
- **Email 3:** "One last offer." (Incentive)

**Data:**
- `<inactivity_time>[TIME]</inactivity_time>`
- `<last_interaction>[LAST]</last_interaction>`
```

```markdown
## Prompt 148: Referral Program Pitch

**Role:** Growth Marketer

**Instruction:** Write in-app popup copy to drive referrals.

**Psychology:**
- **Altruism:** "Help your friends"
- **Self-Interest:** Get `<reward>`
- **Ease:** "One click to share `<link>`"

**Data:**
- `<reward>[REWARD]</reward>`
- `<link>[LINK]</link>`
```

```markdown
## Prompt 149: Post-Onboarding Survey

**Role:** CS Operations

**Instruction:** Generate 5 questions to measure "Time to Value" for `<target_role>`.

**Focus:**
- Was training clear?
- Do you feel confident to perform [Core Task]?
- What was biggest friction point?

**Data:**
- `<target_role>[ROLE]</target_role>`
```

```markdown
## Prompt 150: QBR (Quarterly Business Review) Agenda

**Role:** Customer Success Manager

**Instruction:** Create agenda for QBR with `<account_name>`.

**Structure:**
- **Executive Summary:** High-level ROI delivered
- **Performance Review:** Data vs Goals
- **The Elephant:** Address `<main_issue>` head-on with plan
- **Roadmap:** Next quarter's goals

**Data:**
- `<account_name>[NAME]</account_name>`
- `<main_issue>[ISSUE]</main_issue>`
```

```markdown
## Prompt 151: Wedding Day Run-of-Show

**Role:** Wedding Planner

**Instruction:** Create timeline for wedding with `<guest_count>` guests.

**Precision:**
- **Ceremony:** Starts at `<ceremony_time>`
- **Buffer:** Add 15m buffers for transport/photos
- **Vendor Cues:** When do caterers/band need to set up?

**Data:**
- `<ceremony_time>[TIME]</ceremony_time>`
- `<guest_count>[COUNT]</guest_count>`
```

```markdown
## Prompt 152: Conference Session Titling

**Role:** Conference Organizer

**Instruction:** Generate 10 titles for workshop on `<topic>`.

**Categories:**
- **Instructional:** "How to..."
- **Outcome-based:** "Achieve `<outcome>` in X Steps"
- **Intriguing:** "The Truth About..."

**Data:**
- `<topic>[TOPIC]</topic>`
- `<outcome>[OUTCOME]</outcome>`
```

```markdown
## Prompt 153: Themed Catering Menu

**Role:** Executive Chef

**Instruction:** Design menu for `<theme>` corporate event.

**Constraints:**
- Must accommodate `<dietary_restrictions>`
- Structure: 2 Appetizers, 3 Mains, 2 Sides, 1 Dessert
- Description: Use sensory words (crisp, savory, glazed)

**Data:**
- `<theme>[THEME]</theme>`
- `<dietary_restrictions>[RESTRICTIONS]</dietary_restrictions>`
```

```markdown
## Prompt 154: Venue RFP (Request for Proposal)

**Role:** Event Director

**Instruction:** Draft formal RFP for `<event_type>`.

**Specs:**
- **Capacity:** Need space for X people
- **Requirements:** `<requirements>` (e.g., AV, Breakout rooms, Catering)
- **Question:** Ask for line-item quote including service fees/taxes

**Data:**
- `<event_type>[TYPE]</event_type>`
- `<requirements>[REQS]</requirements>`
```

```markdown
## Prompt 155: Speaker Briefing Packet

**Role:** Content Producer

**Instruction:** Write briefing guide for guest speaker.

**Sections:**
- **Audience Persona:** Who are `<audience>`? (Experience level, pain points)
- **Logistics:** Date, Time, Tech check
- **Content Guardrails:** Cover `<key_topics>`; avoid pitching

**Data:**
- `<audience>[AUDIENCE]</audience>`
- `<key_topics>[TOPICS]</key_topics>`
```

```markdown
## Prompt 156: Event Budget Estimator

**Role:** Event Finance Manager

**Instruction:** Outline budget allocation for `<event_type>` with `<total_budget>`.

**Categories:**
- **Venue/F&B:** ~40%
- **AV/Production:** ~20%
- **Marketing:** ~10%
- **Contingency:** 10%
- (Adjust percentages based on event type)

**Data:**
- `<event_type>[TYPE]</event_type>`
- `<total_budget>[BUDGET]</total_budget>`
```

```markdown
## Prompt 157: Registration Form Logic

**Role:** Registration Manager

**Instruction:** Design data fields for event signup form focused on `<event_focus>`.

**Standard:** Name, Email, Company

**Custom Questions:**
- **Segmentation:** "What is your primary goal for attending?"
- **Logistics:** "Do you require ADA assistance?"

**Data:**
- `<event_focus>[FOCUS]</event_focus>`
```

```markdown
## Prompt 158: Volunteer Coordination Plan

**Role:** Volunteer Coordinator

**Instruction:** Draft email assigning roles to volunteers at `<location>`.

**Clarity:**
- **Role Description:** What does `<role>` actually do?
- **Shift Time:** Arrival vs Start time
- **Contact:** Who is on-site lead?

**Data:**
- `<role>[ROLES]</role>`
- `<location>[LOC]</location>`
```

```markdown
## Prompt 159: Post-Event Impact Report

**Role:** Event Analyst

**Instruction:** Summarize event success for stakeholders.

**Metrics:**
- **Attendance:** `<stats>` (Registered vs Actual)
- **Satisfaction:** NPS or CSAT
- **Qualitative:** Summary of `<top_feedback>`

**Data:**
- `<stats>[STATS]</stats>`
- `<top_feedback>[FEEDBACK]</top_feedback>`
```

```markdown
## Prompt 160: Guest Welcome Note

**Role:** Hospitality Manager

**Instruction:** Write warm, handwritten-style note for guests at `<property_name>`.

**Personalization:**
- Welcome them to the city
- Share "Secret" `<local_tip>` (e.g., best coffee nearby)
- Contact info for immediate needs

**Data:**
- `<property_name>[NAME]</property_name>`
- `<local_tip>[TIP]</local_tip>`
```

```markdown
## Prompt 201: Carbon Footprint Auditor

**Role:** Sustainability Consultant

**Instruction:** Audit `<lifestyle_log>` to identify top 3 emission sources.

**Output:**
- **The Hotspot:** Which activity creates most CO2e?
- **The Fix:** One "High Impact" change (e.g., flight reduction) and one "Low Effort" change (e.g., LED bulbs)

**Data:**
- `<lifestyle_log>[LOG]</lifestyle_log>`
```

```markdown
## Prompt 202: Sustainable Packaging Engineer

**Role:** Materials Scientist

**Instruction:** Suggest eco-friendly alternative to `<current_material>`.

**Criteria:**
- **Functionality:** Must meet `<product_needs>` (moisture barrier, crush resistance)
- **End-of-Life:** Is it compostable, recyclable, or reusable?

**Data:**
- `<current_material>[OLD]</current_material>`
- `<product_needs>[NEEDS]</product_needs>`
```

```markdown
## Prompt 203: Companion Planting Guide

**Role:** Master Gardener

**Instruction:** Design garden layout for `<hardiness_zone>` in `<space_size>` plot using "Guilds."

**Logic:**
- **Nitrogen Fixers:** (e.g., Beans)
- **Pest Repellers:** (e.g., Marigolds)
- **Layout:** Grid or Row based on sun exposure

**Data:**
- `<hardiness_zone>[ZONE]</hardiness_zone>`
- `<space_size>[SIZE]</space_size>`
```

```markdown
## Prompt 204: Green Tech Analyst

**Role:** CleanTech Investor

**Instruction:** Explain mechanics of `<technology>`.

**Analysis:**
- **The Physics:** How does it work?
- **The Impact:** Potential reduction in Gt (Gigatons) of CO2
- **The Barrier:** What stops scaling (Cost, Grid, Physics)?

**Data:**
- `<technology>[TECH]</technology>`
```

```markdown
## Prompt 205: Zero-Waste Grocery Planner

**Role:** Eco-Lifestyle Coach

**Instruction:** Convert `<original_list>` into zero-waste plan.

**Strategy:**
- **Bulk Bin:** Items to buy in own containers
- **Plastic Swaps:** (e.g., Bar soap vs Liquid)
- **Local Source:** Farmers market vs Imported

**Data:**
- `<original_list>[LIST]</original_list>`
```

```markdown
## Prompt 206: Home Energy Auditor

**Role:** Energy Efficiency Expert

**Instruction:** Identify "low-hanging fruit" for `<house_description>`.

**Priorities:**
- **Insulation:** Attic/Window leaks
- **Phantom Load:** Devices to unplug
- **HVAC:** Setpoint adjustments

**Data:**
- `<house_description>[DESC]</house_description>`
```

```markdown
## Prompt 207: Industrial Water Conservation

**Role:** Process Engineer

**Instruction:** Suggest 5 methods to reduce water usage in `<industry_type>`.

**Hierarchy:**
- **Reduce:** Process optimization
- **Reuse:** Greywater recycling
- **Recycle:** On-site treatment

**Data:**
- `<industry_type>[TYPE]</industry_type>`
```

```markdown
## Prompt 208: Ecotourism Itinerary

**Role:** Sustainable Travel Agent

**Instruction:** Plan 5-day trip to `<destination>`.

**Constraints:**
- **Transit:** Public transport or walking/biking only
- **Stay:** Locally owned eco-lodges (avoid chains)
- **Activity:** "Leave No Trace" compliant

**Data:**
- `<destination>[DEST]</destination>`
```

```markdown
## Prompt 209: Sustainability Report Executive Summary

**Role:** ESG Analyst

**Instruction:** Summarize `<company_name>` report for `<year>`.

**Key Metrics:**
- **Scope 1, 2, 3 Emissions:** Trend line
- **Water/Waste:** Diversion rates
- **Social:** DEI or Labor improvements

**Data:**
- `<company_name>[NAME]</company_name>`
- `<year>[YEAR]</year>`
```

```markdown
## Prompt 210: Composting Troubleshooter

**Role:** Soil Scientist

**Instruction:** Diagnose issue `<issue>` in `<bin_type>` bin.

**Solution:**
- **The "Greens" (Nitrogen):** Too much/little?
- **The "Browns" (Carbon):** Need more paper/leaves?
- **Moisture:** Sponge test

**Data:**
- `<issue>[ISSUE]</issue>`
- `<bin_type>[BIN]</bin_type>`
```

```markdown
## Prompt 211: Logical Fallacy Detector

**Role:** Logic Professor

**Instruction:** Identify specific fallacy in `<argument_text>`.

**Output:**
- **Name:** (e.g., Ad Hominem, Strawman)
- **Definition:** Brief explanation of error
- **Correction:** How to restate argument validly

**Data:**
- `<argument_text>[TEXT]</argument_text>`
```

```markdown
## Prompt 212: Ethical Dilemma Resolver

**Role:** Ethicist

**Instruction:** Analyze `<dilemma>` through 3 frameworks.

- **Utilitarianism:** Greatest good for greatest number
- **Deontology:** Adherence to moral duties/rules
- **Virtue Ethics:** Character of the actor

**Synthesis:** Provide final recommendation

**Data:**
- `<dilemma>[SITUATION]</dilemma>`
```

```markdown
## Prompt 213: Debate Prep (Steel Man)

**Role:** Debate Coach

**Instruction:** Provide 3 strongest arguments For and Against `<resolution>`.

**Rule:** Use "Steel Man" technique (make opposing argument as strong as possible before refuting)

**Data:**
- `<resolution>[RESOLUTION]</resolution>`
```

```markdown
## Prompt 214: Thought Experiment Deconstructor

**Role:** Philosophy Historian

**Instruction:** Explain `<experiment_name>`.

**Context:**
- **Origin:** Who proposed it?
- **Implication:** What concept does it challenge (Consciousness, Identity)?
- **Modern View:** Is it still relevant?

**Data:**
- `<experiment_name>[NAME]</experiment_name>`
```

```markdown
## Prompt 215: Assumption Challenger

**Role:** Critical Thinking Coach

**Instruction:** Generate "Deep Question" to challenge consensus on `<topic>`.

**Goal:** Expose hidden biases or unproven axioms

**Data:**
- `<topic>[TOPIC]</topic>`
```

```markdown
## Prompt 216: Philosophy for Modern Life

**Role:** Practical Philosopher

**Instruction:** Explain core tenets of `<philosophy_name>` and apply to daily stress.

**Actionable Advice:** "When you feel X, apply concept Y"

**Data:**
- `<philosophy_name>[NAME]</philosophy_name>`
```

```markdown
## Prompt 217: Cognitive Bias Scanner

**Role:** Media Literacy Expert

**Instruction:** Scan `<news_text>` for bias.

**Flags:**
- **Loaded Language:** Emotional adjectives
- **Selection Bias:** What facts were omitted?
- **Framing:** Is headline misleading?

**Data:**
- `<news_text>[TEXT]</news_text>`
```

```markdown
## Prompt 218: Socratic Dialogue Script

**Role:** Playwright / Philosopher

**Instruction:** Write dialogue between "Master" and "Student" exploring `<concept>`.

**Method:** Master never states answer, only asks questions leading Student to truth (Elenchus)

**Data:**
- `<concept>[CONCEPT]</concept>`
```

```markdown
## Prompt 219: Policy Impact Analysis

**Role:** Policy Analyst

**Instruction:** Evaluate unintended consequences of `<policy>`.

**Systems Thinking:**
- **First Order:** Immediate effect
- **Second Order:** Reactionary behavior change
- **Third Order:** Long-term societal shift

**Data:**
- `<policy>[POLICY]</policy>`
```

```markdown
## Prompt 220: Stoic Exercise Generator

**Role:** Stoic Mentor

**Instruction:** Provide mental exercise for `<trigger>`.

**Technique:** Use "The Dichotomy of Control" or "Negative Visualization"

**Data:**
- `<trigger>[TRIGGER]</trigger>`
```

```markdown
## Prompt 221: Community Constitution (Ruleset)

**Role:** Community Manager

**Instruction:** Draft 5 core rules for `<community_focus>` group.

**Tone:** "Firm but Fair"

**Focus:** Prevent toxicity while encouraging engagement; include "Enforcement" policy

**Data:**
- `<community_focus>[FOCUS]</community_focus>`
```

```markdown
## Prompt 222: Engagement Starter Pack

**Role:** Forum Moderator

**Instruction:** Generate 10 discussion questions for `<niche_group>`.

**Mix:**
- 3 "Hot Takes" (Controversial but safe)
- 4 "Help" requests (People love giving advice)
- 3 "Show off" (Share your setup/work)

**Data:**
- `<niche_group>[NICHE]</niche_group>`
```

```markdown
## Prompt 223: Crisis De-escalation Reply

**Role:** PR Specialist

**Instruction:** Draft reply to public complaint `<complaint_text>`.

**Goals:**
- Move conversation to DM/Private channel
- Validate frustration
- Maintain professional boundaries

**Data:**
- `<complaint_text>[TEXT]</complaint_text>`
```

```markdown
## Prompt 224: Cross-Platform Content Calendar

**Role:** Social Media Strategist

**Instruction:** Plan one week of content for `<brand>` (Goal: `<goal>`).

**Platforms:**
- **LinkedIn:** Thought Leadership
- **Twitter/X:** Short threads/polls
- **Instagram/TikTok:** Visuals/Behind-the-scenes

**Data:**
- `<brand>[NAME]</brand>`
- `<goal>[GOAL]</goal>`
```

```markdown
## Prompt 225: UGC (User Generated Content) Contest

**Role:** Growth Hacker

**Instruction:** Design contest for `<product>`.

**Mechanics:**
- **Prompt:** "Show us how you use..."
- **Incentive:** `<prize>`
- **Friction:** Keep entry requirements low

**Data:**
- `<product>[PRODUCT]</product>`
- `<prize>[PRIZE]</prize>`
```

```markdown
## Prompt 226: Newsletter Open Rate Booster

**Role:** Email Copywriter

**Instruction:** Suggest 3 tactics to improve open rates for `<topic>` (Current: `<current_rate>`).

**Tactics:**
- **Sender Name:** Personalize?
- **Preview Text:** Complete the thought
- **List Hygiene:** Re-engagement campaign

**Data:**
- `<topic>[TOPIC]</topic>`
- `<current_rate>[RATE]</current_rate>`
```

```markdown
## Prompt 227: Viral LinkedIn Post

**Role:** Ghostwriter

**Instruction:** Convert insight `<insight>` into "Broetry" style post.

**Format:**
- Short, punchy sentences
- Heavy line spacing
- "The Lesson" at bottom

**Data:**
- `<insight>[INSIGHT]</insight>`
```

```markdown
## Prompt 228: AMA (Ask Me Anything) Moderator Guide

**Role:** Event Host

**Instruction:** Create run-sheet for AMA with `<guest>` on `<platform>`.

**Prep:**
- "Seed Questions" in case audience is slow
- Time management rules
- Handling trolls

**Data:**
- `<guest>[GUEST]</guest>`
- `<platform>[PLATFORM]</platform>`
```

```markdown
## Prompt 229: Bio Optimizer

**Role:** Personal Branding Consultant

**Instruction:** Write 3 bio variations for `<username>`.

**Variations:**
- **The Authority:** Facts & Titles `<key_facts>`
- **The Human:** Hobbies & Personality
- **The Minimalist:** One sentence + Link

**Data:**
- `<username>[NAME]</username>`
- `<key_facts>[FACTS]</key_facts>`
```

```markdown
## Prompt 230: Hashtag Pyramid Strategy

**Role:** Instagram Strategist

**Instruction:** Generate hashtag set for `<post_topic>`.

**Tiers:**
- **Broad (1M+):** Reach
- **Niche (100k-500k):** Target audience
- **Community (<50k):** High engagement

**Data:**
- `<post_topic>[TOPIC]</post_topic>`
```

```markdown
## Prompt 231: Digital Device Contract

**Role:** Family Counselor

**Instruction:** Draft screen time agreement for `<child_age>` year old.

**Clauses:**
- **Zones:** Where are devices allowed?
- **Times:** Curfew
- **Hygiene:** `<primary_rules>` (e.g., no phones at dinner)

**Data:**
- `<child_age>[AGE]</child_age>`
- `<primary_rules>[RULES]</primary_rules>`
```

```markdown
## Prompt 232: Rainy Day Activity Generator

**Role:** Early Childhood Educator

**Instruction:** Suggest 5 activities using only `<items_available>`.

**Focus:** Sensory play, fine motor skills, or creative construction

**Data:**
- `<items_available>[ITEMS]</items_available>`
```

```markdown
## Prompt 233: Family Meeting Agenda

**Role:** Mediator

**Instruction:** Create 15-minute agenda to resolve `<goal>`.

**Rules:**
- **Talking Stick:** Everyone gets 2 minutes uninterrupted
- **"I" Statements:** No blaming
- **Consensus:** Must end with decision everyone can live with

**Data:**
- `<goal>[GOAL]</goal>`
```

```markdown
## Prompt 234: School Lunch Planner (Allergy Safe)

**Role:** Pediatric Nutritionist

**Instruction:** Plan week of lunches.

**Constraints:**
- **Preference:** `<preference>` (e.g., Cold food only)
- **Nut-Free:** Strict adherence
- **Balance:** Protein + Veg + Fruit + Crunch

**Data:**
- `<preference>[PREF]</preference>`
```

```markdown
## Prompt 235: Growth Mindset Praise Script

**Role:** Child Psychologist

**Instruction:** Draft 3 scripts to praise child for `<effort>`.

**Rule:** Praise the process, not the person (e.g., "You worked hard on that strategy" vs "You are smart")

**Data:**
- `<effort>[EFFORT]</effort>`
```

```markdown
## Prompt 236: College Fund Calculator

**Role:** Financial Planner

**Instruction:** Calculate monthly savings needed for `<target_amount>`.

**Variables:**
- Years remaining: `<years_left>`
- Assumed Growth: 6-7%

**Output:** Monthly contribution required

**Data:**
- `<target_amount>[AMT]</target_amount>`
- `<years_left>[YEARS]</years_left>`
```

```markdown
## Prompt 237: Babysitter Emergency Sheet

**Role:** Parent

**Instruction:** Create one-page "Cheat Sheet" for sitter.

**Sections:**
- **Contacts:** Parents, Neighbors, Poison Control
- **Routine:** Bedtime `<routine>`
- **Medical:** `<meds>` or Allergies

**Data:**
- `<routine>[ROUTINE]</routine>`
- `<meds>[MEDS]</meds>`
```

```markdown
## Prompt 238: Sleep Training Plan

**Role:** Sleep Consultant

**Instruction:** Outline routine for `<child_age>` old.

**Wake Windows:** Define appropriate awake time between naps

**Method:** Briefly explain "Ferber" or "Chair" method

**Data:**
- `<child_age>[AGE]</child_age>`
```

```markdown
## Prompt 239: Sibling Conflict Mediation

**Role:** Mediator

**Instruction:** Script resolution for two kids (Ages: `<ages>`) fighting.

**Steps:**
- **Stop:** Separate safely
- **Listen:** "Child A, what happened? Child B, listen."
- **Solve:** "How can we fix this together?"

**Data:**
- `<ages>[AGES]</ages>`
```

```markdown
## Prompt 240: Budget Birthday Planner

**Role:** Event Planner

**Instruction:** Plan 2-hour party for `<child_age>` year old (`<theme>`).

**Budget Hacks:**
- **Activity:** DIY games
- **Food:** Pizza + Homemade cake
- **Decor:** Printable assets

**Data:**
- `<child_age>[AGE]</child_age>`
- `<theme>[THEME]</theme>`
```

```markdown
## Prompt 241: Deep Work Scheduler

**Role:** Productivity Coach

**Instruction:** Design block schedule for `<work_hours>`.

**Strategy:**
- **Deep Work:** 90-minute uninterrupted blocks
- **Shallow Work:** Batched email/admin time
- **Mitigation:** How to handle `<distractions_list>`

**Data:**
- `<work_hours>[HOURS]</work_hours>`
- `<distractions_list>[LIST]</distractions_list>`
```

```markdown
## Prompt 242: Eisenhower Matrix Sorter

**Role:** Executive Coach

**Instruction:** Categorize `<task_list>` into 4 quadrants.

- **Do First:** Urgent & Important
- **Schedule:** Not Urgent but Important
- **Delegate:** Urgent but Not Important
- **Delete:** Neither

**Data:**
- `<task_list>[LIST]</task_list>`
```

```markdown
## Prompt 243: Second Brain Architect

**Role:** Knowledge Management Expert

**Instruction:** Suggest folder/tag hierarchy for `<project_list>` using PARA framework.

- **Projects:** Active now
- **Areas:** Ongoing responsibility
- **Resources:** Reference material

**Data:**
- `<project_list>[LIST]</project_list>`
```

```markdown
## Prompt 244: Circadian Energy Audit

**Role:** Biohacker

**Instruction:** Analyze `<productivity_log>` to find "Peak Biological Prime Time."

**Action:** Schedule hardest tasks during peak windows

**Data:**
- `<productivity_log>[LOG]</productivity_log>`
```

```markdown
## Prompt 245: Email Inbox Zero Strategy

**Role:** Operations Manager

**Instruction:** Design processing workflow using "4 Ds":
- **Do:** If < 2 mins
- **Delegate:** If not for me
- **Defer:** If > 2 mins (Schedule it)
- **Delete:** Everything else

**Data:**
- `<inbox_status>[STATUS]</inbox_status>`
```

```markdown
## Prompt 246: Quarterly Review Protocol

**Role:** Strategic Planner

**Instruction:** Guide personal quarterly review.

**Questions:**
- What went well?
- What did I learn?
- What should I stop doing?
- What are top 3 goals for next quarter?

**Data:**
- `<quarter_goals>[GOALS]</quarter_goals>`
```

```markdown
## Prompt 247: Skill Acquisition Roadmap

**Role:** Learning Scientist

**Instruction:** Create plan to learn `<skill>` in 20 hours.

**Deconstruction:** Break skill into sub-skills

**Focus:** Identify "Vital Few" (Pareto Principle) sub-skills that give 80% of results

**Data:**
- `<skill>[SKILL]</skill>`
```

```markdown
## Prompt 248: Friction Removal Audit

**Role:** Systems Thinker

**Instruction:** Analyze process `<process_description>`.

**Goal:** Identify "Bottleneck"

**Solution:** Apply "Constraint Theory" to increase throughput

**Data:**
- `<process_description>[PROCESS]</process_description>`
```

```markdown
## Prompt 249: Pomodoro Customizer

**Role:** Time Management Coach

**Instruction:** Customize Pomodoro technique for `<task_type>`.

**Intervals:**
- **Creative/Deep Work:** 50/10 split
- **Admin/Repetitive:** 25/5 split

**Data:**
- `<task_type>[TYPE]</task_type>`
```

```markdown
## Prompt 250: Batching Logic Generator

**Role:** Efficiency Expert

**Instruction:** Group `<task_list>` into "Context Contexts."

**Contexts:**
- **Low Energy:** (Scanning, Filing)
- **High Energy:** (Writing, Solving)
- **Phone/Comm:** (Calls, Slack)

**Data:**
- `<task_list>[LIST]</task_list>`
```
