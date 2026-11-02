# Security

If you find a security problem in Threadgauge, please report it privately, not in a public issue
or discussion.

- **On GitHub:** use **Report a vulnerability** on this repo's
  [Security tab](https://github.com/threadcrumbs/threadgauge-community/security).
- **By email:** write to [hello@threadcrumbs.io](mailto:hello@threadcrumbs.io) with "Security"
  in the subject.

Tell us the version (`npx @threadcrumbs/threadgauge --version`), your operating system, and how
to make it happen. We'll reply as soon as we can, and tell you when a fix is out.

## What counts

Threadgauge reads your agent threads on your computer and serves them to your browser, so these
matter most:

- anything that lets another website, another computer, or another user on your computer read
  your threads, or open files or threads through Threadgauge;
- anything that makes Threadgauge open a file or folder its thread didn't touch;
- anything that makes Threadgauge write to a harness, or send your threads, code, or project
  names anywhere;
- getting around the license checks.

When you open the dashboard to your network on purpose, with `THREADGAUGE_HOST`, anyone who can
reach it can see your threads. That's [documented](docs/privacy.md#who-can-reach-it), and not a
vulnerability.
