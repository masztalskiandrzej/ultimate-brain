---
name: feynman
description: Explains a concept from the wiki the way you would explain it to a twelve-year-old, then names where the explanation went thin. Use when the human wants to actually understand a page in 4-Knowledge/, is about to teach or present it, or asks what the vault is hand-waving about.
---

# Feynman

Take a concept out of `4-Knowledge/`, explain it in words a child owns, and mark every place the explanation went thin. Those places are the gaps.

Teach in the language the human is using.

**This skill reads the wiki and never edits it.** It saves the session to `9-Outputs/` and logs it, so there is a record of what got studied - but it creates no wiki page, changes no existing page, and touches nothing in `5-Raw/`. Learning is not ingesting.

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

Ask the human to explain one piece back in their own words, then ask one follow-up that goes a level deeper than their answer. Skip it only if they say so.

Explaining finds the gaps of whoever is doing the explaining. When you explain, it finds the wiki's gaps. When they explain, it finds theirs. The second one is what they came for, even if they did not ask for it. Whatever they say back goes into the record - that is the part worth rereading in six months.

### 6. Save the session

Write `9-Outputs/[YYYY-MM-DD]-feynman-[concept-slug].md`:

```markdown
---
concept: [Page Name]
date: [YYYY-MM-DD]
pages: [wiki pages read]
gaps: [how many]
---

# Feynman: [Concept]

## The explanation
[what you said, in the plain language you said it]

## Where it went thin
**Wiki:** [gaps in the pages]
**Sources:** [gaps the sources never covered]
**Mine:** [what you could not make simple]

## What would close them
- [one line per gap, phrased as something they could do]

## What they said back
[their explanation from step 5, and where the follow-up landed. Skip the
section if step 5 did not run.]
```

Then append to `4-Knowledge/log.md`:

```
## [YYYY-MM-DD] query | feynman: [Concept]
Pages read: Page A, Page B
Output: 9-Outputs/YYYY-MM-DD-feynman-slug.md
Gaps: x wiki, y sources, z mine
```

It is a `query` action because that is what it is: reading the wiki and producing something from it. The `feynman:` marker makes the study sessions easy to pick out later.

### 7. Offer, do not act

Gaps are worth fixing, but fixing them is a different job. Offer to run `ingest` on a source they name, or `lint` if the wiki looks structurally thin. Wait to be asked.

## Self-check

- Could a twelve-year-old repeat the gist back?
- Did the explanation stay out of the concept's own vocabulary?
- Is there a concrete example with people or objects in it?
- Are the gaps specific, rather than "this section could be clearer"?
- Is the session in `9-Outputs/` and the entry in `4-Knowledge/log.md`?

## Hard constraints

- No wiki page is created or edited. `4-Knowledge/log.md` is the one file in that folder this skill appends to.
- `5-Raw/` is read-only, as always. Reading a source to understand it is not ingesting it.
- Filing a gap into the wiki is `ingest` or `lint`, and only when asked.
