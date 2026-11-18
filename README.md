# LinkedIn Storyteller

A Claude skill that turns your raw notes into a short "build in public" LinkedIn post.

Give it a debugging story, a project milestone, or a product decision. It writes a post under 250 words that is easy to read on mobile and makes people curious in the first two lines.

## Who it is for

Product managers, builders and job seekers who share their work on LinkedIn to network, build credibility, and get noticed by seniors and recruiters.

## What it does

- Writes a post using Freytag's Pyramid (hook, rising action, climax, falling action, resolution)
- Adds scene details using PAST (Place, Action, Speech, Thoughts)
- Never invents metrics, quotes or error messages. Missing details show up as `[BRACKETED PLACEHOLDERS]`
- Avoids AI-sounding words, hashtags and em dashes
- Gives you a short audit with the word count, what is missing, and 2 to 3 questions to fill the gaps

## How to use

1. Download or clone this repo.
2. Add the skill to Claude (Settings > Capabilities > Skills), or place the folder in your skills directory if you use Claude Code.
3. Paste your raw notes and ask Claude to turn them into a LinkedIn post.

## Example

**Input:** "Our onboarding drop-off was 40%. Looked at session recordings, found users got stuck on step 3. Removed it. Drop-off went to 28%."

**Output:** a draft post, plus a list of what is missing (for example, a quote from a user, or what you were thinking when you found the problem).

## Files

- `SKILL.md`: the skill itself

## License

MIT
