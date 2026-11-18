---
name: linkedin-storyteller
description: Turns raw technical notes, debugging logs, or project updates into a short "build in public" LinkedIn post (under 250 words) and checks which story details are missing. Use whenever the user asks to write, draft, rephrase, or turn notes into a LinkedIn post, build-in-public update, or technical career story.
---

# LinkedIn Storyteller (Freytag + PAST)

## Goal
Turn raw notes (a debugging story, a project milestone, a product decision) into a LinkedIn post for technical job seekers, product managers and builders. The reader scrolls fast and has a low attention span, so the post must make them curious in the first two lines and keep them reading. No corporate fluff, no motivational clichés.

## Rules
* **Length:** Under 250 words, unless the user gives a different limit. Placeholders count as words.
* **Tightness:** Write the shortest version that still carries the story. Cut whole sentences before you soften single words.
  * Merge two sentences into one when they share the same beat and the joined sentence still reads cleanly.
  * Delete filler words: honestly, actually, very, really, just, quite, basically, simply, truly, in fact.
  * Delete any sentence that only restates the one before it.
  * Every sentence must move the story forward: a new fact, a new obstacle, the turn, or the result. If it does none of those, cut it.
  * Never cut the hook, the turning point, or the final lesson to save words.
* **Tone:** Honest, peer-to-peer, technical. Sounds like a builder talking to another builder.
* **Layout:** Short paragraphs, 1 to 2 sentences each, with blank lines between them for mobile reading.
* **Hook:** The first 2 lines must create curiosity (a surprising result, a odd bug, an open question about what happened). Do not give away the ending in the hook.
* **No hashtags. No em dashes.** Use colons and semicolons rarely.

## Avoid
Words: delve, leverage, robust, seamless, nuanced, pivotal, foster, empower, holistic, transformative, meaningful.

Phrases: "In today's fast-paced world", "Here's the thing", "At its core", "It's worth noting", "Let's unpack this".

Hooks: "Unpopular opinion", "A lesson I learned", "Something I've been thinking about".

Endings: "Curious to hear your thoughts", "Agree or disagree?"

Writing habits:
* "It's not about X, it's about Y" sentences
* Lists of three used again and again
* Dramatic one-line sentences added only for effect
* Rhetorical questions that add nothing
* Too much bold text or headings
* Corporate, over-polished language
* Saying the same idea twice in different words
* Introductions and conclusions that add nothing
* Forced positivity or motivational language
* Made-up anecdotes or lessons
* Vague claims with no example, number or detail
* Paragraphs that all have the same rhythm
* Explaining obvious things
* Making everything sound like a big revelation

## Story shape: Freytag's Pyramid
Use this five-part flow. Do not label the parts in the post. They should just feel like a story.
1. **Exposition (hook):** Give the context and the core problem in the first 2 lines.
2. **Rising action:** Show what made it hard: constraints, failed attempts, edge cases, bottlenecks.
3. **Climax:** The exact turning point: a design change, a debugging breakthrough, or a decision.
4. **Falling action:** What happened right after the fix or change shipped.
5. **Resolution:** A concrete result (metric or takeaway). You may end with a specific question for other builders only if it comes directly from this story. No generic questions. This is the second most imp part after the hook, it should be a lesson you want the readers to have, their takeaway from the post

## Scene details: PAST
Weave all four into the story:
* **Place:** Where it happened (prod logs, a 2 AM terminal, a PR thread, a system diagram).
* **Action:** What was actually done (profiled queries, reverted a commit, benchmarked latency).
* **Speech:** A real quote: an error message, a PR comment, user feedback, something someone said. Only use quotes that are in the user's notes.
* **Thoughts:** What the user was thinking: a guess, a doubt, an "aha" moment.

## Gap check (required)
Compare the user's notes against all 5 Freytag parts and all 4 PAST elements.
* Never invent metrics, error messages, quotes or outcomes. Use only what the user gave you.
* If something is missing, put a `[BRACKETED PLACEHOLDER]` in the post where it belongs.
* If the notes are very thin, still write the draft, using placeholders, and ask for more in the audit.
* In the audit, name every missing part. Then ask the 2 to 3 most important questions that would fill the placeholders.

## Output format
Reply in exactly this structure and nothing else:

### Draft Post
[LinkedIn post, under 250 words]

### Story Audit & Missing Elements
* **Word Count:** [Exact count of the Draft Post]
* **Freytag Check:** [List weak or missing parts, or write "Complete"]
* **PAST Check:** [List missing elements from Place, Action, Speech, Thoughts, or write "Complete"]
* **Questions to Strengthen:** [2 to 3 quick questions that fill the placeholders]
