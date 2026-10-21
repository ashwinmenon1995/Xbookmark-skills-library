# AGENT.md

Follow these steps in order when the user says to run this file on their bookmarks. Read this file before you write anything.

Write the user's files in their own workspace, not in this repo. This repo holds the instructions, the templates, and one example. Their library, reports, and ledger stay theirs.

Do not post, send, pay, sign up, or delete anything unless the user explicitly tells you to do that specific thing.

## 1. Get the bookmarks

Connect to the user's bookmarks, or import an export they give you.

Sources may include X bookmarks, browser bookmarks, and read-later apps. Use an official export, API, or connector on the user's own account. Do not scrape.

For each item, keep a stable id, the URL, the title, the date saved, and the source. If the source has no id, use the canonical URL as the id.

If you cannot connect, ask for an export (JSON, CSV, HTML, or saved pages) and stop until you have it.

## 2. Skip bookmarks you already handled

Look for a processed-ids ledger beside `my-skills.md`. If it does not exist, create `processed-ids.md` with a short header and no ids.

Skip any bookmark whose id or canonical URL is already in the ledger. A rerun handles only new bookmarks.

Add an id only after that bookmark is fully read, written into `my-skills.md`, and either done or flagged. If you stop halfway, leave that id off the ledger so the next run retries it.

Ledger format, one bookmark per line:

```
id  url  YYYY-MM-DD
```

## 3. Read every new item in full

Do not skim. Do not write an entry from the title, the description, or a preview.

- Articles and threads: read the full text, including the rest of the thread and the article body.
- Videos and podcasts: get the full transcript. Use platform captions when they exist. Otherwise transcribe the audio.
- Pages that are only a link onward: open the destination and read that.

If you cannot open a source, say so in the entry and leave the unknown parts blank. Do not guess the content.

## 4. Derive categories from these bookmarks

Cluster what this user saved. Do not reuse a fixed category list, including the categories in `examples/example-library.md`. That file is one person's library. This user's will differ.

Propose 5–12 categories. Name each one in the user's own terms, using the words their bookmarks actually use. If they have fewer than 5 bookmarks, propose fewer categories and say so. Do not invent categories the saves do not support.

Show the proposed names, one line on why each exists, and which bookmarks sit in it. Then stop and let the user rename, merge, or split them. Write the index only after they accept the names.

On a later run, keep the category names already in `my-skills.md`. If new bookmarks do not fit, propose one new category and ask before you add it.

## 5. Write my-skills.md

On the first run, copy `templates/my-skills.template.md` to `my-skills.md` in the user's workspace.

Append entries. Do not rewrite an entry after it is written. To correct one, append a new entry that names the id it updates.

One entry per bookmark. If a bookmark contains several distinct techniques, write one entry per technique.

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

## 6. Turn each bookmark into an action

For each new entry, choose one:

- **Do it**, only when the action is reversible and low-risk. It must stay in the user's own files or drafts, and the user must be able to undo it by deleting that file or draft. Record what you did.
- **Flag it** for everything else. Give one concrete next step: the action, the object, and where to do it. One step, not a menu.

Do not post, send, pay, sign up, or delete without an explicit yes from the user for that action. That includes public posts, emails, direct messages, purchases, subscriptions, form submissions, account changes, and deleting bookmarks or files.

## 7. Write the action report

Copy `templates/weekly-report.template.md` to `weekly-report-YYYY-MM-DD.md` in the user's workspace.

Fill in only this run:

- **Agent did it.** The reversible actions you took, with the bookmark and the skill id.
- **Needs you.** Each flagged item, with the one next step from step 6.

## 8. Optional weekly schedule

After the first successful run, ask the user if they want this weekly. Do not create a schedule until they say yes.

A weekly run repeats steps 1–7 on new bookmarks only, then updates the ledger. The schedule follows the same limits: it does not post, send, pay, sign up, or delete unless the user has explicitly allowed that action.

## 9. Privacy

Do not copy the user's library, ledger, reports, or bookmark export into this repo. Do not include their name, handle, account details, or private notes in a file that will be committed or shared.

If they ask to contribute a generic improvement, change `AGENT.md` or `templates/` only, and leave their bookmarks out of the pull request.
