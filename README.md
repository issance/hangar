# Hangar

The runtime your coding agents live on, part of issance. Hangar keeps every agent (Claude Code, Codex,
Pi, OpenCode and others) in its own terminal pane, keeps them running when you close the window, knows
which one is working, done or waiting for you, and lets the issance app on your phone see and drive them.

It runs on macOS, Linux and Windows.

## Install

The issance installer sets Hangar up for you. Then:

```bash
hangar            # open your agents
hangar --help     # every command
```

Configuration lives in `~/.config/hangar/` (Windows: `%USERPROFILE%\.hangar\`).

Hangar is a rebranded distribution of an Apache-2.0 project; see NOTICE-ISSANCE.md and LICENSE.
