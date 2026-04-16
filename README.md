# Hi, I'm Genie 👋

> A builder who knows nothing about coding — making small tools that do one thing well.

I ship single-file, zero-backend, open-source utilities for problems I actually hit.
No funnels, no mailing list, no Pro tier chasing. If it helps, star it. If not, carry on.

---

## 🔥 Currently shipping

### [ctxwatch](https://github.com/Genie-J/ctxwatch) — The smoke detector for Claude Code context saturation

A single-file Python CLI that tails your transcript JSONL and tells you, live, how close you are to the context window limit. Built in response to [anthropics/claude-code#49226](https://github.com/anthropics/claude-code/issues/49226) ("the alarm, not the smoke detector"). Stop-hook generator fires at a threshold of your choosing — exactly what the issue author asked for.

- Stdlib only. 20 unit tests. Auto-detects 1M-context subscribers.
- Sibling of `cc-healthcheck` (static) — this is the dynamic version.
- Install: `pipx install git+https://github.com/Genie-J/ctxwatch`

### [cc-healthcheck](https://github.com/Genie-J/cc-healthcheck) — What's eating your Claude Code context window?

A single-file Python CLI that audits everything auto-loading into your Claude Code session: `CLAUDE.md` + `@`-references + `rules/` + skills frontmatter. Lints your hooks against known pitfalls. X-rays the latest session JSONL.

- Zero dependencies. Zero network. Zero upload.
- Surfaces real issues: pipe-quoting bugs (#1132), missing hook timeouts, system-reminder inflation
- Run via `curl -sSL … | python3 -` — nothing stays on disk

### [burncheck](https://github.com/Genie-J/burncheck) — Know before the throttle hits

A single-file HTML tool that reads your `~/.claude/projects/*.jsonl` in-browser and projects whether your current burn rate will cross Anthropic's 7-day Opus or Sonnet cap before the week ends.

- Zero upload. Zero backend. Everything stays on your machine.
- Picks up `isSidechain` subagent calls and classifier sidequeries that `/cost` misses.
- Works via `npx github:Genie-J/burncheck` too, if you prefer terminal.

**Live:** https://genie-j.github.io/burncheck/

---

## 🛠️ Tools I reach for

- **Vanilla HTML + JS** over frameworks when the problem fits on one screen
- **JSONL** over SQLite for append-only telemetry
- **npx github:user/repo** over npm publish when iteration speed matters
- **Single-file deliverables** — if it can't be grokked in one read-through, it's too big

---

## 💬 How to reach me

- Open an [Issue](https://github.com/Genie-J/burncheck/issues) on any of my repos
- Or start a [Discussion](https://github.com/Genie-J/burncheck/discussions)

No DMs, no calendar links. Async is the whole point.
