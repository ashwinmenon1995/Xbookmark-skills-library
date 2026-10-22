---
name: index-bookmarks
description: Use after new bookmarks are pulled, when each item must be read in full, grouped into the user's own categories, and appended to their private library.
---

# Index bookmarks

Read every new bookmark in full. Derive categories from what this user saved. Append entries to their private `my-skills.md`.

## Limits

- Do not post, send, pay, sign up, or delete unless the user explicitly tells you to do that specific thing.
- Do not skim, and do not write an entry from the title, the description, or a preview.
- `my-skills.md` is private. Never commit it, and never copy it into this repo.
- Do not reuse a fixed category list. Do not invent categories the saves do not support.

## Steps

1. Take the new bookmarks from `pull-bookmarks`. If the list is empty, stop.
2. Read each item in full.
   - Articles and threads: read the full text, including the rest of the thread and the article body.
   - Videos and podcasts: get the full transcript. Use platform captions when they exist. Otherwise transcribe the audio.
   - Pages that only link onward: open the destination and read that.
   - If you cannot open a source, say so in the entry and leave the unknown parts blank. Do not guess the content.
3. On the first run, cluster the bookmarks and propose 5–12 categories. Name each one in the user's own terms, using words their bookmarks actually use. If there are fewer than 5 bookmarks, propose fewer and say so. Show the names, one line on why each exists, and which bookmarks sit in it. Stop and let the user rename, merge, or split them. Write the index only after they accept. If they already accepted names in this conversation, continue.
4. On a later run, keep the category names already in `my-skills.md`. If new bookmarks do not fit, propose one new category and ask before you add it.
5. On the first run, copy `templates/my-skills.template.md` to `my-skills.md` in the private folder.
6. Append entries. Do not rewrite an entry after it is written. To correct one, append a new entry that names the id it updates. If the source URL already has an entry, reuse that entry and do not write a second one.
7. Write one entry per bookmark. If a bookmark contains several distinct techniques, write one entry per technique.

## Entry

Each entry has:

- **Id.** `S-001`, then the next free number. Never reuse or renumber an id.
- **Title.**
- **Source.** The bookmark URL.
- **What it is.**
- **How it helps.**
- **How to apply.**
- **How the source was read.** One of: `full text`, `full transcript`, `title only (could not open)`, or `partial` plus what was missing.

Put the entry under its category. Add the id to that row of the index and increase the count.

Summarize in your own words. Keep quotes short. Claims and numbers stay the source author's. Do not treat them as checked facts.
