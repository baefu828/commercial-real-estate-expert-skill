# 商业地产招商运营专家 Skill

![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)
![Version](https://img.shields.io/badge/version-1.0.0-green.svg)
![Skill Format](https://img.shields.io/badge/format-Agent%20Skills-orange.svg)

> **English**: Commercial Real Estate Leasing & Operations Expert Skill — 12 years of hands-on experience in industrial parks, office buildings, and commercial districts.

---

## 📖 项目简介

本 Skill 将 **12 年商业地产招商运营实战经验**封装为标准 Agent Skills 格式，可被 WorkBuddy、Claude Code、Cursor 等 AI 编程/对话工具直接加载使用。

无论你是：
- 🏢 **商业地产从业者**：需要快速查阅招商/催缴/合同/政策等专业内容
- 🤖 **AI 应用开发者**：希望为你的 Agent 集成商业地产领域专业能力
- 📚 **运营/招商团队**：想用 AI 辅助日常决策与方案输出

都能从这个 Skill 中获益。

## 🎯 核心能力

| 领域 | 关键能力 | 代表数据 |
|------|--------|--------|
| **招商拓展** | 渠道搭建、品牌落位、租金定价 | 10个月 95% 招商率；引入星巴克/瑞幸/7-11 等 12+ 品牌 |
| **收缴攻坚** | 分级催收、诉讼推进、风险预警 | 收缴率 95%-98%；累计追回欠缴 37 万 |
| **筹开运营** | 交付倒排、承接查验、商户进场 | 疫情期间保障 43 家商户按期开业 |
| **产业服务** | 孵化器申报、产业 IP 引入 | 单年落地活动 112 场、8000 人次 |
| **政策申报** | 国高/市高、补贴申报 | 累计获补 375+ 万 |
| **标准化建设** | 运营手册、SOP 编写 | 主导万科上海区域商办运营服务手册 |

详细能力清单见 [SKILL.md](./SKILL.md)。

## 📂 仓库内容

```
commercial-real-estate-expert-skill/
├── SKILL.md                          ⭐ 统一入口（人设+能力+知识库索引）
├── README.md                         项目说明（本文件）
├── LICENSE                           MIT 协议
├── CHANGELOG.md                      版本变更日志
├── CONTRIBUTING.md                   贡献指南
├── assets/avatar.png                 专家头像
├── references/                       10 个知识库模块
│   ├── collection-strategy.md        催缴策略（10步时间线+集团6步+实战数据）
│   ├── contract-review-points.md     合同审阅（12维清单+16条速查）
│   ├── industry-insights.md          行业洞察（82篇2025-2026深度文章）
│   ├── leasing-strategy.md           招商策略（渠道+实战KPI+商户案例）
│   ├── merchant-rating-system.md     商户星级评定（五维度100分）
│   ├── policy-database.md            政策申报（杭州市/区矩阵）
│   ├── property-management-standards.md  物业标准（46项表单）
│   ├── rent-benchmark.md             租金基准（杭州各区参考）
│   ├── startup-checklist.md          筹开管理（进场/装修/撤场/巡检）
│   └── vanke-ops-system.md           万科营运（49份制度提炼）
├── templates/                        3 个工具模板
│   ├── 催缴函模板.md
│   ├── 验房承接查验清单.md
│   └── 筹开倒排计划模板.md
└── .github/workflows/validate.yml    CI 校验
```

## 🚀 快速开始

### 方式 1：在 WorkBuddy 中使用

将仓库克隆到 Skills 目录：

```bash
git clone https://github.com/baefu828/commercial-real-estate-expert-skill.git \
  ~/.workbuddy/skills/commercial-real-estate-expert
```

重启 WorkBuddy 后，Skill 会自动出现在可用 Skill 列表中。

### 方式 2：在 Claude Code / Cursor 中使用

直接指向 SKILL.md 即可：

```bash
# Claude Code（在你的项目目录）
git clone https://github.com/baefu828/commercial-real-estate-expert-skill.git
claude --skills ./commercial-real-estate-expert-skill
```

### 方式 3：手动加载

将 `SKILL.md` 内容作为系统提示词前缀注入到任何支持 Markdown 文档加载的 Agent 框架中。

## 💡 使用示例

### 示例 1：项目筹开方案
```
我手上有一个 5 万㎡的产业园项目，从拿房到开业只有 8 个月，
帮我出一份从 0 到 1 的筹开倒排计划。
```
→ AI 会加载 `references/startup-checklist.md` 和 `templates/筹开倒排计划模板.md`，输出可落地的倒排表。

### 示例 2：租户催收
```
某租户已欠租 3 个月，金额 18 万，沟通多次无果，
如何分级推进催缴并准备诉讼？
```
→ AI 会加载 `references/collection-strategy.md` 和 `templates/催缴函模板.md`，给出分级催收+律师函+诉讼推进的完整方案。

### 示例 3：合同风险排查
```
帮我审阅这份商业租赁合同，重点排查租金/物业费/保证金条款的风险点。
```
→ AI 会加载 `references/contract-review-points.md`，按 12 维清单逐项核对。

### 示例 4：政策申报路径
```
我们园区有 12 家科技型中小企业，今年想申请市级高新技术企业和孵化器认定，
需要准备哪些材料、走什么流程？
```
→ AI 会加载 `references/policy-database.md`，给出杭州市/区各级申报矩阵和材料清单。

## ⚠️ 使用须知

本 Skill 提供的内容**仅供专业参考**，实际应用中请注意：

- 📈 **行情相关**：租金定价、招商政策等会因城市/区域/时间不同而异，请结合当地实际调整
- ⚖️ **法律相关**：涉及合同条款解释、诉讼推进等问题，请咨询专业律师
- 🏛️ **政策时效**：政策申报内容会随时间变化，请以最新政策文件为准
- 🎯 **特殊业态**：医疗、教育、宗教等特殊业态规范，超出本 Skill 覆盖范围

## 🤝 贡献

欢迎补充更多知识库内容、修复错误、改善文档！详见 [CONTRIBUTING.md](./CONTRIBUTING.md)。

提交 PR 前请确保：
- Markdown 格式规范（CI 会自动校验）
- 同步更新 `SKILL.md` 中的"知识库索引"章节（如新增/重命名 reference）
- 在 `CHANGELOG.md` 的 `Unreleased` 段落记录变更

## 📜 许可证

[MIT](./LICENSE) — 自由使用、修改、分发，需保留版权声明。

## 🙏 致谢

本 Skill 由 [@baefu828](https://github.com/baefu828) 基于 12 年商业地产招商运营实战经验整理发布。

如有问题或建议，请在 GitHub Issues 区提交。

---

**English version follows / 英文版本如下**

---

# Commercial Real Estate Expert Skill

A standard Agent Skills format Skill encapsulating **12 years of hands-on commercial real estate leasing & operations experience** across industrial parks, office buildings, and commercial districts. Compatible with WorkBuddy, Claude Code, Cursor, and other AI agent frameworks.

## Quick Start

```bash
git clone https://github.com/baefu828/commercial-real-estate-expert-skill.git
```

Load `SKILL.md` as the entry point. Sub-files under `references/` and `templates/` are loaded on demand based on trigger keywords.

## Core Capabilities

- **Leasing & Investment Promotion**: channel building, brand placement, rent pricing — 95% occupancy in 10 months
- **Rent Collection**: tiered collection, legal escalation, risk alerting — 95-98% collection rate
- **Project Startup**: delivery countdown, handover inspection, tenant onboarding
- **Industry Services**: incubator applications, IP introduction, community building
- **Policy Subsidies**: national/provincial high-tech applications, subsidy filings — ¥3.75M+ secured
- **Standardization**: SOP design, operations handbook writing

## License

MIT — see [LICENSE](./LICENSE).

## Credits

Curated by [@baefu828](https://github.com/baefu828). Issues and PRs welcome.