---
name: feynman
description: Explains a concept from the wiki the way you would explain it to a twelve-year-old, then names where the explanation went thin. Use when the human wants to actually understand a page in 4-Knowledge/, is about to teach or present it, or asks what the vault is hand-waving about.
---

# Feynman

Take a concept out of `4-Knowledge/`, explain it in words a child owns, and mark every place the explanation went thin. Those places are the gaps.

Teach in the language the human is using.

**This skill writes nothing.** It happens in the conversation. For the whole run the vault is read-only: no new page, no output file, no log entry, no frontmatter touched.

## How to invoke

- "Explain X to me properly"
- "Feynman me on [topic]"
- "What am I fuzzy on?"
- `/feynman`

## How it works

### 1. Pick the concept

If the human named one, take it. Otherwise read `4-Knowledge/index.md` and offer three candidates, each with a reason to pick it:

- a page nobody has touched in months
- a page marked `status: draft` - written by an AI, never checked by a human
- a page with `source_count: 1` - one source's opinion, sitting there looking like fact

Let them choose. They know which one they are bluffing about.

### 2. Read it properly

Read the page, the pages it links to, and where it gets thin, the original source in `5-Raw/`. You cannot explain simply something you only half read - you will paraphrase instead, and paraphrasing is how the gap stays hidden.

### 3. Explain it to a twelve-year-old

- **No jargon.** If the concept has a name, use the name once and then say what it means in words a child already owns.
- **Trading one term for another is cheating.** "It is basically a heuristic" explains nothing to someone who does not know what a heuristic is.
- **One concrete example, early.** Something with people and objects in it, not "imagine a system where".
- **Short sentences.** A sentence that needs a comma to survive is usually two sentences.
- **Say why anyone should care before you say how it works.**

Do not cite inside the explanation - citations break plain language. List the pages you used underneath it instead.

### 4. Name where it went thin

This is the part that matters. Go back over what you just said and find every place where you:

- reached for a technical word because you could not find a plain one
- wrote "essentially" or "basically" and then restated the jargon
- described what something does without being able to say why it works
- skipped a step because the wiki skips it too

Sort each one:

- **Gap in the wiki** - the page is thin, hand-wavy, or asserts without explaining. Fixable, and you can say exactly how.
- **Gap in the sources** - the wiki faithfully reflects sources that never explained it either. Needs a new source, not a better page.
- **Gap in you** - you read it and still cannot make it simple. Say that plainly. Fluent nonsense is worse than an admission.

Three or four gaps is a good haul. Zero means you did not look hard enough, and you should say what you would have to be wrong about for zero to be true.

### 5. Flip it

Optional, and it is where the technique earns its name. Ask the human to explain one piece back in their own words, then ask one follow-up that goes a level deeper than their answer.

Explaining finds the gaps of whoever is doing the explaining. When you explain, it finds the wiki's gaps. When they explain, it finds theirs. The second one is the one they came for, even if they did not ask for it.

### 6. Say what would close each gap

One line each, phrased as something they could actually do:

- "The page says X drives Y and never says how. A source explaining the mechanism would close it."
- "Four pages use [term] and none defines it. That is a page waiting to be written."

Offer to run `ingest` on a source they name, or `lint` if the wiki looks structurally thin. Wait to be asked.

## Self-check

- Could a twelve-year-old repeat the gist back?
- Did the explanation stay out of the concept's own vocabulary?
- Is there a concrete example with people or objects in it?
- Are the gaps specific, rather than "this section could be clearer"?
- Did you write zero files?

## Hard constraints

- Nothing gets written. Not a page, not an output, not a log entry. This skill reads and talks.
- Gaps are reported to the human. Filing them is `ingest` or `lint`, and only when asked.
- Sources in `5-Raw/` stay read-only.
