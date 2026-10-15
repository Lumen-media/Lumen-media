<p align="center">
  <img src="https://raw.githubusercontent.com/Lumen-media/lumen/main/public/logo.png" alt="Lumen" width="120" />
</p>

<h1 align="center">Lumen Media</h1>

<p align="center">
  <strong>The control room for your live event.</strong>
</p>

<p align="center">
  Media management software for churches and live events — built for simplicity, performance, and extensibility.
</p>

<p align="center">
  <a href="https://github.com/Lumen-media/lumen/releases"><img alt="Latest Release" src="https://img.shields.io/github/v/release/Lumen-media/lumen?label=Latest%20Release&style=for-the-badge" /></a>
  <a href="https://github.com/Lumen-media/lumen/blob/main/LICENSE"><img alt="License" src="https://img.shields.io/github/license/Lumen-media/lumen?style=for-the-badge" /></a>
  <a href="https://github.com/Lumen-media/lumen/stargazers"><img alt="Stars" src="https://img.shields.io/github/stars/Lumen-media/lumen?style=for-the-badge" /></a>
  <a href="https://github.com/Lumen-media/lumen/issues"><img alt="Issues" src="https://img.shields.io/github/issues/Lumen-media/lumen?style=for-the-badge" /></a>
</p>

---

## 🎬 What is Lumen?

**Lumen** is a desktop application that puts everything you need to run a live event in one window: lyrics, slides, media playback, live camera feeds, team chat, and remote control from any phone — all over your local network.

Designed for operators who need to drive a show with one hand while talking. No frozen decks, no second laptop, no internet required.

<p align="center">
  <img src="https://raw.githubusercontent.com/Lumen-media/lumen/main/public/screenshot-main.png" alt="Lumen Screenshot" width="800" />
</p>

---

## 🏗️ Architecture

| Layer | Technology |
|-------|------------|
| **Desktop Shell** | Tauri 2 (Rust) |
| **Interface** | React 19, TypeScript, Tailwind CSS 4 |
| **Build** | Vite + SWC, pnpm workspaces |
| **Routing & State** | TanStack Router, TanStack Query, Zustand |
| **Editing** | TipTap, TanStack Markdown, TanStack Virtual |
| **Playback & Media** | React Player; yt-dlp + FFmpeg (managed by app) |
| **Imaging** | Rust thumbnail cache, `lumen://` protocol |
| **Live & Remote** | WebRTC, WebSocket, built-in HTTP server |
| **Storage** | SQLite, Tauri plugins |
| **i18n** | 6 locales, over-the-air updates |

---

## 📦 Repositories

| Repository | Description |
|------------|-------------|
| **[lumen](https://github.com/Lumen-media/lumen)** | Main desktop application |
| **[module-sdk](https://github.com/Lumen-media/module-sdk)** | SDK for building Lumen modules |
| **[community-modules](https://github.com/Lumen-media/community-modules)** | Catalog of community-contributed modules |
| **[lumen-locales](https://github.com/Lumen-media/lumen-locales)** | Translation strings with OTA updates |

---

## 🧩 Module Ecosystem

Lumen is a **shell** — functionality lives in modules. Install from the in-app Module Store:

| Module | Description |
|--------|-------------|
| **Countdown Timer** | Full-featured countdowns with triggers |
| **YouTube Search** | Search and queue videos without leaving Lumen |
| **Bible Reader** | Multi-version Bible with slide export |
| **Raffle** | Random pickers for events |

[Build your own module →](https://github.com/Lumen-media/module-sdk)

---

## 🚀 Quick Start

### For Users
1. Download the latest **Windows** or **Linux** installer from [Releases](https://github.com/Lumen-media/lumen/releases)
2. Drop media into the library — Lumen creates the folder structure on first run
3. Open a lyric or import `.pptx`, press **F5** to send to output
4. Scan the QR code in **Settings → Remote Access** to pair your phone

### For Developers
```bash
git clone https://github.com/Lumen-media/lumen.git
cd lumen
pnpm install
pnpm tauri dev
```

Requires: Node.js, pnpm, Rust toolchain. Optional: `VITE_UNSPLASH_CLIENT_ID` in `.env` for background search.

---

## 📚 Documentation

| Guide | Link |
|-------|------|
| Presenter Guide | [`docs/presenter-usage.md`](https://github.com/Lumen-media/lumen/blob/main/docs/presenter-usage.md) |
| Remote Access & Device Protocol | [`docs/websocket-access-api.md`](https://github.com/Lumen-media/lumen/blob/main/docs/websocket-access-api.md) |
| Module API Reference | [`docs/module-api-reference.md`](https://github.com/Lumen-media/lumen/blob/main/docs/module-api-reference.md) |
| Architecture Decisions | [`docs/architecture/`](https://github.com/Lumen-media/lumen/tree/main/docs/architecture) |

---

## 🤝 Contributing

Issues and PRs welcome! Please use the issue templates in `.github/`. Feature-labelled issues from non-maintainers are auto-redirected to keep the roadmap focused.

---

## 📄 License

[Apache-2.0](https://github.com/Lumen-media/lumen/blob/main/LICENSE) © 2026 Gabriel Santos. Use it, fork it, ship it — just keep the notice, and don't use the Lumen name or logo to endorse something that isn't us. See [NOTICE](https://github.com/Lumen-media/lumen/blob/main/NOTICE).

---

<p align="center">
  Made with ❤️ for churches and live event teams everywhere.
</p>

<p align="center">
  <a href="https://github.com/Lumen-media/lumen">Main App</a> •
  <a href="https://github.com/Lumen-media/module-sdk">Module SDK</a> •
  <a href="https://github.com/Lumen-media/community-modules">Community Modules</a> •
  <a href="https://github.com/Lumen-media/lumen/releases">Releases</a>
</p>