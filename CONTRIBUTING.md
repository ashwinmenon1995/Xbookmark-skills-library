# Contributing

Improvements to `AGENT.md`, `skills/`, `templates/`, and the docs are welcome. Open a pull request.

## Rules

- Keep the change generic. Do not add names, handles, account details, bookmark exports, or categories taken from one person's saves.
- Do not commit private output. That includes `my-skills.md`, `agents.md`, `dispatch-queue.md`, `processed-ids.md`, `weekly-report-*.md`, `content-plan-*.md`, `what-works-for-me.md`, `inbox/`, and `private/`. The default private folder is `~/bookmark-library/`, outside this repo.
- Do not add instructions to scrape, bypass a login, or bypass a paywall.
- A skill does not post, send, pay, sign up, or delete unless the user explicitly allows that exact action.

## Add a skill

1. Create `skills/<name>/SKILL.md`.
2. Start with YAML frontmatter: `name` (the folder name) and `description` (what it does and when to use it).
3. Write numbered steps another agent can follow without this conversation.
4. Add a row to the skills table in `README.md`.
5. If it belongs in the bookmark cycle, add it to the numbered list in `AGENT.md`. Content skills stay on the optional list.

The fake files in `examples/` show the shape of private output. Do not replace them with real bookmarks.
