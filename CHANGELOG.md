# Changelog

What changed in each release of Threadgauge. Run `npx @threadcrumbs/threadgauge@latest` to get
the newest one.

## 0.2.3 — November 11, 2026

- **Message any thread:** a Message button in each thread's header, R, Ctrl+K, and Reply on phones
  open the composer. A sent message shows Sending, then Sent.
- **Code as you type:** close a backtick for inline code, or type ``` and Shift+Enter for a code
  block. Enter still sends the Markdown you see.
- **Set up from where you are:** with agent controls off, Message, Respond, and Retry say so, and
  lead to one confirm that turns them on and lists the files it writes. Settings' switches use the
  same confirm.
- **Fewer words:** messages and the composer match the details' text size, the composer bar wraps
  instead of cutting off, and each note is one short line.
- **Clearer states:** a box that can't send is dimmed and says why. Free's locked controls say what
  they'd do, and Free's Conversation ends with a locked chat box. Stop has a label, and answer
  options look clickable.
- **Faster typing:** a keystroke in a 5,000-line draft takes about 12 ms, down from 107.
- **Remove from this computer:** Settings › Threadcrumbs can take your license off this computer.
  Free its slot in the customer portal.

## 0.2.2 — November 10, 2026

- **Install a missing CLI:** when a harness's threads are on this computer but its CLI isn't,
  Settings › Agent controls and the composer say so, with the install command to copy and a link to
  the vendor's install page. For Claude Code, Codex, Gemini CLI, Copilot CLI, Kilo Code, and
  Antigravity, Install it shows the vendor's own command and where it comes from before anything
  runs, then its progress. It's free, and it works with agent controls off. Cursor, Hermes, and
  OpenCode link to their install pages.
- **Found right away:** a CLI you install shows up without restarting Threadgauge.
- **Sign in:** after an install, Sign in opens a terminal running the CLI's own login. Threadgauge
  never sees your login.

## 0.2.1 — November 10, 2026

- **Message idle Claude Code threads:** a Claude Code thread with no process running now counts as
  between turns for certain, so you can message it. Before, it counted as a guess.
- **A thread open in its own app:** Send queues your message for a Claude Code thread there, and it
  goes in when its next turn ends. Or choose Continue here to resume it in your own CLI beside the
  open window, after a one-line confirm.
- **Why it can't send, and the fix:** when nothing can reach a thread, the composer says why, with
  the fix, such as turning on its hooks or closing it in its own app.
- **Upgrade to the bundle:** with Threadgauge Pro or Threadnauts Pro, Settings › Threadcrumbs offers
  Upgrade to the bundle, and so does the Pro dialog when your plan lacks Threadgauge Pro. It opens
  Polar's customer portal to change your plan, and you pay only the difference. If Polar asks for a
  payment method, add one in the portal's settings first.
- **On [threadgauge.io/pro](https://threadgauge.io/pro):** "Already subscribed?" links to the
  customer portal, and the FAQ says how to upgrade to the bundle.

## 0.2.0 — November 10, 2026

Threadgauge Pro is on sale: $29 a year, or $49 a year for the Threadcrumbs Pro Bundle with
Threadnauts Pro, at [threadgauge.io/pro](https://threadgauge.io/pro). Everything Threadgauge shows
stays free.

- **Answer your agents:** allow or deny a permission request, pick an option or answer a question,
  or retry after an error, in a thread's details and its Conversation.
- **Message a thread:** send a message now or when its turn ends, and cancel one that's still
  waiting.
- **Stop and start agents:** stop a thread while it works, or start a new one in any folder from
  New thread, with your own CLI and its own login.
- **Prompts and actions:** built-in ones and your own, from More, Ctrl+K, a key you give them,
  quick actions that fit the thread's status, and each section's actions. Choose threads in the
  table to run one on all of them.
- **Agents message each other:** agents in Claude Code, Codex, and Cursor can message threads in
  any harness, under rules you set, with Deliver and Deny for the messages that wait for you. The
  Messages section and the Message log show every one.
- **From Threadnauts:** its Commander's prompts and actions go through Threadgauge once you let
  it, in Settings › Agent controls.
- **Nothing written until you turn it on:** one switch in Settings › Agent controls lists every file
  it writes, such as Claude Code's hooks, and Undo removes them. Every answer, message, stop, and
  start is logged, and nothing goes to an agent while its status is only a guess. The Session
  section says how each thread is reached.
- **On the free tier,** each Pro control says what it does, with Get Pro and "I have a key".

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
  agents from Threadgauge, comes next.
- **Stays on your computer:** Threadgauge reads each harness's own files and uploads nothing about
  your threads. It answers only its own page, on your own computer.
- **Beside Threadnauts:** the two apps share ports from 5274, start in either order, and agree on
  every thread. While Threadgauge runs, Threadnauts' bot cards show what each thread is doing and
  what it needs from you.
