# What stays on your computer

Threadgauge runs on your computer, reads your harnesses' files there, and shows the dashboard in
your browser. There's no account and no sign-in.

| | |
| --- | --- |
| **Reads** | Your harnesses' own session records and transcripts |
| **Writes** | Nothing, until you enter a Pro license key. Then it writes the license to `license.json` in the shared Threadcrumbs folder. Your dashboard choices are kept in your browser |
| **Never writes** | Anything belonging to a harness |
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

`THREADGAUGE_HOST` changes the address it listens on, and `THREADGAUGE_ALLOWED_HOSTS` lists other
names it answers to, comma separated. **Anyone who can reach the port sees every thread's title,
folder, and branch**, so only open it to a network you trust.

## What it opens

Threadgauge opens only what a thread touched: the files it changed or named, its folders, and its
transcript. **Open** hands a thread back to its harness through the harness's own link.
