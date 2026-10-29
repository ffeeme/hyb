# HYB (Hatch Your Beta) · Product Launch & Growth Distribution Console

> 🚀 A local-first, multi-project launch workspace for indie hackers and SaaS founders.
>
> **No login · No server upload · Zero dependencies · Ready to use**

**English** | [简体中文](./README.zh-CN.md)

<p align="center">
  <img src="https://img.shields.io/badge/version-12.0-black" alt="Version">
  <img src="https://img.shields.io/badge/license-MIT-green" alt="License">
  <img src="https://img.shields.io/badge/storage-localStorage-orange" alt="Storage">
  <img src="https://img.shields.io/badge/i18n-English%20%7C%20中文-blue" alt="i18n">
  <img src="https://img.shields.io/badge/dependencies-0-brightgreen" alt="Dependencies">
  <img src="https://img.shields.io/badge/PRs-welcome-blueviolet" alt="PRs">
</p>

<p align="center">
  <a href="https://hyb.vip/">🌐 Live Demo</a> ·
  <a href="#-features">✨ Features</a> ·
  <a href="#-quick-start">⚡ Quick Start</a> ·
  <a href="#-data-storage">💾 Data Storage</a> ·
  <a href="#-contributing">🤝 Contributing</a>
</p>

---

## 📖 Introduction

**HYB** is a **single-file, zero-dependency, pure frontend** console for product launches and channel distribution.

It brings three things together in one minimal local workspace:

- **Launch materials management** — keep your product copy ready to paste
- **500+ acquisition channel tracking** — the full GTM distribution stack
- **Cold start progress recording** — every placement, every date, every note

All data is stored **only in your browser's `localStorage`**. Nothing is uploaded. No account required.

Open it, use it, close it — your data stays with you.

> **Built for:** indie hackers, SaaS founders, global launch teams, content creators, and product marketers.

---

## ✨ Features

### 🗂 Multi-Project Materials Library
- Each product keeps its own **name / website / tagline / description**
- One-click copy for a single field or the entire material set
- Collapsible project cards, unlimited projects in parallel

### 📊 Overview Dashboard
- **Live Placements** / **Total Channels** / **Launched** / **Featured** — real-time stats
- Per-project breakdown so you can see each product's progress at a glance
- Auto-saved locally with a timestamp

### 🎯 Goal Tracking (OKR)
- Supports **weekly / monthly / quarterly / yearly** cycles
- Independent target per project
- Progress bar + days remaining + smart coach messages that adapt to your pace
- Automatically counts placements by their launch date

### 🌐 500+ Growth Channels
Pre-loaded with 500+ real acquisition channels, including:

| Category | Examples |
|----------|----------|
| AI Tool Directories | There's An AI For That, Futurepedia, Toolify |
| SaaS Reviews | G2, Capterra, TrustRadius, GoodFirms |
| Launch & Startup | Product Hunt, BetaList, Indie Hackers, Uneed |
| Developer Tools | GitHub, Hacker News, Dev.to, Stack Overflow |
| Social & Content | X, LinkedIn, Reddit, Medium, YouTube |
| Community Promotion | r/SideProject, r/indiehackers, Growth Hackers |
| Business & PR | Crunchbase, G2, Yelp, BBB |
| Search Engines | Google, Bing, Yandex, Baidu, Naver |
| Other Channels | Tons of niche directories, AI navigators, dev communities |

Each channel ships with a **DR (Domain Rating)** value. Sort by DR ascending or descending, and click any DR value to edit it manually.

### 📋 Distribution Progress
For every **channel × project** combination, track:

- **Status**: Pending → Launched → Featured / Rejected
- **Follow-up date**: overdue rows are automatically highlighted
- **Live URLs**: each placement can record URL + title + launch date
- **Notes**: freeform notes per channel

### 🔍 Powerful Filtering
- Filter by project / category / status / fee / keyword
- DR is a **sort dimension only** — it never filters
- Channels are hidden when all their project rows are filtered out

### 🌍 Bilingual UI
- Switch between **English / 简体中文** instantly
- Full i18n coverage, preference persisted automatically

### 💾 Import & Export
- Export everything as a JSON backup
- Import backups, migrate legacy data, support old V10 data structures

### 🎨 Minimal Design
- Clean black / white / grey aesthetic, no clutter
- Responsive — works on desktop, tablet, and mobile
- No CSS framework, no JS library

---

## ⚡ Quick Start

### Option 1: Use it online (recommended)

👉 **[https://hyb.vip/](https://hyb.vip/)**

### Option 2: Run locally

```bash
# Clone the repo
git clone https://github.com/ffeeme/hyb.git
cd hyb

# Open it in your browser
open index.html          # macOS
start index.html         # Windows
xdg-open index.html      # Linux
💡 Because the app uses localStorage, we recommend serving it through a local server:

bash
# Pick one
python3 -m http.server 8080
npx serve .
php -S localhost:8080
Then open http://localhost:8080.

Option 3: Deploy to static hosting
This project is a single HTML file — deploy it anywhere:

✅ Vercel / Netlify / Cloudflare Pages

✅ GitHub Pages

✅ Any static server or object storage

💾 Data Storage
HYB uses a local-first architecture. All data lives in your browser:

Key	Content
hyb_v12_platforms	Channel list (including custom channels)
hyb_v12_projects	Project materials
hyb_v12_progress	Per channel × project progress
hyb_v12_okr	Per-project goal settings
hyb_v12_lang	Language preference
hyb_v12_ui	UI collapse state
hyb_v12_saved_at	Last saved timestamp
⚠️ Important
Data is never synced to any server — it stays in your current browser

Clearing browser data / changing devices / incognito mode → data is lost

Back up regularly using the "Export" button

Data is isolated per browser and per domain

🗺 Roadmap
☑ 500+ preloaded channels
☑ Multi-project materials
☑ Channel × project progress matrix
☑ OKR goal tracking
☑ Bilingual UI
☑ JSON import / export
☑ DR sorting & inline editing
□ Live link health check
□ Visual charts (weekly / monthly trends)
□ Channel recommendations based on product type
□ PWA offline install
□ Optional cloud sync
🤝 Contributing
Contributions of any kind are welcome:

🐛 Report bugs

💡 Suggest new features

📝 Improve docs

🔧 Submit code

🧩 Add quality channels to the built-in list

PR workflow
bash
# 1. Fork this repo
# 2. Create a branch
git checkout -b feature/your-feature-name

# 3. Commit your changes
git commit -m "feat: add your feature"

# 4. Push
git push origin feature/your-feature-name

# 5. Open a Pull Request
Opening an issue
Please search for existing issues first. Include:

Description of the problem

Steps to reproduce

Browser version / OS

Screenshots or recordings (if applicable)

Adding a channel
Want to contribute a channel to the built-in list? Edit the REAL_PLATFORMS array in index.html. Please ensure:

name is unique

url uses https://

category is one of the preset categories

Optionally add DR data to the PRELOADED_DR object

📄 License
Released under the MIT License. Free for personal and commercial use.

🔗 Links
🌐 Website: https://hyb.vip/

🐙 GitHub: https://github.com/ffeeme/hyb

🐦 X (Twitter): @xYCV8jRRrs4uBvC

📺 YouTube: @hyb-vip

📖 User Guide: https://www.hyb.vip/#faq

🔒 Privacy Policy: https://www.hyb.vip/privacy-policy/

⭐ Star History
If this project helps you, please give it a star ⭐ — it means a lot!

<p align="center"> <a href="https://star-history.com/#ffeeme/hyb&Date"> <img src="https://api.star-history.com/svg?repos=ffeeme/hyb&type=Date" alt="Star History Chart"> </a> </p>
<p align="center"> <strong>HYB · Hatch Your Beta</strong><br> <em>Make every launch count.</em> </p><p align="center"> Made with 🖤 for indie hackers worldwide. </p> ```
