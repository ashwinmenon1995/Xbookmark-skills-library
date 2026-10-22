---
name: triage-bookmarks
description: Use when a new library entry needs a decision, classifying it as agent-doable and reversible or as human-doable with one concrete next step.
---

# Triage bookmarks

Classify each new library entry. Do not dispatch it and do not do the work yourself.

## Limits

- Do not post, send, pay, sign up, or delete unless the user explicitly tells you to do that specific thing.
- Do not label those actions agent-doable, and do not put them in a task for another agent.
- Keep the triage notes in the user's private workspace. Never commit them to this repo.

## Steps

1. Take the entries just added by `index-bookmarks`. If there are none, stop.
2. For each entry, choose one label.
   - **Agent-doable.** Applying it is reversible and low-risk. The user can undo it by deleting a file, reverting a draft, or ignoring a task. It must also fit an agent the user has listed, or could fit one they have not listed yet.
   - **Human-doable.** Everything else. Write one concrete next step: the action, the object, and where to do it. One step, not a menu.
3. These stay human-doable unless the user has explicitly allowed that exact action: posting, sending, paying, signing up, deleting, public posts, emails, direct messages, purchases, subscriptions, form submissions, and account changes.
4. Give the labeled list to `dispatch-to-agents`. For each human-doable item, include the one next step. Tell the user those next steps in this run. Do not send them to another agent.
