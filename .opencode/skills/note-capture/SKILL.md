---
name: note-capture
description: Use when the user asks to add, save, record, or upload a note to this knowledge base, including Danish requests such as "tilføj note" or "gem dette".
---

# Capture A Knowledge-Base Note

Turn the user's supplied text into a concise, useful Markdown note.

1. Use the stated date if the user provides one. Otherwise use today's local date in `YYYY-MM-DD` format.
2. Derive a short Danish filename slug from the subject. Store the note as `notes/YYYY/MM/YYYY-MM-DD-slug.md`.
3. Use this structure:

```markdown
# Titel

Dato: YYYY-MM-DD
Tags: tag-1, tag-2

## Noter

Indholdet af noten.
```

4. Create missing year and month folders as needed.
5. Add one link to `INDEX.md` under `## Noter`, sorted newest date first. Include the date and a short description.
6. Keep raw, incomplete captures in `INBOX.md` only when the user asks for an inbox note or the content has no identifiable subject.
7. After verifying the change, commit the note and the updated index immediately. Push only when the user explicitly says `push`, `upload`, or equivalent.

Preserve existing notes and links. If a note already exists for the same date and subject, update it rather than creating a duplicate.
