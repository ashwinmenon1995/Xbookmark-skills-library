---
name: pull-bookmarks
description: Use when fetching or exporting the user's bookmarks from X, a browser, or a read-later app, and when skipping bookmarks already recorded so a rerun handles only new ones.
---

# Pull bookmarks

Fetch the user's bookmarks and return only the ones not yet in the processed-ids ledger. This skill does not read, classify, or dispatch them.

## Limits

- Do not post, send, pay, sign up, or delete unless the user explicitly tells you to do that specific thing.
- Do not scrape. Use an official export, API, or connector on the account the user authorizes.
- Keep the ledger and any export in the user's private workspace. Never commit them to this repo.

## Steps

1. Pick a private folder in the user's workspace. If the current directory is this kit, choose a different folder. Do not create private files here.
2. Open `processed-ids.md` in that folder. If it does not exist, create it with a one-line header and no ids.
3. Connect to the user's bookmarks, or import an export they give you. Sources may include X bookmarks, browser bookmarks, and read-later apps. If you cannot connect, ask for an export (JSON, CSV, HTML, or saved pages) and stop until you have it.
4. For each item, keep a stable id, the URL, the title, the date saved, and the source. If the source has no id, use the canonical URL as the id.
5. Drop any item whose id or canonical URL is already in the ledger. Return the remaining items to the next skill. Do not record them yet.

## Record a processed id

Record an id only after that bookmark has been indexed, triaged, and either dispatched or handed to the user with a next step. If a later skill stops halfway, leave the id off the ledger so the next run retries it.

Append one line per finished bookmark:

```
id  url  YYYY-MM-DD
```

Do not record the same id or canonical URL twice.
