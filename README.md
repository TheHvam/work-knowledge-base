# Work Knowledge Base

Personlig knowledge base til arbejdsnoter, beslutninger, guides og research.

## Struktur

- `INBOX.md` - hurtige noter, som endnu ikke er sorteret.
- `INDEX.md` - oversigt over de vigtigste og færdige noter.
- `notes/YYYY/MM/` - færdige noter, sorteret efter notens dato.

## Konventioner

- Brug små bogstaver og bindestreger i filnavne, fx `notes/2026/08/2026-08-21-github-adgang.md`.
- Start noter med en tydelig titel, `Dato` og eventuelle `Tags`.
- Opret nye eller ufærdige noter i `INBOX.md`; flyt dem til `notes/`, når emnet og indholdet er klart.
- Tilføj færdige noter til `INDEX.md`, så de kan findes igen.

Ændringer committes lokalt umiddelbart efter validering. Push til GitHub sker kun, når det ønskes.

## OpenCode-kommandoer

- `/note <indhold>` opretter en dateret note og opdaterer indekset.
- `/sorter-noter` gennemgår og placerer eksisterende noter i datomapper samt sorterer indekset nyeste først.

Skriv "upload", "commit" eller "push", når ændringen også skal lægges på GitHub.
