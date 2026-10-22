---
name: post-draft-check
description: Use when the user shares a post draft and wants it checked against their library, with specific fixes that cite entry ids.
---

# Post draft check

Check one draft the user shares. Suggest specific fixes. Cite the library entries each fix comes from.

## Limits

- Do not post, send, pay, sign up, or delete unless the user explicitly tells you to do that specific thing.
- Do not publish, schedule, or send the draft.
- Suggestions stay in the conversation or in a private note the user asked for. Never commit the draft or the notes to this repo.
- Cite real entry ids from `my-skills.md`. If the library has no relevant entry, say so. Do not invent an id.

## Private folder

`~/bookmark-library/` unless the user named a different folder outside this repo.

## Steps

1. Read the draft the user shared. If they did not include a draft, ask for it and stop.
2. Read `~/bookmark-library/my-skills.md`. If `~/bookmark-library/what-works-for-me.md` exists, read it so the suggestions fit what has worked for this user. Do not copy that file into a shared place.
3. Pick the entries that apply to this draft and this platform. Ignore entries that do not change this draft.
4. Suggest specific fixes. For each fix, name the entry id, the line or claim to change, and the replacement or the exact edit. Do not give a general note with no edit.
5. Leave the user's draft unchanged unless they ask you to apply the edits in their private files. Applying an edit is still not permission to post it.
