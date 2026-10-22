---
name: triage-bookmarks
description: Use when a new library entry is still pending, to classify it as agent-doable and reversible or as human-doable with one concrete next step.
---

# Triage bookmarks

Classify each new library entry. Do not dispatch it, do not do the work, and do not record the ledger.

## Limits

- Do not post, send, pay, sign up, or delete unless the user explicitly tells you to do that specific thing.
- Do not label those actions agent-doable, and do not put them in a task for another agent.
- Do not append to `processed-ids.md`. `weekly-bookmark-report` records a human-doable bookmark after the user has been told in the run report.

## Private folder

`~/bookmark-library/` unless the user named a different folder outside this repo.

## Steps

1. Open `~/bookmark-library/my-skills.md`. Take entries whose Triage line is `pending`. If there are none, stop.
2. Choose one label from the entry itself. Do not look at `agents.md`, and do not choose agent-doable because an agent could be added later. If the source was read as `title only` or `partial` and the body is blank, choose human-doable. The next step is: paste the missing text or transcript for that source URL.
   - **Agent-doable.** Applying it is reversible and low-risk. The user can undo it by deleting a file, reverting a draft, or ignoring a task. Nothing is posted, sent, paid, signed up for, or deleted.
   - **Human-doable.** Everything else. Write one concrete next step: the action, the object, and where to do it. One step, not a menu.
3. These stay human-doable unless the user has explicitly allowed that exact action: posting, sending, paying, signing up, deleting, public posts, emails, direct messages, purchases, subscriptions, form submissions, and account changes.
4. Edit only the `Triage` line, from `pending` to `agent-doable` or `human-doable`. For a human-doable entry, also fill the blank `Next step` line. Do not change any other line.
5. In this run's reply, list each human-doable entry id and its one next step. Do not send those items to another agent. The run report is what counts as the user having been told for the ledger.
