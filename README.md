<div align="center">

# KenjaGrid

**Spreadsheets and data — an open-source, high-performance modern spreadsheet app, built in
pure Rust.** A fast, familiar, private-by-default spreadsheet: ribbon and formula bar, 500+
functions, dynamic arrays, pivot tables, charts and native XLSX — running natively on macOS,
Windows, Linux and BSD, and in the browser via WebAssembly.

*Your numbers. Your machine. No subscription.*

**[Privacy Policy](privacy.md)**

**Free and open source (MIT / Apache-2.0).**

</div>

---

KenjaGrid is a spreadsheet for people who just want their spreadsheet to work: the ribbon,
formula bar, Name Box, sheet tabs, fill handle and keyboard shortcuts are all right where you
expect them, and XLSX is the native format — styles, formulas (including dynamic arrays),
tables, conditional formats, charts, pictures, sparklines and pivot tables round-trip. A
dependency-graph calculation engine with incremental recalculation and a virtualised grid keeps
it fast; copy-on-write workbooks make undo snapshots nearly free. And it is agent-native: every
ribbon button, menu item and keystroke is a command an AI agent can run over an MCP server, the
CLI or a local JSON control channel. No accounts, no telemetry, no tracking; your workbooks
never leave your machine.

> "Kenja" is Japanese for *sage* — the wise one. Building smarter software is the mission.

## 中文介绍

**KenjaGrid 是一款开源、高性能的现代电子表格应用，用纯 Rust 构建**：功能区和编辑栏、500+
个工作表函数、动态数组、数据透视表、图表，原生 XLSX 双向往返——在 macOS、Windows、Linux、
BSD 上原生运行，并通过 WebAssembly 在浏览器中运行。快速（增量重算、虚拟化网格）、兼容
（XLSX 原生格式）、Agent 友好（MCP 服务器、CLI、本地 JSON 控制通道）。无账号、无遥测、
无追踪；工作簿从不出你的设备。

**[隐私政策](privacy.md)**

---

## Website (this repository)

This is the KenjaGrid product website / SEO repository. The privacy policy is
[`privacy.md`](privacy.md) — English · 简体中文 · 日本語 in one Markdown document; the site
serves its English rendering at `privacy.html`.

The site lives in `docs/`, matching the sibling KenjaPDF-site / KenjaDeck-site:

- Served by GitHub Pages from branch `main`, folder `/docs` (repo Settings → Pages):
  EN at `index.html`, 简体中文 at `zh.html`, 日本語 at `ja.html`, privacy at `privacy.html`,
  plus `CNAME`, `robots.txt`, `sitemap.xml` and `llms.txt`. Screenshots in `docs/assets/`
  are original screenshots made with KenjaGrid itself.
- DNS: `kenjagrid.kofukuai.com` CNAME → `KenjaHub.github.io`.
- Privacy policy URL (declared wherever the app is distributed):
  `https://kenjagrid.kofukuai.com/privacy.html`; marketing URL:
  `https://kenjagrid.kofukuai.com`.

---

© 2026 KenjaHub · [Privacy Policy](privacy.md) · [kenjasoft@kofukuai.com](mailto:kenjasoft@kofukuai.com)
