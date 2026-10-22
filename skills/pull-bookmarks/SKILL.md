---
name: pull-bookmarks
description: Use when fetching or exporting the user's bookmarks from X, a browser, or a read-later app, and when skipping bookmarks already listed in the ledger so a rerun handles only new ones.
---

# Pull bookmarks

Fetch the user's bookmarks and return only the ones not yet in the ledger. This skill does not read, classify, dispatch, or record them.

## Limits

- Do not post, send, pay, sign up, or delete unless the user explicitly tells you to do that specific thing.
- Do not scrape. Do not bypass a login.
- Keep exports and `processed-ids.md` in the private folder. Never commit them to this repo.

## Private folder

`~/bookmark-library/` unless the user named a different folder outside this repo. Create it if it is missing. Do not create it inside the kit repo.

## Steps

1. Copy `templates/processed-ids.template.md` to `~/bookmark-library/processed-ids.md` if that file does not exist.
2. Read the ledger. Ignore blank lines and lines that start with `#`.
3. Get bookmarks from one of the sources below, or from an export the user already handed you. If none of that is available, ask them to paste URLs, one per line. If they still have nothing, stop.
4. For each item, keep a stable id, the canonical URL, the title, the date saved, and the source. If the source has no id, the canonical URL is the id.
5. Canonical URL: lowercase the host, remove the fragment (`#...`), and remove one trailing slash. Keep the query string.
6. Drop any item whose id or canonical URL is already in the ledger. Return the rest to `index-bookmarks`. Do not append to the ledger.

## Getting your bookmarks

Use an official export, API, or connector the user authorizes. Do not scrape.

| Source | What to export | Fields to parse |
|---|---|---|
| X | Bookmarks from the official X API or a connector signed in as the user. The downloadable account archive may not include bookmarks, so do not treat an archive file as the bookmark list. | Post id, post URL, text if the API returns it, bookmarked time if present. Id is the post id. |
| Chrome | Bookmark manager, menu, Export bookmarks. Save the HTML file. | `HREF` is the URL, the link text is the title, `ADD_DATE` is the saved time when present (Unix seconds). Id is the canonical URL. |
| Firefox | Manage bookmarks, Import and Backup, Export Bookmarks to HTML. | Same HTML fields as Chrome. |
| Safari | File, Export Bookmarks. Save the HTML file. | Same HTML fields as Chrome. |
| Pocket | Account settings, Export, CSV. | Title, URL, time added, tags. Id is the canonical URL. |
| Readwise | The CSV of saved documents from account settings. | Document title, source URL, saved or created date. Ignore other columns. Id is the canonical URL. |
| Raindrop | Settings, Backups, download the CSV. | Title, URL, created time, folder, tags. Id is the canonical URL. |
| Fallback | The user pastes URLs, one per line. Skip blank lines and lines that start with `#`. | The URL is the id and the canonical URL. Title is unknown until the next skill reads it. Saved date is the run date. Source is `pasted`. |

If several sources are present, merge them and drop duplicate canonical URLs.
