# AGENT.md

Orchestrator. Do the work by reading each skill file and following it. Do not replace those steps with a shorter version.

Private files go in `~/bookmark-library/` unless the user named a different folder outside this repo. Never write them in this repo.

Do not post, send, pay, sign up, or delete anything unless the user explicitly tells you to do that specific thing. Do not put that action in a task you hand to another agent.

The only ledger is `~/bookmark-library/processed-ids.md`. Follow `templates/processed-ids.template.md`. The skill that finishes a bookmark appends it. Human-doable bookmarks are appended only after the run report has told the user.

## Bookmark cycle

When the user says to run this file on their bookmarks, call these five skills in order. Finish each one before the next. If `index-bookmarks` is waiting for the user to accept category names, stop until they answer.

1. `skills/pull-bookmarks/SKILL.md`
2. `skills/index-bookmarks/SKILL.md`
3. `skills/triage-bookmarks/SKILL.md`
4. `skills/dispatch-to-agents/SKILL.md`
5. `skills/weekly-bookmark-report/SKILL.md`

Then repeat on new bookmarks. After the first successful pass, ask if they want this weekly. Do not create a schedule until they say yes. A later run calls the same five skills. `pull-bookmarks` skips ids already in the ledger. `dispatch-to-agents` also sends anything still `queued`.

## Optional content skills

Not part of the cycle. Call one only when the user asks for it.

- `skills/weekly-content-plan/SKILL.md` when they want post ideas for the week.
- `skills/post-draft-check/SKILL.md` when they share a draft.
- `skills/weekly-content-review/SKILL.md` when they want a lookback at performance.

## Privacy

Do not copy the user's library, routing table, dispatch queue, ledger, inbox, reports, content plans, drafts, or `what-works-for-me.md` into this repo. Do not include their name, handle, account details, or private notes in a file that will be committed.
