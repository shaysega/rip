# rip

A Claude Code plugin that reads your vibe-coded app and tells you the brutal truth.

No API key. No install friction. Uses your existing Claude Code session.

## Install

```bash
claude /plugin install https://github.com/shayse-xr/rip
```

Or load locally during development:

```bash
claude --plugin-dir ./rip
```

## Commands

Three levels of brutality. Pick your poison.

```
/rip:roast                              # grades A-F + what to fix
/rip:roast ./my-app
/rip:roast https://github.com/user/repo

/rip:kill                               # one paragraph, no mercy
/rip:kill ./my-app
/rip:kill https://github.com/user/repo

/rip:murder                             # short hits, each one lands
/rip:murder ./my-app
/rip:murder https://github.com/user/repo
```

Without an argument, each command analyzes the current directory.

## What it does

Reads your codebase and delivers an honest verdict on code quality, architecture, security, and whether the product concept makes any sense.

`/rip:roast` - structured critique with grades (A-F) and actionable fixes.

`/rip:kill` - one dense paragraph. Every sentence names a specific file, function, or line. No softening.

`/rip:murder` - 4-6 standalone hits. Each one a different angle. Closes with a one-liner.
