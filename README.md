<div align="center">

<img src="assets/zap-logo.svg" alt="Zap" width="128" />

# Zap

[简体中文](./README.zh-CN.md) · [日本語](./README.ja.md)

<sub><i>Currently based on <a href="https://github.com/warpdotdev/warp">Warp</a>; evolving independently going forward.</i></sub>

</div>

Zap is an open, local-first terminal with first-class AI and agent support. Plug in any AI provider, bring in any CLI agent, manage SSH hosts inside the terminal — with keys, history and agent state staying on your machine by default.

## Install this fork on macOS

The current release of the [ThalesMMS fork](https://github.com/ThalesMMS/zap) supports **Apple Silicon Macs**. The app is signed with Developer ID and notarized by Apple.

### Homebrew

With [Homebrew](https://brew.sh/) installed, run:

```sh
brew install --cask ThalesMMS/tap/zap
```

Use the full name `ThalesMMS/tap/zap`: the short name `zap` identifies Zed Attack Proxy in Homebrew's official catalog. The two packages cannot be installed together.

If you already have a manually installed `Zap.app` in Applications, quit it and move it to a backup folder before installing through Homebrew. Keep your settings and application data in place.

To update:

```sh
brew update
brew upgrade --cask ThalesMMS/tap/zap
```

To uninstall the app while keeping its settings and data:

```sh
brew uninstall --cask ThalesMMS/tap/zap
```

The cask is maintained in [ThalesMMS/homebrew-tap](https://github.com/ThalesMMS/homebrew-tap).

### Direct download

Download the macOS ARM64 ZIP from [this fork's releases](https://github.com/ThalesMMS/zap/releases), extract it, and move `Zap.app` to Applications. If replacing an existing copy, quit Zap first and keep a backup of the old app.

## What Zap adds over upstream Warp

- **No mandatory cloud** — no account, login, Drive sync or cloud agent history required.
- **BYOP AI providers** — any OpenAI-compatible endpoint, plus native OpenAI / Anthropic / Gemini / DeepSeek / Ollama protocols. Keys stay local.
- **Third-party CLI agents** — DeepSeek-TUI / Codex CLI / Claude Code / Google Antigravity (`agy`) wired into Blocks and the notification center.
- **Built-in SSH host manager** — manage hosts, configs and sessions inside the terminal, with tmux integration.
- **Editable system prompts** — minijinja templates rendered on the client.
- **Rendering fixes** — tuned Markdown pipeline; CJK soft-wrap caret and bold subpixel fixes.
- **Localized UI** — English / Simplified Chinese / Japanese out of the box, community-extensible.
- **Privacy defaults** — Cloud Agent / Computer Use / Referral / telemetry off by default.

## Migrating from OpenWarp or Warp

If you used the project before it was renamed to Zap (formerly **OpenWarp**),
or are coming from upstream **Warp**, see
[docs/migrate-from-warp.md](docs/migrate-from-warp.md) to bring your settings
across.

## Roadmap

See [docs/roadmap.md](docs/roadmap.md).

## Acknowledgements

- [Warp](https://github.com/warpdotdev/warp) — the upstream terminal Zap is built on.
- [DeepSeek-TUI](https://github.com/Hmbown/DeepSeek-TUI) — first-class CLI agent partner.
