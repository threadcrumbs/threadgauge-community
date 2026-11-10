# Changelog

What changed in each release of Threadgauge. Run `npx @threadcrumbs/threadgauge@latest` to get
the newest one.

## 0.1.2 — November 10, 2026

- **Long titles stay short:** a thread whose title is a whole prompt now shows only its first line,
  up to 120 characters, and never more than two lines in the list.
- **Activity stays compact:** a long command stays on one line, cut off with "…". Hover it or open
  the call to see all of it.
- **Rings you can read:** the rings beside Output, Input, Cache reads, Cache writes, and Spend are
  now as tall as their label and number.
- **More room in a subagent's view:** its context chart is wider, on the left, with its figures
  beside it, so Activity and Tools start higher. When the subagent runs its thread's model, the
  chart is colored against the same limit as the thread's.

## 0.1.1 — November 9, 2026

- **The loading screen stays dark:** it no longer shows a lighter panel behind it while it fades in.
- **Waiting on agents is right for Claude Code:** a thread whose turn has ended while its background
  subagents keep working now shows Waiting on agents instead of Working.

## 0.1.0 — November 9, 2026

The first release.

- **Every agent on this computer, live:** one list of every thread from Claude Code (the desktop
  app and the CLI), Codex, Cursor, OpenCode, Kilo Code, Hermes, and Antigravity CLI. Each row shows
  its status, what it's doing right now, how full its context is, its output, and the lines it has
  changed. Threads older than a day are listed too.
- **What needs you, first:** Needs you, Error, Done, Working, Waiting on agents, and Idle, in the
  same colors as Threadnauts. A thread that's stopped shows why: the question and its options, the
  command waiting for permission, or the error.
- **Every thread in a table:** close a thread and the window lines them all up, sorted by any
  column.
- **A thread's details:** its plan, subagents, thoughts, activity, errors, files changed with the
  agent's own diffs, tools, context (what fills the window, the room left, and every reply against
  the limit), prompts, and session, plus the Conversation, its prompts and replies.
- **Back to where it runs:** the harness's chip opens a thread in its own app or terminal. Files
  open in VS Code, Cursor, Windsurf, Zed, or the default app, and the resume command is one copy
  away.
- **Group, sort, and search:** by whose turn it is, by repo and organization, or by state. Press N
  for the next thread waiting on you, J and K to step through the list, / to search, and Ctrl+K
  for threads and actions.
- **Usage limits:** Codex's 5-hour and weekly limits, in the list's footer.
- **On a phone too:** the list sits above the details, with a bar to step between threads.
- **Free:** everything Threadgauge shows is free. Threadgauge Pro, for answering and directing your
  agents from Threadgauge, arrives with Threadbare.
- **Stays on your computer:** Threadgauge reads each harness's own files and uploads nothing about
  your threads. It answers only its own page, on your own computer.
- **Beside Threadnauts:** the two apps share ports from 5274, start in either order, and agree on
  every thread. While Threadgauge runs, Threadnauts' bot cards show what each thread is doing and
  what it needs from you.
