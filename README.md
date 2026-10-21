# Turn your bookmarks into action

Point your own AI agent at this repo. It reads the bookmarks you saved, groups them into categories that match what you actually keep, and turns each one into a skill plus a next step.

## Quick start

Point your agent at this repo and say: run AGENT.md on my bookmarks.

Any agent that can read a repo can do this (Claude, Codex, Cursor, Grok, or another). It will ask you to connect or export your bookmarks from X, your browser, or a read-later app.

## What you get

- Your own skills library (`my-skills.md`): categories named from your bookmarks, and one entry per bookmark.
- A weekly action report, split into what the agent did and what needs you, with a next step on each item that needs you.

The agent only acts on its own when the action is reversible and low-risk. It does not post, send, pay, sign up, or delete unless you tell it to.

## How to contribute

Open a pull request to improve `AGENT.md` or the files in `templates/`. Keep the change generic. Do not add names, handles, or account details.

`examples/example-library.md` is one finished library. Do not rewrite its entries. Your categories will be different.

Do not commit your own `my-skills.md`, reports, or bookmark exports.
