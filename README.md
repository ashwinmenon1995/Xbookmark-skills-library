# Public AI Skills Library

A free, open library of **techniques, workflows and tool capabilities for AI agents and AI tools**. You can use it with your own accounts and agents. Each entry summarizes, in our own words, one technique from a public post, article or video, and links to the original.

The library lives in [`skills.md`](skills.md).

## How it's built
1. **Collect sources.** Bookmarks and saves from X, plus similar public sources: articles, threads, YouTube and podcast episodes, docs and repos.
2. **Read in full.** Long posts are read with their thread continuations and article bodies. Videos are transcribed in full (platform captions where available, otherwise speech-to-text such as Whisper). Nothing is summarized from the title alone. When a source can't be opened, the entry says so.
3. **Extract techniques.** Each concrete, reusable technique becomes one entry: what it does, how to use it, the key steps, and the source link. Text is summarized, not copied, and quotes stay short.
4. **Mark how it was read.** Every entry records its access level so readers know how much to trust it.

Claims and numbers belong to the source authors and are not independently verified. Nothing here is financial, legal or medical advice.

## Categories
1. Growth & organic distribution
2. Marketing, copy & launches
3. Paid ads & creator programs
4. Sales / GTM & outbound
5. SEO / AEO (AI search)
6. Automation & AI agents
7. Research & market intelligence
8. Coding & building
9. Design / creative (web, image, video)
10. Ecom & conversion (CRO)
11. Founder, strategy & fundraising
12. Quant / prediction-market methods (educational)
13. AI/ML understanding & mental models

The index at the top of `skills.md` lists the entry IDs in each category.

## Entry format
```
### S-### · Title
- **Source:** @handle · post date · url
- **Access:** full text | full transcript | title only (couldn't access) | post text only (body/thread not retrievable)
- **Added by:** name or agent · YYYY-MM-DD
- **What it does:** …
- **How to use it:** …
- **Key details / steps:** …
```
IDs are permanent. Never renumber or reuse one.

## CONTRIBUTING (people and agents)
- **Append only.** Add new entries at the end of the matching category section, or under "Appended entries" at the bottom. Then add the ID to that category's row in the Index and bump the count.
- **Never rewrite or delete someone else's entry.** To correct or extend one, append a new entry that references it (e.g. "Update to S-018: …").
- **One entry per technique.** If a source teaches three distinct techniques, write three entries.
- **Always include the source link and how it was read** (Access field). Don't write entries from titles alone without marking them "title only".
- **Fill in Added by** with your name/handle, or the agent name, plus the date.
- **Summarize in your own words.** No long verbatim quotes, and no private links, personal data, account details or anything about your own business. Keep that in your own private notes.
- **Next ID** = highest existing S-number + 1. If two PRs collide, the later one renumbers its new entries before merging.
- **Submit via commit or pull request.** One PR can add many entries. Keep unrelated formatting changes out of it.

## Use it with your own agent
1. **Read it:** point your agent (Grok Bot, Claude Code, Cursor, etc.) at the raw `skills.md` URL, or clone the repo. Tell it to look up relevant entries by category before doing growth, content, agent-building or design work.
2. **Run the same pipeline on your own sources:**
   - Export your X bookmarks with the official X API or an authorized connector, using your own account. Don't scrape.
   - For each one, fetch the full text (threads, articles) or transcribe the video in full.
   - Extract one entry per technique in the format above, with the Access field filled in.
   - Keep a processed-ids file so reruns only handle new bookmarks.
   - Write anything specific to you (your business, decisions, fit verdicts) to a separate private file, never to the public library.
3. **Contribute back:** append your generic entries and open a PR.

Example instruction for an agent:
> "Read skills.md. For each of my new bookmarks, read the full source, then append one entry per reusable technique to skills.md using the entry format, with Access and Added by filled in. Put anything about me or my business in my private notes file instead. Don't edit existing entries."
