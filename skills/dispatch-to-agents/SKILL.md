---
name: dispatch-to-agents
description: Use when agent-doable entries should be written as self-contained tasks for the user's agents, or left queued when no agent is listed yet, and tracked as queued, sent, applied, or needs human.
---

# Dispatch to agents

Route each agent-doable entry to the best-fit agent. If the user has not listed any agents, leave those entries queued and continue the run.

## Limits

- Do not post, send, pay, sign up, or delete unless the user explicitly tells you to do that specific thing.
- Do not put that action in a task you hand to another agent.
- If writing to a channel would itself post, send, pay, sign up, or delete, do not use that channel. Set the row to `needs human` and fill the next step. Do not record the bookmark for that reason alone.
- `agents.md`, `dispatch-queue.md`, and `inbox/` stay in the private folder. Never commit them.

## Private folder

`~/bookmark-library/` unless the user named a different folder outside this repo. Create `inbox/` there if it is missing.

## Ledger

Follow `templates/processed-ids.template.md`. Append a bookmark only when the entry you just queued or sent was the last unfinished entry from that bookmark. If any entry from it is human-doable, do not append. The report records it after the user has been told.

## Steps

1. Copy `templates/agents.template.md` to `~/bookmark-library/agents.md` if it does not exist. Copy `templates/dispatch-queue.template.md` to `~/bookmark-library/dispatch-queue.md` if it does not exist.
2. A row in `agents.md` is filled when the Agent cell is not blank. Read replies already in the inbox files and other channels. A confirmation is a line by itself, after the task, that is exactly `Status: applied` or starts with `Status: needs human:`. Do not treat the task text as a confirmation. Update the matching `sent` row. Do not mark `applied` without that line.
3. If `agents.md` has at least one filled row, route rows still marked `queued`. Use the best-fit agent. Then handle new agent-doable entries from this run the same way. One queue row per library entry id. If the row exists, update it. Do not add a second row.
4. If there is no filled row, do not stop and do not invent an agent. For each new agent-doable entry, write a queue row with Routed to empty, Channel empty, Status `queued`, and a one-line task summary. Do not create an inbox file for it. Ask the user to add agents when they can, then continue to the report.
5. When a filled row leaves Channel blank, the channel is `~/bookmark-library/inbox/<agent>.md`. `<agent>` is the agent name in lowercase, with spaces and slashes turned into hyphens. Append the task to that file. Tell the user to paste the file into that agent, or to point the agent at it. Skip this step for rows that stay `queued`.
6. The task must stand alone. The receiving agent does not need this repo or the rest of the library.

```
# Task
- Skill: S-### · Title
- Source: url
- What it is:
- How it helps:
- How to apply:
- Do this: one reversible change in the workflow this agent already runs
- Do not: post, send, pay, sign up, or delete
- When done: add a new line after this task, `Status: applied` or `Status: needs human: <one step>`
```

7. Set Status to `sent` only after the task is on that channel. Set human-doable rows to `needs human` and copy the next step from the entry. Do not dispatch human-doable entries to an agent.
8. Apply the ledger rule above for bookmarks whose last unfinished entry just became `queued` or `sent`.
