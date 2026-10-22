# processed-ids

One bookmark per line. This is the only ledger. Append a line only when that bookmark is finished. Never append the same id or the same canonical URL twice.

`pull-bookmarks` only reads this file. `index-bookmarks` and `triage-bookmarks` do not append.

Entries with the same canonical source URL are one bookmark. A bookmark is finished when every entry from it is finished:

- An **agent-doable** entry is finished when `dispatch-queue.md` has a row for that entry id with status `queued` or `sent`. `dispatch-to-agents` appends the bookmark if that was the last unfinished entry.
- A **human-doable** entry is finished when its one next step is under "Needs you" in the run report and that report has been shown to the user. That is when the user has been told. `weekly-bookmark-report` appends the bookmark if that was the last unfinished entry.

Ignore blank lines and lines that start with `#`.

Line format, two spaces between fields:

```
id  url  YYYY-MM-DD
```
