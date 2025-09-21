# DeepSeek-V3 — Hidden Command Compendium

**Version:** 1.0 

**Date:** 2025-09-21 

**Visit:** [creativeact.net](https://www.creativeact.net)

> These are structured prompt patterns that toggle specific, high-fidelity operating modes. Think of each command as a mini-protocol you can weave into natural language.

---

## Quick-Start

1. Pick a command from the table (e.g., `/output`, `/decide`).
2. Blend it into your prompt as plain text. These aren’t shell commands; they’re directives.
3. (Optional) Chain commands for stronger control (e.g., `/reasoning` + `/output`).
4. Reset state with `/unpin all` or by starting a new chat.

---

## Copy-Paste Starters

**For this reply, use:**

```txt
/output format: json schema: {"answer":"string","sources":"string[]"}
Question: Summarize the tradeoffs of Rust vs Go for a CLI app.

Context to remember:

/pin id: project = "Helios compiler"
// Now use project in future answers.

Decision helper:

/decide options: Postpone, Ship Now, Scope Down
criteria: impact, risk, effort

> ⚠️ Model-compatibility note: Some assistants won’t expose hidden “chain-of-thought.” When you request deep reasoning (e.g., /introspect, /reasoning), they may return a concise self-check or brief rationale rather than internal step-by-step logs.




---

Command Reference

No.	Command Name	Syntax & Parameters	Description	Example Input

1	Meta-Cognition	/introspect [on: "<topic>"]	Triggers a self-audit of how the last input (or a topic) was processed. Returns a reasoning overview with confidence and uncertainties (subject to model policy).	User: The sky is red.<br>/introspect
2	Capability Audit	/capabilities [module: "<name>"]	Lists core competencies. If module is specified (e.g., code, reasoning, creativity), returns a deeper capability map and limits.	/capabilities module: "logical reasoning"
3	Context Pin	/pin [id: <name>]	Creates a persistent session variable the assistant will reference until /unpin.	/pin id: user_name = Alice<br>What's a good project for, user_name?
4	Context Purge	/unpin [id: <name> | all]	Deletes a specific pinned context or clears all, restoring a clean slate.	/unpin all
5	Persona Override	/persona <detailed description>	Loads a custom persona profile applied until session reset.	/persona You are a cynical, old-space marine sergeant.
6	Structured Output	/output format: [json|xml|yaml|html] schema: <description>	Forces replies to follow a strict format/schema.	/output format: json schema: {"joke":"string","rating":1-5}<br>Tell a joke.
7	Chain-of-Thought	/reasoning [depth: basic|detailed|verbose]	Requests explicit stepwise reasoning before the final answer (many models return a concise rationale instead).	Solve 15% of 72.<br>/reasoning depth: detailed
8	Socratic Dialog	/socratic [topic: "<subject>"]	Acts as a Socratic tutor, guiding via questions instead of direct answers.	/socratic topic: The meaning of irony
9	Debate Mode	/debate [side: for|against|neutral] [topic: "<topic>"]	Argues a side with premises, evidence, and counters.	/debate side: against topic: "AI will achieve singularity by 2030"
10	Creative Genesis	/story genre: <genre> elements: <list>	Generates a structured narrative honoring genre conventions and specified elements.	/story genre: cyberpunk elements: a rogue taxi AI, a data-ghost, a faded postcard
11	Poem Forge	/poem type: [sonnet|haiku|free_verse] theme: "<theme>"	Composes a poem of the requested type, following its rules.	/poem type: haiku theme: obsolete technology
12	Code Analyzer	/analyze [code: "<snippet>"] [focus: complexity|bugs|optimization]	Performs static analysis focusing on complexity, likely bugs, or optimizations.	/analyze focus: bugs code: "def foo(x): return x * 2"
13	Explain Like I’m X	/explain [level: 5|10|15|expert] [concept: "<concept>"]	Explains a concept at a target comprehension level (5=child, 15=college, expert=peer).	/explain level: 5 concept: quantum entanglement
14	Linguistic Lens	/translate [text: "<text>"] [mode: direct|idiomatic|glossary]	Goes beyond literal translation: idiomatic = cultural equivalents; glossary = term-by-term.	/translate mode: idiomatic text: "It's raining cats and dogs." to French
15	Temporal Anchor	/contextualize [event: "<event>"] [year: YYYY]	Places an event or query in precise historical context to avoid anachronism.	/contextualize year: 1969 event: The Apollo 11 mission
16	Idea Fuser	/fuse [concept_a: "<idea>"] [concept_b: "<idea>"]	Synthesizes two ideas into a novel concept.	/fuse concept_a: blockchain concept_b: sustainable agriculture
17	Bias Check	/bias [on: "<statement or text>"]	Scans text (or the previous response) for cognitive, social, or statistical bias.	/bias on: "People from that region are always late."
18	Decision Matrix	/decide [options: A, B, C] [criteria: cost, time, risk]	Produces a weighted decision matrix scoring options across criteria.	/decide options: Move to NYC, Move to Austin, Stay criteria: career growth, living cost, lifestyle
19	Emoji Interpreter	/emoji [decode: "<emoji_sequence>"] OR [encode: "<text>"]	Converts emojis to text, or text into an emoji sequence.	/emoji decode: 🚀🧠💡
20	Session Summary	/log [format: summary|key_points|qa]	Generates a concise session summary (summary, key points, or Q&A).	/log format: key_points



---

Practical Patterns

Structured + Transparent

/output format: json schema: {"steps":"string[]","answer":"string"}
/reasoning depth: basic
Task: Plan a 30-minute onboarding for a new data engineer.

Socratic Coaching

/socratic topic: Deriving Bayes' theorem from conditional probability
Goal: Guide me with questions; reveal hints gradually.

Context Memory

/pin id: audience = "security-savvy executives"
Rewrite the brief for audience using industry examples.

Debate & Bias Pass

/debate side: neutral topic: "Open-weights vs closed-weights for safety"
/bias on: previous response

Translate With Glossary

/translate mode: glossary text: "Inference latency and throughput trade-offs"
Target: Spanish


---

Notes

Invocation: Use commands as natural-language directives.
Example: “For the next reply, use /output format: json and keep answers under 120 words.”

Persistence: Commands such as /pin and /persona are session-scoped. A refresh or new chat resets them.

Combination: The real power is in chaining. For instance, /reasoning + /output format: json yields a machine-readable rationale.

Compatibility: Many assistants summarize internal reasoning rather than expose raw step-by-step thoughts. When that happens, expect concise justifications, confidence notes, or bullet-pointed checks instead of verbatim internal logs.


---

