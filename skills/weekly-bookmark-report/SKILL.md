---
name: weekly-bookmark-report
description: Use at the end of a bookmark run to write the run report of what agents did and what needs the user, then record human-doable bookmarks now that the user has been told.
---

# Weekly bookmark report

Write one report for this run. The file name and the heading both use the run date. After the report is shown, record human-doable bookmarks. That is when the user has been told.

## Limits

- Do not post, send, pay, sign up, or delete unless the user explicitly tells you to do that specific thing.
- The report stays in the private folder. Never commit it.
- Do not invent results the queue and the library do not show.

## Private folder

`~/bookmark-library/` unless the user named a different folder outside this repo.

## Steps

1. Use the run date, `YYYY-MM-DD`, for both the file and the heading. Copy `templates/weekly-report.template.md` to `~/bookmark-library/weekly-report-YYYY-MM-DD.md`. Replace the heading so it reads `Run of YYYY-MM-DD` with that same date. If that file already exists, update it in place. Do not create a second file for the same date.
2. Under **Agent did it**, list entries from this run whose queue status is `sent` or `applied`, and any previously `sent` row that moved to `applied` during this run. Include the bookmark URL, the library entry id, the agent, the status, and what was done.
3. Under **Needs you**, list two kinds of rows. Each has one next step.
   - `needs human`: the next step already on the entry.
   - `queued`: the next step is to add a matching agent in `agents.md`. The item stays queued until then.
4. Set "New bookmarks" to the number of bookmarks `pull-bookmarks` returned this run. Count bookmarks, not library entries. A split bookmark still counts as one.
5. Show the report to the user. Showing this file is what counts as the user having been told.
6. Follow `templates/processed-ids.template.md`. For each bookmark that has at least one human-doable entry, append its ledger line only if every human-doable entry from it is under Needs you in the report you just showed, and every agent-doable entry from it is already `queued` or `sent`. Skip the line if that id or canonical URL is already in the ledger. Do not append bookmarks that are only agent-doable. Dispatch already recorded those.
