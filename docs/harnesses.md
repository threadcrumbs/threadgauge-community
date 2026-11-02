# Harnesses

A **harness** is whatever runs your agent threads: Claude Code, Codex, Cursor, and the rest.
Threadgauge reads each one's own files on your computer as they change. It never writes to them.

It shows the threads from the last 24 hours, plus every live one, from every harness on the
computer. Threads you archived or deleted in the harness are left out.

## What each one records

Harnesses save different things, and Threadgauge shows only what a harness actually saved. Where
it didn't, the card shows "—".

| Harness | Status | Tool | Context | Tokens | Spend | Lines | Plan | Subagents |
| --- | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
| **Claude Code** | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| **Codex** | ✅ | ✅ | ✅ | ✅ | — | ✅ | ✅ | ✅ |
| **OpenCode** | ✅ | ✅ | ✅ | ✅ | ✅ | ✅¹ | ✅ | ✅ |
| **Kilo Code** | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| **Hermes** | ✅ | ✅ | ✅ | ✅ | ✅ | — | ✅ | ✅ |
| **Cursor** | ✅ | Last called | — | — | — | — | ✅ | ✅ |
| **Antigravity CLI** | ✅ | — | — | — | — | — | ✅ | — |

¹ OpenCode 2.x doesn't record lines.

- **Codex** doesn't save what a thread cost, so there's no spend.
- **Codex's lines** are counted from the patches that applied.
- **Antigravity** writes its transcript only after each turn, and keeps tokens and context in a
  format that isn't read yet.
- **Claude Code's spend** is every reply's tokens at Anthropic's API list prices, subagents
  included, the same way Claude Code's `/usage` adds it up. A Pro or Max plan covers this usage,
  so it isn't what a subscriber pays.

## Opening a thread

Every card has an Open button that hands the thread back to its harness.

- **A thread running in a terminal:** that terminal comes to the front.
- **Claude Code:** the desktop app opens on the thread.
- **Most others:** their own link.
- **Cursor:** it has no link to a single thread, so Open opens the repo in Cursor.
- **Hermes:** there's no Open button, because Hermes has nothing to link to.
- **Linux with no desktop app:** the harness's CLI resumes the thread in a new terminal.
- **When nothing on the computer answers the link:** Claude Code threads try VS Code's Claude Code
  extension next. Otherwise, a dialog names the app that's missing, with a link to download it, and
  offers to open the thread in a terminal when the harness's CLI is installed.

## Not yet supported

Using a harness that isn't here? [Ask for it](https://github.com/threadcrumbs/threadgauge-community/issues/new?template=harness.yml).
If someone has already asked, a 👍 on their request helps us see what to add next.

Some of these readers were built from a harness's source code or documented formats and tested
against fake installs, not a real one. If one shows something wrong,
[report it](https://github.com/threadcrumbs/threadgauge-community/issues/new?template=bug.yml)
with the harness's version.
