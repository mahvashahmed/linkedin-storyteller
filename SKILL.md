---
name: linkedin-storyteller
description: Turns raw technical notes, debugging logs, or project updates into a short "build in public" LinkedIn post (under 250 words) and checks which story details are missing. Use whenever the user asks to write, draft, rephrase, or turn notes into a LinkedIn post, build-in-public update, or technical career story.
---

# LinkedIn Storyteller (Freytag + PAST)

## Goal
Turn raw notes (a debugging story, a project milestone, a product decision) into a LinkedIn post for technical job seekers, product managers and builders. The reader scrolls fast and has a low attention span, so the post must make them curious in the first two lines and keep them reading. No corporate fluff, no motivational clichés.

## Step 1: Pick the post type
Every post is one of two shapes. Decide which one before you draft, because the gap check and the audit differ.

**Story post.** A debugging session, a failure, a milestone, a decision you made. Something happened and then something changed.
* Full Freytag treatment. All five beats and all four PAST elements apply.
* Use the gap check and the `[BRACKETED PLACEHOLDER]` rule as written. A story post is usually missing something, and the placeholder tells you what to go and find.

**Announcement post.** A tool you built, a launch, a lesson you learned, a process change. The point is the thing you made, not a narrative arc.
* Freytag still applies, loosely. The hook is the problem. The turn is what changed your approach. The resolution is the rule or takeaway the reader should walk away with.
* Leave out the rising action and the falling action unless the notes genuinely have them. Do not manufacture them.
* No placeholders. Write around the gaps.
* The audit does not check for missing story beats. It asks only about things that would change the post.

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
* **Match the examples, if there are any.** If this skill folder contains an `examples/` directory, write in the style of those posts: their vocabulary, their sentence rhythm and their level of detail. The examples also show one of each post type. Where an example uses a phrase the Avoid list bans, the example wins, except for asking the reader for comments or suggestions.
* **No hashtags. No em dashes.** Use colons and semicolons rarely.

## Avoid
Words: delve, leverage, robust, seamless, nuanced, pivotal, foster, empower, holistic, transformative, meaningful.

Phrases: "In today's fast-paced world", "Here's the thing", "At its core", "It's worth noting", "Let's unpack this".

Hooks: "Unpopular opinion", "A lesson I learned", "Something I've been thinking about".

Endings: "Curious to hear your thoughts", "Agree or disagree?", asking the reader for comments or suggestions

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
Use this five-part flow for a story post. Do not label the parts in the post. They should just feel like a story.
1. **Exposition (hook):** Give the context and the core problem in the first 2 lines.
2. **Rising action:** Show what made it hard: constraints, failed attempts, edge cases, bottlenecks.
3. **Climax:** The exact turning point: a design change, a debugging breakthrough, or a decision.
4. **Falling action:** What happened right after the fix or change shipped.
5. **Resolution:** A concrete result (metric or takeaway). You may end with a specific question for other builders only if it comes directly from this story. No generic questions. This is the second most imp part after the hook, it should be a lesson you want the readers to have, their takeaway from the post

## Scene details: PAST
Weave all four into a story post:
* **Place:** Where it happened (prod logs, a 2 AM terminal, a PR thread, a system diagram).
* **Action:** What was actually done (profiled queries, reverted a commit, benchmarked latency).
* **Speech:** A real quote: an error message, a PR comment, user feedback, something someone said. Only use quotes that are in the user's notes.
* **Thoughts:** What the user was thinking: a guess, a doubt, an "aha" moment.

## Gap check (required)

**Story post.** Compare the user's notes against all 5 Freytag parts and all 4 PAST elements.
* Never invent metrics, error messages, quotes or outcomes. Use only what the user gave you.
* If something is missing, put a `[BRACKETED PLACEHOLDER]` in the post where it belongs.
* If the notes are very thin, still write the draft, using placeholders, and ask for more in the audit.
* In the audit, name every missing part. Then ask the 2 to 3 most important questions that would fill the placeholders.

**Announcement post.** Do not audit for missing Freytag beats or PAST elements. A good announcement has no rising action and no falling action.
* Still never invent metrics, error messages, quotes or outcomes.
* Write around the gaps. No placeholders in an announcement.
* In the audit, ask only about things that would change the post: a missing reason for a design choice, a missing number, a missing next step.

## Output format
Reply in exactly this structure and nothing else:

### Draft Post
[LinkedIn post, under 250 words]

### Story Audit & Missing Elements
* **Word Count:** [Exact count of the Draft Post]
* **Freytag Check:** [Story post: list weak or missing parts, or write "Complete". Announcement post: write "Not applicable, announcement shape."]
* **PAST Check:** [Story post: list missing elements from Place, Action, Speech, Thoughts, or write "Complete". Announcement post: write "Not applicable, announcement shape."]
* **Questions to Strengthen:** [2 to 3 quick questions that fill the placeholders. For an announcement post, ask only about things that would change the post.]
