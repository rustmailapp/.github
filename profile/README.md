<p align="center">
  <img src="https://raw.githubusercontent.com/rustmailapp/.github/main/profile/logo.png" alt="RustMail" width="100" />
</p>

<h3 align="center">Local SMTP catcher built in Rust.</h3>

<p align="center">
  Catch, inspect, and assert on outbound email from dev and test environments.<br>
  Nothing gets delivered — everything lands in a local web UI instead.
</p>

---

**RustMail** is a single-binary SMTP server that captures outgoing mail and exposes it through a web UI and a REST API. SQLite-backed, dark-mode-first, built for developers who test email flows locally or in CI.

### Ecosystem

| Repository | What it does |
|---|---|
| **[rustmail](https://github.com/rustmailapp/rustmail)** | Core server — SMTP capture, web UI, REST API, CLI |
| **[rustmail-action](https://github.com/rustmailapp/rustmail-action)** | GitHub Action — start the server and assert on emails in CI |
| **[rustmail-homebrew](https://github.com/rustmailapp/rustmail-homebrew)** | Homebrew tap — `brew install rustmailapp/tap/rustmail` |
| **[rustmail.nvim](https://github.com/rustmailapp/rustmail.nvim)** | Neovim plugin — browse captured emails without leaving the editor |

### Quick start

```sh
# Install
brew install rustmailapp/tap/rustmail

# Run
rustmail

# Point your app's SMTP at localhost:1025, open localhost:8025
```

Or with cargo:

```sh
cargo install rustmail
```

Or with Docker:

```sh
docker run -p 1025:1025 -p 8025:8025 ghcr.io/rustmailapp/rustmail:latest
```

### Links

<a href="https://rustmail.app">Website</a> · <a href="https://github.com/rustmailapp/rustmail#documentation">Docs</a> · <a href="https://crates.io/crates/rustmail">Crates.io</a>
