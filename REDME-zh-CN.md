# HYB (Hatch Your Beta) · 产品发布与分发控制台

> 🚀 为独立开发者与出海团队打造的多项目产品发布与增长分发工作台
>
> **无需登录 · 数据不上传 · 零依赖 · 开箱即用**

[English](./README.md) | **简体中文**

<p align="center">
  <img src="https://img.shields.io/badge/version-12.0-black" alt="Version">
  <img src="https://img.shields.io/badge/license-MIT-green" alt="License">
  <img src="https://img.shields.io/badge/storage-localStorage-orange" alt="Storage">
  <img src="https://img.shields.io/badge/i18n-中文%20%7C%20English-blue" alt="i18n">
  <img src="https://img.shields.io/badge/dependencies-0-brightgreen" alt="Dependencies">
  <img src="https://img.shields.io/badge/PRs-welcome-blueviolet" alt="PRs">
</p>

<p align="center">
  <a href="https://hyb.vip/">🌐 在线体验</a> ·
  <a href="#-功能特性">✨ 功能特性</a> ·
  <a href="#-快速开始">⚡ 快速开始</a> ·
  <a href="#-数据存储">💾 数据存储</a> ·
  <a href="#-贡献指南">🤝 贡献指南</a>
</p>

---

## 📖 简介

**HYB** 是一个**单文件、零依赖、纯前端**的产品发布与渠道分发控制台。

它将「发布物料管理」「500+ 获客渠道追踪」「冷启动进度记录」三件事整合到一个极简的本地工作台中。所有数据仅保存在你的浏览器 `localStorage` 中，**不上传任何服务器**，也**无需登录**。

打开即用，关闭即走，数据始终在你手里。

> **适合人群：** 独立开发者 (Indie Hackers)、SaaS 创始人、出海团队、内容创作者、产品运营。

---

## ✨ 功能特性

### 🗂 多项目物料库
- 每个产品独立保存 **产品名称 / 官网链接 / 一句话介绍 / 详细描述**
- 一键复制单字段或整套物料
- 项目级折叠展开，支持无限多项目并行管理

### 📊 数据概览面板
- **存活外链数** / **渠道总数** / **已操作渠道** / **已收录渠道** 实时统计
- 按项目分行显示小计，一眼看清每个产品的推进情况
- 自动本地保存，带时间戳提示

### 🎯 目标追踪 (OKR)
- 支持 **周 / 月 / 季度 / 年** 四种周期
- 每个项目独立设置目标分发数量
- 进度条 + 剩余天数 + 智能教练提示（根据不同状态给出不同建议）
- 自动按外链发布日期统计达成数量

### 🌐 增长渠道库 (500+ Channels)
预置 500+ 真实获客渠道，涵盖：

| 分类 | 示例 |
|------|------|
| AI 工具目录 | There's An AI For That、Futurepedia、Toolify |
| SaaS 软件评测 | G2、Capterra、TrustRadius、GoodFirms |
| 产品发布创业 | Product Hunt、BetaList、Indie Hackers、Uneed |
| 开发者技术 | GitHub、Hacker News、Dev.to、Stack Overflow |
| 社交内容平台 | X、LinkedIn、Reddit、Medium、YouTube |
| 社区推广 | r/SideProject、r/indiehackers、Growth Hackers |
| 商业企业PR | Crunchbase、G2、Yelp、BBB |
| 搜索引擎 | Google、Bing、Yandex、百度、Naver |
| 其他渠道 | 大量小众目录、AI 导航站、开发者社区 |

每个渠道内置 **DR 域名权重** 数据，可按 DR 升降序排序；点击 DR 值可手动编辑。

### 📋 分发进度管理
对「渠道 × 项目」每个组合都可独立记录：

- **状态**：待发布 → 已发布 → 已收录 / 被拒绝
- **跟进日期**：自动识别逾期并高亮
- **上线地址**：每条外链可记录 URL + 标题 + 发布日期
- **备注**：为每条渠道写操作心得

### 🔍 强大筛选与搜索
- 按项目 / 分类 / 状态 / 费用 / 关键词筛选
- DR 单独作为排序维度，不参与筛选
- 某渠道所有项目行被筛掉时自动隐藏

### 🌍 双语界面
- 简体中文 / English 一键切换
- 界面文案完整 i18n，切换后自动持久化

### 💾 导入导出
- 导出全部数据为 JSON 备份
- 支持导入备份、迁移旧版数据、旧版 V10 数据结构

### 🎨 极简设计
- 黑白灰极简风格，无多余装饰
- 响应式布局，桌面 / 平板 / 手机均可用
- 零 CSS 框架依赖，无 JS 库依赖

---

## ⚡ 快速开始

### 方式一：在线使用（推荐）

直接访问 👉 **[https://hyb.vip/](https://hyb.vip/)**

### 方式二：本地运行

```bash
# 克隆仓库
git clone https://github.com/ffeeme/hyb.git
cd hyb

# 直接用浏览器打开 index.html
open index.html          # macOS
start index.html         # Windows
xdg-open index.html      # Linux
💡 由于使用 localStorage，建议通过本地服务器访问以获得完整体验：

bash
# 任选其一
python3 -m http.server 8080
npx serve .
php -S localhost:8080
然后访问 http://localhost:8080。

方式三：部署到静态托管
本项目是单个 HTML 文件，可直接部署到：

✅ Vercel / Netlify / Cloudflare Pages

✅ GitHub Pages

✅ 任意静态服务器 / 对象存储

💾 数据存储
HYB 采用 local-first 架构，所有数据均保存在你的浏览器中：

Key	内容
hyb_v12_platforms	渠道列表（含自定义渠道）
hyb_v12_projects	项目物料库
hyb_v12_progress	每个「渠道 × 项目」的进度记录
hyb_v12_okr	每个项目独立的目标设置
hyb_v12_lang	语言偏好
hyb_v12_ui	界面折叠状态
hyb_v12_saved_at	最后保存时间
⚠️ 注意事项
数据不会同步到任何服务器，仅存在于当前浏览器

清除浏览器数据 / 更换设备 / 使用无痕模式 → 数据会丢失

强烈建议定期使用「导出」功能备份数据

不同浏览器 / 不同域名下的数据相互独立

🗺 路线图
☑ 500+ 预置渠道库
☑ 多项目物料管理
☑ 多渠道 × 多项目进度矩阵
☑ OKR 目标追踪
☑ 双语界面
☑ 数据导入导出
☑ DR 权重排序与编辑
□ 外链存活检测（自动 check 链接可达性）
□ 数据可视化图表（按周/月趋势）
□ 渠道推荐（根据产品类型推荐匹配渠道）
□ PWA 离线安装
□ 云端同步（可选账号）
🤝 贡献指南
我们欢迎任何形式的贡献！无论是：

🐛 报告 Bug

💡 提出新功能建议

📝 改进文档

🔧 提交代码

🧩 补充优质渠道到内置列表

提交 PR 流程
bash
# 1. Fork 本仓库
# 2. 创建分支
git checkout -b feature/your-feature-name

# 3. 提交改动
git commit -m "feat: add your feature"

# 4. 推送
git push origin feature/your-feature-name

# 5. 提交 Pull Request
提交 Issue
提交 Issue 前请先搜索是否已有相同问题。请包含：

问题描述

复现步骤

浏览器版本 / 操作系统

截图或录屏（如有）

添加渠道
想为内置渠道库贡献新渠道？请编辑 index.html 中的 REAL_PLATFORMS 数组，确保：

name 唯一

url 使用 https://

category 属于预设分类之一

如有 DR 数据，可补充到 PRELOADED_DR 对象

📄 许可证
本项目基于 MIT License 开源，可自由用于个人或商业项目。

🔗 相关链接
🌐 官网：https://hyb.vip/

🐙 GitHub：https://github.com/ffeeme/hyb

🐦 X (Twitter)：@xYCV8jRRrs4uBvC

📺 YouTube：@hyb-vip

📖 使用指南：https://www.hyb.vip/#faq

🔒 隐私政策：https://www.hyb.vip/privacy-policy/

⭐ Star History
如果这个项目对你有帮助，请给个 Star ⭐ 支持一下！

<p align="center"> <a href="https://star-history.com/#ffeeme/hyb&Date"> <img src="https://api.star-history.com/svg?repos=ffeeme/hyb&type=Date" alt="Star History Chart"> </a> </p>
<p align="center"> <strong>HYB · Hatch Your Beta</strong><br> <em>让每一次发布，都有迹可循。</em> </p><p align="center"> Made with 🖤 for indie hackers worldwide. </p> ```
