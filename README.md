# A Second Brain for Product Builders

A vault your AI reads, writes and maintains. From the team behind [AI Product Heroes](https://aiproductheroes.pl).

Every chat starts from zero. You paste the same context, get a good answer, close the tab, and the thinking is gone. Next week you ask a related question and do it all again. The tool got smarter; your setup did not.

Super Brain is a folder instead of a conversation. Sources compile into a linked wiki. Questions get answered from that wiki and saved, so asking makes it better instead of just using it up. Projects carry enough context that an agent can join one cold. Your profile lives in a file, not a system prompt, so it moves with you between tools and jobs.

It is an adaptation of [Andrej Karpathy's LLM knowledge base method](https://x.com/karpathy/status/2039805659525644595), with the parts a working product builder actually needs bolted on.

## Setup

```
git clone https://github.com/superhero-tech/super-brain
cd super-brain
claude
```

Then run `/second-brain-setup` and answer the questions. That is the whole install.

Obsidian is the recommended window onto it (`Open folder as vault`), but nothing depends on it. [SETUP.md](SETUP.md) covers the other routes: Claude Cowork for non-developers, OpenCode with a ChatGPT subscription or a free model, and any AI-enabled IDE.

## Why this exists

We have run this method on our own work for a year and taught it to people who then went and broke it in interesting ways. The same four failures keep showing up.

**Notes accumulate, knowledge does not.** Most systems file a summary per source and call it a knowledge base. `ingest` maps everything a source touches, writes one page per concept, and updates every other page that source has something to say about, with links in both directions. One article moves five pages or it tells you why it did not.

**Good answers evaporate into the terminal.** You ask a sharp question, get a synthesis nobody has written down before, and lose it when the tab closes. `query` saves every substantial answer with its citations and a section naming what the wiki could not answer, then offers to file the new thinking back in.

**Wikis rot quietly.** A subtly wrong page gets built on until five pages agree on the same error. `lint` runs monthly, sorts findings into errors, warnings and notes, and ranks what to fix first. It reports; you decide.

**Projects you cannot pick up cold.** A brief tells you what a project was supposed to be. `project-update` keeps the log that tells you what it became, and refreshes the index so the next session starts from the truth.

## The skills

Five workflows, one skill each, plus setup, video capture and a way to find out whether you actually understand what you have collected. They trigger on their own when the conversation calls for them - say "process what I dropped in the inbox" and `ingest` shows up - or you invoke them directly with `/query`. Claude reads them from `.claude/skills/`, Codex and ChatGPT from `.agents/skills/`; both are published from `7-Skills/`, so they work on a fresh clone without setup.

| Skill | What it does |
|---|---|
| **`ingest`** | Turns a source in `2-Inbox/` into wiki. Lists everything the source touches and checks that reading with you before writing, then updates every page it touches with links in both directions. A substantial source moves five pages, or it says why it did not. |
| **`query`** | Answers from the wiki with `[source: ...]` citations, saves the answer to `9-Outputs/` with a section naming what the wiki could not answer, and offers to file new synthesis back as a page. |
| **`lint`** | Monthly health check. Ten checks sorted into errors, warnings and notes: contradictions, uncited claims, orphans, stale frontmatter, people who became hubs without a page. Writes a ranked report and stops, because repair is a separate decision. |
| **`project-start`** | Opens a project through an interview that pushes back once per section. "Everyone" is not a segment and "more engagement" is not an outcome. "I do not know" is a valid answer that becomes an open question. |
| **`project-update`** | Turns what happened into an artefact, a log entry and a fresh index row. The last two decay first because they produce nothing visible, and a stale index means the next session starts from a false picture. |
| **`second-brain-setup`** | Writes your profile into `8-System/about.md`, from a pasted assessment (Gallup, DISC, MBTI) or a short interview. Re-run it after a role change and it updates only what moved. |
| **`youtube`** | Turns a video into a source note with metadata, key ideas and quotes, then hands it to `ingest`. Wants `yt-dlp`; without it, it asks you to paste the transcript and carries on. |
| **`feynman`** | Explains a page in words a twelve-year-old owns, then names every place the explanation went thin, sorted into the wiki's fault, the sources' fault and its own. Saves the session to `9-Outputs/` so you can see what you have been studying. Edits no wiki page. |

The one to try first: drop three articles on one topic into `2-Inbox/`, run `ingest` on each, then ask `query` something none of them answers on its own.

## What it does badly

Read [8-System/limits.md](8-System/limits.md) before you trust it on anything expensive. Error compounding is real, a wiki that looks authoritative gets checked less than it should, and the index-first approach has a ceiling around a hundred pages. We would rather you knew that from us.

## Who's behind this

We're Wojtek and Piotr, founders of [Superhero.tech](https://superhero.tech) and [AI Product Heroes](https://aiproductheroes.pl), a course where product people learn to build real products in the AI era. This is the vault we use on our own work, not a demo.

If this is your kind of thing, the [newsletter](https://newsletter.superhero.tech) is where we publish the rest.
