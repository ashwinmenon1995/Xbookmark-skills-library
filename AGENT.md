# AGENT.md

Orchestrator. Do the work by reading each skill file and following it. Do not replace those steps with a shorter version.

Write private files in the user's workspace, not in this repo. This repo holds the instructions, the skills, and the templates.

Do not post, send, pay, sign up, or delete anything unless the user explicitly tells you to do that specific thing. Do not put that action in a task you hand to another agent.

## Run the bookmark cycle

When the user says to run this file on their bookmarks, call these skills in order. Finish each one before the next. If a skill stops to wait for the user, do not continue until they answer.

1. `skills/pull-bookmarks/SKILL.md`
2. `skills/index-bookmarks/SKILL.md`
3. `skills/triage-bookmarks/SKILL.md`
4. `skills/dispatch-to-agents/SKILL.md`
5. `skills/weekly-bookmark-report/SKILL.md`

Then repeat on new bookmarks. After the first successful pass, ask if they want this weekly. Do not create a schedule until they say yes. A weekly run calls the same five skills again. `pull-bookmarks` skips ids already in the ledger.

## Run the content skills

Call these when the user asks, in this order:

6. `skills/weekly-content-plan/SKILL.md` when they want ideas for the week.
7. `skills/post-draft-check/SKILL.md` when they share a draft. Skip it when they have no draft.
8. `skills/weekly-content-review/SKILL.md` when they want a lookback at performance.

A full week calls 1–6, then 7 if they share a draft, then 8. Skills 6–8 read the private library. They do not replace steps 1–5.

## Privacy

Do not copy the user's library, routing table, dispatch queue, ledger, reports, content plans, drafts, or `what-works-for-me.md` into this repo. Do not include their name, handle, account details, or private notes in a file that will be committed.

If they ask to contribute a generic improvement, change `AGENT.md`, `skills/`, or `templates/` only.
