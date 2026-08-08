# Hi, I'm Amen 👋

Building voice AI, agent tooling, and developer infrastructure.

🌐 [amenophis.dev](https://amenophis.dev)

[X](https://x.com/amenophis1er) · [LinkedIn](https://www.linkedin.com/in/amenophis/) · [Threads](https://www.threads.com/@amenophis1er) · [Instagram](https://www.instagram.com/amenophis1er) · [Facebook](https://www.facebook.com/amenophis1er)

## Stack

**Languages:** Go · TypeScript · Rust · Python  
**Domains:** voice AI (STT/TTS/LLM streaming) · AI agents & MCP · developer tooling  
**Infra:** Cloudflare Workers · Docker · GitHub Actions · macOS/Linux

## Featured

- **[Shot Crisp](https://shotcrisp.app)** `Swift` — macOS screenshot studio — capture, annotate, OCR, pin, share; menu-bar native with an MCP bridge for agents.
- **[Vocito](https://vocito.app)** `Swift` — Dictation that types for you — push-to-talk voice typing for macOS. Talk naturally, false starts and all; Vocito types the sentence you meant, formatted for wherever you're writing. Private beta.
- **[My Notes — Side Panel Notepad](https://mynotes.amenophis.dev)** `TypeScript` — Local-first, Notion-like notes in the Chrome side panel — block editor, revision history, optional Drive/Dropbox sync.
- **[cadence](https://github.com/amenophis1er/cadence)** `Go` — Provider-agnostic Go engine for low-latency STT→LLM→TTS voice pipelines — streaming engines behind uniform interfaces, swap vendors with a config change. Owns the hot path.
- **[xPhone (Go version)](https://github.com/x-phone/xphone-go)** `Go` — Give your Go program a phone line. Dial out or answer calls on any SIP trunk — call audio arrives as PCM frames on a channel, ready to pipe into STT or a voice agent. No Asterisk, no per-minute API.
- **[Vonzio](https://github.com/vonzio/vonzio)** `TypeScript` — The runtime for production agents — bring your own model. Open-source, self-hostable, isolated Docker workspaces per session.
- **[elefante](https://github.com/amenophis1er/elefante)** `TypeScript` — The open, Git-native memory protocol for MCP agents: portable, inspectable, versioned, and human-editable.
- **[claude-voice](https://github.com/amenophis1er/claude-voice)** `TypeScript` — Give Claude Code a voice — selective, tasteful spoken summaries and attention cues. Quiet by default.

## Also building

- **[xbridge](https://github.com/x-phone/xbridge)** `Rust` — Phone calls for every other language: one self-hosted binary turns SIP calls into WebSocket audio + REST call control. Twilio-compatible framing, so existing voice apps port over with the URL swapped.
- **[xPhone (Rust version)](https://github.com/x-phone/xphone-rust)** `Rust` — The same phone line for Rust — SIP and RTP implemented from scratch, zero telephony crate dependencies. Call audio as crossbeam channels of PCM frames; powers xbridge in production.
- **[fakepbx](https://github.com/x-phone/fakepbx)** `Go` — In-process SIP server for Go tests. Real SIP over loopback — no Docker, no Asterisk, no hardcoded ports.
- **[xpbx](https://github.com/x-phone/xpbx)** `Go` — A real PBX in one docker run — Asterisk with a web UI for extensions, trunks and dialplans. The five-minute test bench for anything you build with xphone or xbridge.
- **[oxiclean](https://getoxiclean.com)** `Rust` — macOS storage cleaner — reclaims disk from package-manager caches, Docker artifacts, and orphaned app data. brew install getoxiclean/tap/oxiclean
- **[Trokky](https://github.com/Trokky)** `TypeScript` — Modern, composable CMS for developers — in private beta, with an open-source CLI for backup, restore, export and import.
- **[gh-setup](https://github.com/amenophis1er/gh-setup)** `Go` — Declaratively configure GitHub accounts, repos, and settings from a YAML file
- **[tts-bridge](https://github.com/amenophis1er/tts-bridge)** `Rust` — TTS APIs speak HTTP. Voice apps speak WebSocket. This bridges the gap.
- **[shopcart](https://github.com/amenophis1er/shopcart)** `TypeScript` — Save Amazon products to custom lists. Chrome extension for organizing your wishlist

## Writing

- [The anatomy of time-to-first-audio in a voice agent](https://amenophis.dev/writing/anatomy-of-first-audio/) — I measured my voice pipeline's wait — sentence buffer, VAD endpointing, and a live LLM→TTS chain. Post-commit, my code is ~14% of it; adding endpointing roughly doubles the share I control.
- [Giving AI agents a real phone line](https://amenophis.dev/writing/voice-agents-real-phone-line/) — A browser voice demo proves your model can talk. It doesn't prove your stack can survive a phone network — so I measured mine: frame-timing distributions at 50 concurrent calls, plus a live-trunk check.

---
<div align="center"><sub>This README is generated from a manifest — updated when I ship, not when I remember.</sub></div>
