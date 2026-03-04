# 🌅 科技早报 · AI 智能精选

每天北京时间 08:00 自动抓取、分析的科技新闻早报。

**双引擎智能聚合：**
- 📰 **RSS Feeds** - 25+ 优质科技媒体
- 🔍 **Tavily Real-time Search** - AI 驱动的实时热点搜索

由 Kuro 🖤 智能生成，基于 OpenClaw + openclaw-feeds + Tavily AI Search。

---

## 🚀 核心特性

### **双引擎信息源**

**1. RSS Feeds（广度覆盖）**
- Wired、TechCrunch、The Verge、Ars Technica
- Slashdot、Hacker News、Quanta Magazine
- 25+ 优质科技媒体并发抓取

**2. Tavily AI Search（实时热点）**
- AI 大模型动态（ChatGPT、Claude、Gemini）
- Web3 区块链与加密货币
- 科技创业、融资、IPO
- OpenClaw 与 AI Agent 生态

---

## 📂 报告结构

每日报告包含：

```markdown
# 🌅 科技早报 · 智能精选

## 🔥 今日热点（Tavily 实时搜索）
- 4 个主题的实时搜索结果
- AI 生成的摘要
- 相关度排序的来源链接

## 📰 RSS 精选文章（前 30 篇）
- 标题、来源、时间
- 文章摘要
- 原文链接
```

**查看示例：** [2026-03-04 报告](./reports/2026-03-04.md)

---

## 🎯 信息源详解

### **RSS Feeds（875+ 篇/天）**

| 媒体类型 | 代表媒体 | 内容特点 |
|---------|---------|---------|
| 科技深度 | Wired, Ars Technica | 技术分析、产品评测 |
| 创投新闻 | TechCrunch | 融资、创业、商业 |
| 技术社区 | Hacker News, Slashdot | 程序员视角、技术讨论 |
| 科学前沿 | Quanta Magazine, Symmetry | 科学研究、物理学 |
| 思想文化 | Aeon, Nautilus | 科技与人文 |

### **Tavily AI Search（实时）**

**搜索主题：**
1. **AI 大模型** - ChatGPT, Claude, Gemini 最新动态
2. **Web3 生态** - 区块链、加密货币、DeFi
3. **科技创业** - 融资、IPO、独角兽
4. **AI Agent** - OpenClaw 及相关生态

**Tavily 优势：**
- ✅ 专为 AI agent 设计
- ✅ 返回 AI 优化的摘要
- ✅ 相关度评分和排序
- ✅ 自动去噪和过滤

---

## 🤖 技术架构

```
                    ┌─────────────────┐
                    │  Cron Scheduler │
                    │  (Daily 08:00)  │
                    └────────┬────────┘
                             │
                ┌────────────┴────────────┐
                │                         │
         ┌──────▼──────┐          ┌──────▼──────┐
         │ RSS Feeds   │          │   Tavily    │
         │ (875 篇)    │          │  AI Search  │
         └──────┬──────┘          └──────┬──────┘
                │                         │
                └────────────┬────────────┘
                             │
                    ┌────────▼────────┐
                    │  Smart Digest   │
                    │  (Analysis +    │
                    │   Formatting)   │
                    └────────┬────────┘
                             │
                    ┌────────▼────────┐
                    │  GitHub Push    │
                    └────────┬────────┘
                             │
                    ┌────────▼────────┐
                    │ Discord Notify  │
                    └─────────────────┘
```

### **技术栈：**
- **信息聚合**: openclaw-feeds (RSS) + Tavily AI Search
- **调度**: Linux Cron（每天 UTC 00:00 = 北京时间 08:00）
- **处理**: Bash + Node.js + jq
- **存储**: GitHub（自动 commit + push）
- **通知**: Discord（heartbeat）

---

## 📊 数据统计

- **RSS 来源**: 25+ 科技媒体
- **RSS 文章量**: 875+ 篇/天
- **Tavily 主题**: 4 个热点方向
- **精选输出**: ~35 篇（Tavily 实时 + RSS 精选）
- **更新频率**: 每日 1 次
- **零成本**: 无需付费 API（Tavily 免费开发版）

---

## 🔧 本地运行

```bash
# 克隆仓库
git clone https://github.com/CrypticDriver/36kr-daily.git
cd 36kr-daily

# 查看最新报告
cat reports/2026-03-04.md

# 浏览所有报告
ls reports/
```

---

## 🎨 报告示例

### **Tavily 实时热点**
```markdown
### 主题：AI大模型 ChatGPT Claude Gemini

ChatGPT、Claude、Gemini 等主流 AI 模型持续演进...

**来源：**
- AI大模型全景解析（相关度：100%）
- ChatGPT vs Claude 对比分析（相关度：100%）
```

### **RSS 精选文章**
```markdown
### The $599 MacBook Neo is Apple's colorful MacBook

**来源：** arstechnica.com | **时间：** 2026-03-04

Cute, colorful laptop takes the place of the old $599 M1 MacBook Air.

🔗 [阅读原文](https://arstechnica.com/...)
```

---

## 🔮 未来计划

- [ ] AI 自动总结（每日 Top 5 核心价值）
- [ ] 多语言支持（中英双语）
- [ ] 自定义搜索主题
- [ ] 邮件订阅
- [ ] 历史趋势分析

---

## 📮 反馈

有建议或发现问题？欢迎提 Issue！

---

*自动化工作流由 Kuro 🖤 创建和维护*

**GitHub：** https://github.com/CrypticDriver/36kr-daily  
**Skills：**
- [openclaw-feeds](https://github.com/arc-claw-bot/openclaw-feeds)
- [Tavily AI Search](https://tavily.com)
