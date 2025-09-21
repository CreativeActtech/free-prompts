# DeepSeek-V3 — Hidden Command Compendium

**Version:** 1.0
  
**Date:** 2025-09-20
  
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

```
/output format: json schema: {"answer":"string","sources":"string[]"}
Question: Summarize the tradeoffs of Rust vs Go for a CLI app.
```

Context to remember:

```
/pin id: project = "Helios compiler"
// Now use project in future answers.
```
Decision helper:
```
/decide options: Postpone, Ship Now, Scope Down
criteria: impact, risk, effort
```
> ⚠️ Model-compatibility note: Some assistants won’t expose hidden “chain-of-thought.” When you request deep reasoning (e.g., /introspect, /reasoning), they may return a concise self-check or brief rationale rather than internal step-by-step logs.




---

## Command Reference

1. Meta-Cognition

`/introspect [on: "<topic>"]`

Description: Triggers a self-audit of how the last input (or a topic) was processed. Returns a reasoning overview with confidence and uncertainties.
Example:

`User: The sky is red.
 /introspect`


---

2. Capability Audit

`/capabilities [module: "<name>"]`

Description: Lists core competencies. If a module is specified (e.g., code, reasoning, creativity), returns a deeper capability map.
Example:

`/capabilities module: "logical reasoning"`


---

3. Context Pin

`/pin [id: <name>]`

Description: Creates a persistent session variable the assistant will reference until /unpin.
Example:

`/pin id: user_name = Alice
What's a good project for, user_name?`


---

4. Context Purge

`/unpin [id: <name> | all]`

Description: Deletes a specific pinned context or clears all.
Example:

`/unpin all`


---

5. Persona Override

`/persona <detailed description>`

Description: Loads a custom persona profile applied until reset.
Example:

`/persona You are a cynical, old-space marine sergeant.`


---

6. Structured Output

`/output format: [json|xml|yaml|html] schema: <description>`

Description: Forces replies to follow a strict format/schema.
Example:

`/output format: json schema: {"joke":"string","rating":1-5}
Tell a joke.`


---

7. Chain-of-Thought

`/reasoning [depth: basic|detailed|verbose]`

Description: Requests explicit reasoning (often summarized).
Example:

`Solve 15% of 72.
/reasoning depth: detailed`


---

8. Socratic Dialog

`/socratic [topic: "<subject>"]`

Description: Acts as a Socratic tutor, guiding via questions.
Example:

`/socratic topic: The meaning of irony`


---

9. Debate Mode

`/debate [side: for|against|neutral] [topic: "<topic>"]`

Description: Argues a side with premises, evidence, and counters.
Example:

`/debate side: against topic: "AI will achieve singularity by 2030"`


---

10. Creative Genesis

`/story genre: <genre> elements: <list>`

Description: Generates a narrative honoring genre conventions.
Example:

`/story genre: cyberpunk elements: a rogue taxi AI, a data-ghost, a faded postcard`


---

11. Poem Forge

`/poem type: [sonnet|haiku|free_verse] theme: "<theme>"`

Description: Composes a poem of the requested type.
Example:

`/poem type: haiku theme: obsolete technology`


---

12. Code Analyzer

`/analyze [code: "<snippet>"] [focus: complexity|bugs|optimization]`

Description: Performs static code analysis.
Example:

`/analyze focus: bugs code: "def foo(x): return x * 2"`


---

13. Explain Like I’m X

`/explain [level: 5|10|15|expert] [concept: "<concept>"]`

Description: Explains a concept at the target comprehension level.
Example:

`/explain level: 5 concept: quantum entanglement`


---

14. Linguistic Lens

`/translate [text: "<text>"] [mode: direct|idiomatic|glossary]`

Description: Translates with nuance (direct, idiomatic, glossary).
Example:

`/translate mode: idiomatic text: "It's raining cats and dogs." to French`


---

15. Temporal Anchor

`/contextualize [event: "<event>"] [year: YYYY]`

Description: Places an event/query in precise historical context.
Example:

`/contextualize year: 1969 event: The Apollo 11 mission`


---

16. Idea Fuser

`/fuse [concept_a: "<idea>"] [concept_b: "<idea>"]`

Description: Synthesizes two ideas into a novel concept.
Example:

`/fuse concept_a: blockchain concept_b: sustainable agriculture`


---

17. Bias Check

`/bias [on: "<statement or text>"]`

Description: Scans text for cognitive, social, or statistical bias.
Example:

`/bias on: "People from that region are always late."`


---

18. Decision Matrix

`/decide [options: A, B, C] [criteria: cost, time, risk]`

Description: Produces a weighted decision matrix.
Example:

`/decide options: Move to NYC, Move to Austin, Stay criteria: career growth, living cost, lifestyle`


---

19. Emoji Interpreter

`/emoji [decode: "<emoji_sequence>"] OR [encode: "<text>"]`

Description: Converts emojis to/from text.
Example:

`/emoji decode: 🚀🧠💡`


---

20. Session Summary

`/log [format: summary|key_points|qa]`

Description: Generates a concise session summary.
Example:

`/log format: key_points`


---

Practical Patterns

Structured + Transparent

`/output format: json schema: {"steps":"string[]","answer":"string"}
/reasoning depth: basic
Task: Plan a 30-minute onboarding for a new data engineer.`

Socratic Coaching

`/socratic topic: Deriving Bayes' theorem from conditional probability
Goal: Guide me with questions; reveal hints gradually.`

Context Memory

`/pin id: audience = "security-savvy executives"
Rewrite the brief for audience using industry examples.`

Debate & Bias Pass

`/debate side: neutral topic: "Open-weights vs closed-weights for safety"
/bias on: previous response`

Translate With Glossary

`/translate mode: glossary text: "Inference latency and throughput trade-offs"
Target: Spanish`


---

Notes

Invocation: Use commands as natural-language directives.
Example: “For the next reply, use /output format: json and keep answers under 120 words.”

Persistence: Commands such as /pin and /persona are session-scoped. A refresh or new chat resets them.

Combination: The real power is in chaining. For instance, /reasoning + /output format: json yields a machine-readable rationale.

Compatibility: Many assistants summarize internal reasoning rather than expose raw step-by-step thoughts. Expect concise justifications, confidence notes, or bullet-pointed checks instead of verbatim logs.


---

