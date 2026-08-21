---
name: date-sort-notes
description: Use when the user asks to sort, organize, index, or clean up knowledge-base notes by date, including Danish requests such as "sorter noter efter dato".
---

# Sort Knowledge-Base Notes By Date

Organize the completed Markdown notes without losing their content or links.

1. Read each note's `Dato: YYYY-MM-DD` metadata. If it is absent, use a leading `YYYY-MM-DD` filename prefix. If neither exists, leave the note in place and report it for manual dating.
2. Move each dated note to `notes/YYYY/MM/YYYY-MM-DD-slug.md`, where the year and month come from its date.
3. Keep filenames lowercase, ASCII where possible, and hyphen-separated. Do not overwrite a different existing note; use a distinct descriptive slug instead.
4. Rebuild the `## Noter` section in `INDEX.md` from the dated notes, sorted newest first. Each entry must contain a relative Markdown link, date, and short description.
5. Do not move `INBOX.md` entries automatically; they are intentionally unsorted.
6. After verifying the sorting result, commit the affected notes and index immediately. Push only when the user explicitly asks for it.

After sorting, state how many notes were moved, indexed, and left undated.
