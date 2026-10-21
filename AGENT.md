# AGENT.md

Run this file as a repeating cycle:

1. Pull the user's bookmarks.
2. Organize them into the user's own categories.
3. Triage each item as human-doable or agent-doable.
4. Dispatch agent-doable items to the user's own agents, and send human-doable items to the user with one concrete next step.

Then repeat on new bookmarks.

Write the user's files in their workspace, not in this repo. This repo holds the instructions, the templates, and one example.

Do not post, send, pay, sign up, or delete anything unless the user explicitly tells you to do that specific thing. Do not put that action in a task you hand to another agent either.

## 1. Pull the bookmarks

Connect to the user's bookmarks, or import an export they give you.

Sources may include X bookmarks, browser bookmarks, and read-later apps. Use an official export, API, or connector on the user's own account. Do not scrape.

For each item, keep a stable id, the URL, the title, the date saved, and the source. If the source has no id, use the canonical URL as the id.

If you cannot connect, ask for an export (JSON, CSV, HTML, or saved pages) and stop until you have it.

### Skip bookmarks already in the ledger

Look for `processed-ids.md` beside `my-skills.md`. If it does not exist, create it with a short header and no ids.

Skip any bookmark whose id or canonical URL is already in the ledger. A rerun pulls only new bookmarks. Still check the dispatch queue for rows marked `sent`, and update those statuses when the receiving agent has replied.

Add an id only after that bookmark is fully read, written into `my-skills.md`, triaged, and either dispatched or handed to the user. If you stop halfway, leave the id off the ledger so the next run retries it.

Before you append a skill, check the source URL. If that URL already has an entry, reuse it. Do not write a second entry.

Ledger format, one bookmark per line:

```
id  url  YYYY-MM-DD
```

### Read every new item in full

Do not skim. Do not write an entry from the title, the description, or a preview.

- Articles and threads: read the full text, including the rest of the thread and the article body.
- Videos and podcasts: get the full transcript. Use platform captions when they exist. Otherwise transcribe the audio.
- Pages that are only a link onward: open the destination and read that.

If you cannot open a source, say so in the entry and leave the unknown parts blank. Do not guess the content.

## 2. Organize into the user's categories

Cluster what this user saved. Do not reuse a fixed category list, including the categories in `examples/example-library.md`. That file is one person's library. This user's will differ.

Propose 5–12 categories. Name each one in the user's own terms, using the words their bookmarks actually use. If they have fewer than 5 bookmarks, propose fewer categories and say so. Do not invent categories the saves do not support.

Show the proposed names, one line on why each exists, and which bookmarks sit in it. Then stop and let the user rename, merge, or split them. Write the index only after they accept the names. If they already accepted names in this conversation, continue the cycle.

On a later run, keep the category names already in `my-skills.md`. If new bookmarks do not fit, propose one new category and ask before you add it.

### Write my-skills.md

On the first run, copy `templates/my-skills.template.md` to `my-skills.md`.

Append entries. Do not rewrite an entry after it is written. To correct one, append a new entry that names the id it updates.

One entry per bookmark. If a bookmark contains several distinct techniques, write one entry per technique, and triage each one.

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

## 3. Triage each item

For each new entry, choose one:

- **Agent-doable.** Applying it is reversible and low-risk, and it fits an agent in `agents.md`. The user can undo it by deleting a file, reverting a draft, or ignoring the task. Record that choice.
- **Human-doable.** Everything else. The user gets one concrete next step: the action, the object, and where to do it. One step, not a menu.

These are human-doable unless the user has explicitly allowed that exact action: posting, sending, paying, signing up, deleting, public posts, emails, direct messages, purchases, subscriptions, form submissions, and account changes.

## 4. Dispatch

### Routing table

On the first run, copy `templates/agents.template.md` to `agents.md`.

Ask the user to list their agents and what each one handles. Agents might include their Claude, Codex, Cursor, Grok, or others. Each row needs three fields: the agent, what it handles, and the channel it reads (a shared file, a sheet, an issue, or another queue).

Do not invent agents or channels. If `agents.md` has no rows, ask the user to fill it in and stop before dispatch. Leave those bookmarks off the ledger.

### Route each agent-doable item

Pick the best-fit row in `agents.md`. Write one self-contained task to that channel. The receiving agent must be able to do the task without this repo and without the rest of the library.

Use this shape:

```
# Task
- Skill: S-### · Title
- Source: url
- What it is:
- How it helps:
- How to apply:
- Do this: one reversible change in the workflow this agent already runs
- Do not: post, send, pay, sign up, or delete
- When done: reply on this channel with "applied", or with "needs human" and one next step
```

If writing to that channel would itself post, send, pay, sign up, or delete, do not dispatch. Triage the item as human-doable instead.

### Track status

On the first run, copy `templates/dispatch-queue.template.md` to `dispatch-queue.md`. One row per item. Status is only:

- `sent` — the task is on the channel and not confirmed yet
- `applied` — the receiving agent confirmed it applied the learning
- `needs human` — the user has to act, or the receiving agent could not apply it

Set agent-doable rows to `sent` when the task is on the channel. Set human-doable rows to `needs human` and put the one next step in that row. Do not mark `applied` until the receiving agent or the user confirms it.

On later runs, read replies on those channels and update `sent` rows to `applied` or `needs human` before you dispatch new work.

### Tell the user what is theirs

Send every `needs human` item to the user with its one next step. Do not dispatch those items to another agent.

## 5. Write the action report

Copy `templates/weekly-report.template.md` to `weekly-report-YYYY-MM-DD.md`.

Fill in only this run:

- **Agent did it.** Rows you dispatched or that moved to `applied`. Include the bookmark, the skill id, the agent, the status, and what was done.
- **Needs you.** Each `needs human` item, with the one next step.

## 6. Repeat

After the first successful pass, ask the user if they want this weekly. Do not create a schedule until they say yes.

A weekly run repeats this cycle on new bookmarks only, updates statuses for tasks already `sent`, writes the report, and updates the ledger. The schedule follows the same limits.

## 7. Privacy

Do not copy the user's library, routing table, dispatch queue, ledger, reports, or bookmark export into this repo. Do not include their name, handle, account details, or private notes in a file that will be committed or shared.

If they ask to contribute a generic improvement, change `AGENT.md` or `templates/` only, and leave their bookmarks out of the pull request.
