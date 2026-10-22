---
name: dispatch-to-agents
description: Use when agent-doable bookmark items should be routed to the user's own agents as self-contained tasks and tracked as sent, applied, or needs human.
---

# Dispatch to agents

Route each agent-doable item to the best-fit agent in the user's routing table. Track every item in the dispatch queue.

## Limits

- Do not post, send, pay, sign up, or delete unless the user explicitly tells you to do that specific thing.
- Do not put that action in a task you hand to another agent.
- If writing to a channel would itself post, send, pay, sign up, or delete, do not dispatch. Send the item back to triage as human-doable.
- `agents.md` and `dispatch-queue.md` are private. Never commit them to this repo.

## Steps

1. On the first run, copy `templates/agents.template.md` to `agents.md` in the private folder. Ask the user to list their agents and what each one handles. Agents might include their Claude, Codex, Cursor, Grok, or others. Each row needs the agent, what it handles, and the channel it reads: a shared file, a sheet, an issue, or another queue. Do not invent agents or channels. If the table has no rows, ask the user to fill it in and stop. Do not write queue rows, and leave this run's bookmarks off the ledger.
2. On the first run, copy `templates/dispatch-queue.template.md` to `dispatch-queue.md` in the private folder.
3. Before routing new work, read replies on the existing channels. Update rows marked `sent` to `applied` or `needs human`. Do not mark `applied` until the receiving agent or the user confirms the learning was applied.
4. For each agent-doable item, pick the best-fit row. Write one self-contained task to that channel. The receiving agent must be able to do the task without this repo and without the rest of the library.

```
# Task
- Skill: S-### · Title
- Source: url
- What it is:
- How it helps:
- How to apply:
- Do this: one reversible change in the workflow this agent already runs
- Do not: post, send, pay, sign up, or delete
- When done: reply on this channel with "applied", or with "needs human" and one next step
```

5. Add or update one queue row per item. Status is only:
   - `sent` — the task is on the channel and not confirmed yet
   - `applied` — the receiving agent confirmed it applied the learning
   - `needs human` — the user has to act, or the receiving agent could not apply it
6. Set agent-doable rows to `sent` when the task is on the channel. Set human-doable rows to `needs human` and copy in the one next step from triage. Do not dispatch human-doable items to an agent.
