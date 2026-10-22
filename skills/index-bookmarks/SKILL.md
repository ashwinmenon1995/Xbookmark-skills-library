---
name: index-bookmarks
description: Use after new bookmarks are pulled, when each item must be read in full, grouped into the user's own categories, and appended to their private library.
---

# Index bookmarks

Read every new bookmark. Derive categories from what this user saved. Append entries to their private `my-skills.md`.

## Limits

- Do not post, send, pay, sign up, or delete unless the user explicitly tells you to do that specific thing.
- Do not skim, and do not write an entry from a title, a description, show notes, or a preview.
- Do not guess missing text. Do not bypass a login or a paywall. Do not scrape.
- `my-skills.md` stays in the private folder. Never commit it.
- Do not reuse a fixed category list, including the sample category in `examples/`. Do not invent categories the saves do not support.
- Do not append to `processed-ids.md`.

## Private folder

`~/bookmark-library/` unless the user named a different folder outside this repo.

## Steps

1. Take the new bookmarks from `pull-bookmarks`. If the list is empty, stop.
2. Open `~/bookmark-library/my-skills.md`. If it does not exist, copy `templates/my-skills.template.md` there before you propose any categories.
3. Read each item with the ladder below. Finish the ladder for every item before you name categories.
4. On the first run, or whenever `my-skills.md` has no accepted category names yet, cluster what this user saved and propose 5–12 categories. Name each one in the user's own terms, using words their bookmarks actually use. If there are fewer than 5 bookmarks, propose fewer and say so. Show the names, one line on why each exists, and which bookmarks sit in it. Stop until the user accepts, renames, merges, or splits them. If they already accepted names in this conversation, continue. A later run keeps the names already in the file. If new bookmarks do not fit, propose one new category and ask before you add it.
5. If the body is blank, choose the category from the title only. Append entries. Do not rewrite an entry after it is written. The only later edit allowed is the one in `triage-bookmarks`: it may change `Triage` from `pending` once, and it may fill `Next step` once. To correct anything else, append a new entry that names the id it updates. If the canonical URL already has an entry and you are not splitting per the rule below, reuse that entry.
6. Add each id to its category row in the index and increase the count.

## When to split one bookmark into several entries

Split only when the source teaches two or more techniques that need different actions: a different next step, a different agent, or a different category. Do not split supporting examples, a list of tips for one technique, or several points of one argument. A bookmark with one technique stays one entry. Each split entry uses the same source URL and its title names which part it covers. Entries that share a source URL are one bookmark in the ledger.

## Reading ladder

Stop at the first rung that gives you the body. Use the same ladder for an X post that will not open and for a paywall. Do not log in and do not bypass the wall.

1. **Full text.** Read the article body, or the full thread including the posts that continue it. If the page is only a link onward, open that destination and read it. A complete read is `full text`.
2. **Captions.** For video or audio, use platform captions when they cover the whole piece. A description, a blurb, or a chapter list is not a transcript. Complete captions are `full transcript`.
3. **Local transcript.** If captions are missing and both `yt-dlp` and `whisper` are already installed, run them locally. Do not install them unless the user asks. Do not upload the media. Write the transcript to `~/bookmark-library/transcripts/<id>.txt`. A completed local transcript is `full transcript`.
4. **Ask once.** Ask the user to paste the transcript or the full text. One ask per item. A paste that covers the piece is `full text` or `full transcript`, matching what they pasted.
5. **Mark and continue.** If this run gets no paste, do not wait and do not stop the other bookmarks. Use `partial` when some of the body was read and say what was missing. Use `title only (could not open)` when nothing but the title or a closed page was available. Leave the unknown parts blank.

## Entry

- **Id.** `S-001`, then the next free number. Never reuse or renumber an id.
- **Title.**
- **Source.** The canonical URL.
- **Category.** The accepted category name.
- **Triage.** `pending`.
- **Next step.** Leave blank.
- **What it is.**
- **How it helps.**
- **How to apply.**
- **How the source was read.** `full text`, `full transcript`, `partial` plus what was missing, or `title only (could not open)`.

Summarize in your own words. Keep quotes short. Claims and numbers stay the source author's. Do not treat them as checked facts.
