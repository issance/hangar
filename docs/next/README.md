# hangar


<p align="center">
  <img src="assets/logo.png" alt="hangar" width="100" />
</p>

<p align="center">
  <a href="https://issance.com">herdr.dev</a> · <a href="#install">install</a> · <a href="https://issance.com/docs/hangar/quick-start/">quick start</a> · <a href="https://issance.com/docs/hangar/">docs</a>
</p>

<p align="center">
  English · <a href="README.zh-CN.md">简体中文</a>
</p>

<p align="center">
  <a href="LICENSE"><img src="https://img.shields.io/badge/license-Apache--2.0-666666?labelColor=333333" alt="Apache 2.0 license" /></a>
  <a href="https://github.com/issance/hangar/releases"><img src="https://img.shields.io/github/downloads/issance/hangar/total?labelColor=333333&color=666666" alt="total GitHub release downloads" /></a>
  <a href="https://github.com/issance/hangar/stargazers"><img src="https://img.shields.io/github/stars/issance/hangar?labelColor=333333&color=666666&logo=github" alt="GitHub stars" /></a>
  <a href="https://github.com/issance/hangar/releases/latest"><img src="https://img.shields.io/github/v/release/issance/hangar?label=release&labelColor=333333&color=666666" alt="latest stable release" /></a>
  <a href="https://formulae.brew.sh/formula/hangar"><img src="https://img.shields.io/homebrew/v/hangar?label=homebrew&labelColor=333333&color=666666" alt="Homebrew version" /></a>
  <a href="https://x.com/herdrdev"><img src="https://img.shields.io/badge/follow-%40herdrdev-000000?logo=x&logoColor=white" alt="follow @herdrdev on X" /></a>
</p>

---

https://github.com/user-attachments/assets/043ec09f-4bdd-41d5-aee0-8fda6b83e267

**the runtime your coding agents live on.**

- **detach without stopping work** — hangar keeps terminals running in a background server when you close the client or lose your SSH connection. after a server or machine restart, hangar restores the saved layout and can resume supported agent sessions; the original processes do not survive. [session state →](https://issance.com/docs/hangar/session-state/)
- **several machines, one window** — keep local work and saved ssh machines together, with a combined agent list and independent reconnects. [remote machines →](https://issance.com/docs/hangar/connecting-machines/)
- **never hunt for the stuck one** — every pane is marked working, blocked, or idle. when an agent stops and needs an answer, hangar says so.
- **agent-native** — agents drive hangar through the cli and socket api: they can spawn panes, prompt each other, and wait until another agent is genuinely blocked. [agent skill →](https://issance.com/docs/hangar/agent-skill/)
- **runs what you already run** — claude code, codex, cursor, opencode, grok and the rest. hangar doesn't wrap or replace them; it owns their terminals. building an agent? [add hangar support →](https://issance.com/docs/hangar/add-herdr-support/)
- **keyboard and mouse, both first-class** — tmux-style prefix keys *and* click, drag, split. pick per moment, not per tool.
- **plugins** — extend panes and workflows. [browse the marketplace →](https://issance.com/plugins/)
- **one rust binary, no electron** — runs in whatever terminal you already use.

---

## install

```bash
curl -fsSL https://issance.com/install.sh | sh
```

or `brew install hangar` · `mise use -g hangar` · windows: `powershell -ExecutionPolicy Bypass -c "irm https://issance.com/install.ps1 | iex"` · [endpoint-protected Windows](https://issance.com/docs/hangar/windows-beta/) · [binaries](https://github.com/issance/hangar/releases)

then start it where the work lives:

```bash
hangar
```

run your agents, split panes, walk away. `ctrl+b q` detaches, `hangar` reattaches. [quick start →](https://issance.com/docs/hangar/quick-start/)

## docs

everything lives at [herdr.dev/docs](https://issance.com/docs/hangar/): [quick start](https://issance.com/docs/hangar/quick-start/) · [concepts](https://issance.com/docs/hangar/concepts/) · [supported agents](https://issance.com/docs/hangar/agents/) · [keyboard](https://issance.com/docs/hangar/keyboard/) · [configuration](https://issance.com/docs/hangar/configuration/) · [session state](https://issance.com/docs/hangar/session-state/) · [connecting machines](https://issance.com/docs/hangar/connecting-machines/) · [remote](https://issance.com/docs/hangar/persistence-remote/) · [integrations](https://issance.com/docs/hangar/integrations/) · [add hangar support to your agent](https://issance.com/docs/hangar/add-herdr-support/) · [plugins](https://issance.com/docs/hangar/plugins/) · [socket api](https://issance.com/docs/hangar/socket-api/)

## thanks

every past sponsor and backer is listed in [SPONSORS.md](./SPONSORS.md) — thank you 🐑

enterprise / partnership: hey@herdr.dev

## agent instructions

if you are an ai agent helping with this repository, read [`AGENTS.md`](./AGENTS.md) before making changes and read [`CONTRIBUTING.md`](./CONTRIBUTING.md) before opening issues or PRs.

## development

```bash
git clone https://github.com/issance/hangar
cd hangar
cargo build --release

just test        # unit tests
just check       # formatting, tests, and maintenance checks
```

## license

Hangar is licensed under the [Apache License 2.0](LICENSE).
