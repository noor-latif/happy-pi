# Project Sessions

This is the workspace root for sandboxed Claude project sessions.

## Environment

- Running in Docker with `--dangerously-skip-permissions`
- Full access to all repos in this directory
- SSH keys available for git operations
- `TMUX_WINDOW_NAME` env var contains your window name (if set)

## After Cloning a Repo

When you clone a repo, CLAUDE.md and settings won't be loaded until you restart.

**Use the restart_self MCP tool:**
```
Call restart_self with your window name to pick up CLAUDE.md and settings.
Your window name is in the TMUX_WINDOW_NAME environment variable.
```

This is needed because Claude Code reads CLAUDE.md and settings at startup, not dynamically.

## tmux Navigation

- `Ctrl-b w` - list all windows
- `Ctrl-b d` - detach (session keeps running)
