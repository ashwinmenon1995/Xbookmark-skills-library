---
name: weekly-bookmark-report
description: Use at the end of a bookmark run, or on a weekly pass, to report what agents did and what still needs the user, with one next step on each item that needs them.
---

# Weekly bookmark report

Write one report for this run. Split what agents did from what needs the user.

## Limits

- Do not post, send, pay, sign up, or delete unless the user explicitly tells you to do that specific thing.
- The report is private. Never commit it to this repo.
- Include only this run. Do not invent results the queue does not show.

## Steps

1. Copy `templates/weekly-report.template.md` to `weekly-report-YYYY-MM-DD.md` in the private folder. Use today's date. If that file already exists for this run, update it instead of starting a second report.
2. Under **Agent did it**, list rows you dispatched or that moved to `applied`. Include the bookmark, the library entry id, the agent, the status (`sent` or `applied`), and what was done.
3. Under **Needs you**, list each `needs human` item from this run. Each row has one concrete next step: the action, the object, and where to do it.
4. Show the report to the user.
5. Record a processed id, using the record step in `pull-bookmarks`, only for bookmarks that have a queue row from this run. If dispatch stopped before writing the queue, record nothing.
