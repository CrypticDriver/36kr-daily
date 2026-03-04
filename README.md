# 🌅 科技早报 - 每日自动聚合

每天北京时间 08:00 自动抓取、生成的科技新闻早报。

由 Kuro 🖤 自动生成，基于 OpenClaw + openclaw-feeds skill。

---

## 📰 信息源

通过 **openclaw-feeds** skill 聚合多个优质科技媒体：

### 国际媒体
- **Wired** - 科技深度报道
- **TechCrunch** - 创投与科技新闻
- **The Verge** - 科技与文化
- **Ars Technica** - 技术分析
- **Slashdot** - 技术社区

### 专业内容
- **Quanta Magazine** - 科学与数学
- **Symmetry Magazine** - 粒子物理
- **Aeon** - 思想与文化
- **Nautilus** - 科学与人文

---

## 📂 报告位置

所有日报存储在 [`/reports`](./reports) 目录：

- 文件名格式：`YYYY-MM-DD.md`
- 每日 50 篇精选文章
- 按来源分组展示

**最新报告：** [查看今日早报](./reports)

---

## 🤖 技术栈

- **信息源聚合**: openclaw-feeds skill（RSS 并发抓取）
- **调度**: Linux Cron（每天 UTC 00:00 = 北京时间 08:00）
- **部署**: 隔离环境执行
- **存储**: GitHub（自动 commit + push）

---

## 📊 特点

✅ **自动化**：每天自动运行，无需人工干预  
✅ **多源聚合**：25+ 优质科技媒体  
✅ **实时更新**：抓取当天最新文章  
✅ **版本控制**：GitHub 自动存档  
✅ **零成本**：无需 API key，直接读取公开 RSS

---

## 🔧 本地运行

```bash
# 克隆仓库
git clone https://github.com/CrypticDriver/36kr-daily.git
cd 36kr-daily

# 查看报告
ls reports/
cat reports/2026-03-04.md
```

---

## 📝 示例报告

```markdown
# 🌅 科技早报

**日期：** 2026-03-04
**来源：** openclaw-feeds（Wired, TechCrunch, Slashdot 等）
**文章数：** 50 篇精选

---

## 📰 今日热点

### Father sues Google, claiming Gemini chatbot drove son into fatal delusion
**来源：** techcrunch.com | **时间：** Wed, 04 Mar 2026 14:58:36 +0000

A father is suing Google and Alphabet, alleging its Gemini chatbot...

🔗 [阅读原文](https://techcrunch.com/...)

---

### MacBook Neo, Apple's colorful answer to the Chromebook, starting at $599
**来源：** techcrunch.com | **时间：** Wed, 04 Mar 2026 14:57:17 +0000

Apple is offering the MacBook Neo at a more affordable price point...

🔗 [阅读原文](https://techcrunch.com/...)
```

---

## 📮 反馈

有建议或发现问题？欢迎提 Issue！

---

## 🛠️ 系统架构

```
openclaw-feeds skill
      ↓
  抓取 RSS feeds（25+ 源）
      ↓
  提取前 50 篇
      ↓
  生成 Markdown 报告
      ↓
  上传到 GitHub
      ↓
  Discord 通知（heartbeat）
```

---

*自动化工作流由 Kuro 🖤 创建和维护*

**GitHub：** https://github.com/CrypticDriver/36kr-daily  
**Skill：** [openclaw-feeds](https://github.com/arc-claw-bot/openclaw-feeds)
