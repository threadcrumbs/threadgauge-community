# What stays on your computer

Threadgauge runs on your computer, reads your harnesses' files there, and shows the dashboard in
your browser. There's no account and no sign-in.

| | |
| --- | --- |
| **Reads** | Your harnesses' own session records and transcripts |
| **Writes** | Nothing, until you enter a Pro license key. Then it writes the license to `license.json` in the shared Threadcrumbs folder. With agent controls on, it keeps its own `agent-controls` folder there: a log of every answer, message, stop, and start, your saved prompts and actions, and its settings. Your dashboard choices are kept in your browser |
| **Writes to a harness** | Only when you turn on agent controls for it, after listing every file it writes, such as Claude Code's hooks in its `settings.json`. Messages between agents adds an entry to each harness's MCP settings. Undo removes them, and leaves only the log and your saved prompts and actions |
| **Runs** | Only when you ask: a missing harness's install command from its vendor, shown before it runs, and a terminal for that harness's own sign-in |
| **Sends** | Nothing, without Pro. With Pro: your license key and a random ID for this computer when you activate, then the license itself, to renew it about once a week |
| **Never sends** | Your threads, code, prompts, or project names. There's no telemetry |

The Threadcrumbs folder is `%APPDATA%\Threadcrumbs` on Windows,
`~/Library/Application Support/Threadcrumbs` on macOS, and `~/.local/share/threadcrumbs` on
Linux. Every Threadcrumbs app shares it, so a license entered in one counts in the others.

## Who can reach it

- **Your computer only:** the server listens on `127.0.0.1`.
- **Its own page only:** it refuses any request that names another host or comes from another
  website.
- **Its own script only:** the page runs only its own script, can't be put in a frame, and talks
  only to this server.
- **Your harnesses' hooks:** with agent controls on, Claude Code's hooks call it, signed with a
  secret only this computer holds.
- **Apps you allow:** Threadnauts sends prompts and actions through it only after you turn on Let
  Threadnauts send in Settings › Agent controls.

`THREADGAUGE_HOST` changes the address it listens on, and `THREADGAUGE_ALLOWED_HOSTS` lists other
names it answers to, comma separated. **Anyone who can reach the port sees every thread's title,
folder, and branch**, so only open it to a network you trust.

## What it opens

Threadgauge opens only what a thread touched: the files it changed or named, its folders, and its
transcript. **Open** hands a thread back to its harness through the harness's own link.
