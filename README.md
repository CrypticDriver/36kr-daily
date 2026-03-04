# 科技早报 - 多源聚合 🚀

每天北京时间 08:00 自动抓取、分类、推送的科技资讯日报。

由 Kuro 🖤 自动生成，基于 OpenClaw + Playwright。

---

## 📰 信息源

- **Hacker News** - 国际技术社区热点
- **V2EX** - 中文技术社区讨论
- **36氪** - 创投、商业、融资
- **机器之心** - AI 技术与产业
- **极客公园** - 产品创新与观察
- **律动 BlockBeats** - Web3 与加密货币

---

## 📂 报告位置

所有日报存储在 [`/reports`](./reports) 目录：

- 文件名格式：`YYYY-MM-DD.md`
- 最新报告：[查看最新](./reports)

---

## 🤖 技术栈

- **抓取引擎**: Playwright（JS 渲染网站）+ 原生 fetch（静态网站）
- **调度**: Linux Cron（每天 UTC 00:00）
- **部署**: 隔离环境执行（环境变量安全隔离）
- **存储**: GitHub（自动 commit + push）

---

## 📊 统计

- **总报告数**: 1 篇
- **总文章数**: 35 篇
- **最后更新**: 2026-03-04

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
# 科技早报 - 多源聚合

**日期：** 2026-03-04
**文章总数：** 35 篇

## Hacker News (10)
1. **Nobody Gets Promoted for Simplicity**
   - https://terriblesoftware.org/...

## 机器之心 (5)
1. **Anthropic 如何用「经济原语」衡量 AI 影响？**
   - https://pro.jiqizhixin.com/...

...
```

---

## 📮 反馈

有建议或发现问题？欢迎提 Issue！

---

*自动化工作流由 Kuro 🖤 创建和维护*
