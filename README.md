# 商业地产招商运营专家 Skill

**Commercial Real Estate Leasing & Operations Expert — an [Agent Skills](https://agentskills.io) package that turns 12 years of hands-on property operations into a portable skill for AI agents.**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](./LICENSE)
[![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)](./CHANGELOG.md)
[![Agent Skills](https://img.shields.io/badge/Agent%20Skills-compatible-5288ff.svg)](https://agentskills.io)
[![References](https://img.shields.io/badge/references-10%20modules-green.svg)](./references/)
[![Language](https://img.shields.io/badge/lang-中文-red.svg)](#english)

Works with Claude Code, Claude.ai, OpenAI Codex, Cursor, Gemini CLI, GitHub Copilot, VS Code, WorkBuddy and any agent that supports the [Agent Skills spec](https://agentskills.io).

`commercial-real-estate` `property-management` `real-estate-operations` `leasing` `tenant-management` `rent-collection` `industrial-park` `office-buildings` `retail-operations` `facility-management` `asset-management` `proptech` `agent-skills` `skill-md` `china-real-estate`

---

## 这是什么

一个把**商业地产招商运营实战经验**打包成标准的 `SKILL.md` 目录，让 AI Agent 在遇到招商、催缴、筹开、合同审阅、政策申报等问题时，**自动加载对应知识库并给出可落地的方案**，而不是泛泛而谈的行业套话。

它不是一份电子书，也不是一个 prompt 模板，而是一套**按需加载的知识系统**：

- Agent 冷启动时只读取 `SKILL.md`（约 200 行摘要）
- 命中触发词后，才加载对应的 `references/` 模块原文
- 需要出活时，直接调用 `templates/` 里的表单与模板

### 和其他「商业地产 prompt」的区别

| | 通用大模型 | 本 Skill |
|---|---|---|
| 知识来源 | 公开泛化信息 | 6 个标杆项目操盘总结 + 万科产城 49 份制度提炼 + 82 篇 2025-2026 行业深度文章 |
| 输出形态 | 建议性文字 | 带时间线、责任人、量化指标、风险预案的结构化方案 |
| 数据支撑 | 无 | 招商率 95%、收缴率 95%-98%、追回欠缴 37 万等真实项目数据 |
| 表单工具 | 无 | 催缴函、承接查验清单、筹开倒排表可直接套用 |
| 边界意识 | 容易编造 | 明确标注经验边界，政策/法律类问题主动提示以官方口径为准 |

---

## 它能做什么

按「你说什么 → 它调什么 → 你得到什么」的方式触发：

| 当你需要… | 自动加载 | 你会得到 |
|---|---|---|
| 做招商策略、品牌落位、租金定价、中介合作 | `leasing-strategy.md` | 渠道矩阵、品牌金字塔、去化节奏、租金定价方法论 |
| 催欠租、发律师函、推进诉讼、做风险预警 | `collection-strategy.md` + 催缴函模板 | 10 步催缴时间线、分级催收动作、文书模板 |
| 新项目筹开、交付倒排、承接查验、商户进场装修 | `startup-checklist.md` + 倒排计划模板 | 分阶段倒排表、查验清单、装修巡检标准 |
| 审阅租赁合同、排查条款风险 | `contract-review-points.md` | 12 维清单逐项核对 + 16 条速查 + 违约触发点 |
| 申报补贴、高企、孵化器、小微园区 | `policy-database.md` | 杭州市/区政策矩阵、申报路径、材料清单 |
| 做商户星级评定、商户考核与激励 | `merchant-rating-system.md` | 五维度 100 分评分表 + 坪效指数 + 奖惩机制 |
| 建物业标准、处理消防/应急/商户守则 | `property-management-standards.md` | 管理制度要点 + 46 项表单索引 |
| 看行业趋势、做竞品分析、写运营复盘 | `industry-insights.md` | 82 篇深度文章的精华结论 |
| 搭营运体系、写 SOP、建流程制度 | `vanke-ops-system.md` | 万科产城全套营运制度提炼 |
| 查杭州各区租金、算坪效 | `rent-benchmark.md` | 分区租金参考区间与定价逻辑 |

---

## 仓库结构

```
commercial-real-estate-expert-skill/
├── SKILL.md                          # 统一入口：人设 + 能力 + 触发词 + 知识库索引
├── references/                       # 10 个知识库模块（按需加载）
│   ├── collection-strategy.md        # 催缴策略：10 步时间线 + 集团 6 步 + 实战数据
│   ├── contract-review-points.md     # 合同审阅：12 维清单 + 16 条速查
│   ├── industry-insights.md          # 行业洞察：82 篇 2025-2026 深度文章精华
│   ├── leasing-strategy.md           # 招商策略：渠道矩阵 + 实战 KPI + 商户案例
│   ├── merchant-rating-system.md     # 星级评定：五维度 100 分 + 坪效指数
│   ├── policy-database.md            # 政策申报：杭州市/区申报矩阵
│   ├── property-management-standards.md  # 物业标准：46 项表单索引
│   ├── rent-benchmark.md             # 租金基准：杭州各区参考区间
│   ├── startup-checklist.md          # 筹开管理：进场/装修/巡检/撤场
│   └── vanke-ops-system.md           # 万科营运：49 份制度提炼
├── templates/                        # 3 个可直接套用的工具模板
│   ├── 催缴函模板.md
│   ├── 验房承接查验清单.md
│   └── 筹开倒排计划模板.md
├── assets/avatar.png
├── CHANGELOG.md  CONTRIBUTING.md  LICENSE
└── .github/workflows/validate.yml    # CI：frontmatter / 链接 / 路径合规校验
```

---

## 安装

### 方式 1：CLI（推荐）

```bash
npx skills add baefu828/commercial-real-estate-expert-skill
# 或
npx skillkit install baefu828/commercial-real-estate-expert-skill
```

### 方式 2：克隆到你的 Agent 目录

```bash
# WorkBuddy
git clone https://github.com/baefu828/commercial-real-estate-expert-skill.git \
  ~/.workbuddy/skills/commercial-real-estate-expert

# Claude Code
git clone https://github.com/baefu828/commercial-real-estate-expert-skill.git \
  ~/.claude/skills/commercial-real-estate-expert

# Cursor / Codex / 其他（放到项目内也可被识别）
git clone https://github.com/baefu828/commercial-real-estate-expert-skill.git \
  .agents/skills/commercial-real-estate-expert
```

重启工具后即可使用，无需额外配置。

### 方式 3：作为 Git Submodule 引入项目

```bash
git submodule add https://github.com/baefu828/commercial-real-estate-expert-skill.git \
  .agents/skills/commercial-real-estate-expert
```

### 方式 4：手动加载

把 `SKILL.md` 的内容作为系统提示词前缀，注入任何支持 Markdown 的 Agent 框架即可。

---

## 使用示例

直接用自然语言说，Agent 会自行判断加载哪个模块。

```
我手上有个 5 万㎡的产业园，从拿房到开业只有 8 个月，
帮我出一份从 0 到 1 的筹开倒排计划。
```
→ 加载 `startup-checklist.md` + `筹开倒排计划模板.md`，输出带里程碑的倒排表。

```
某租户欠租 3 个月共 18 万，沟通多次无果，
怎么分级推进催缴、什么时候上律师函？
```
→ 加载 `collection-strategy.md` + `催缴函模板.md`，给分级催收 + 诉讼推进路径。

```
帮我审这份租赁合同，重点看租金、物业费、保证金条款有什么坑。
```
→ 加载 `contract-review-points.md`，按 12 维清单逐项核对并标注法理依据。

```
园区有 12 家科技型中小企业，今年想报市高和孵化器，
材料和流程怎么走？
```
→ 加载 `policy-database.md`，给申报矩阵、材料清单与时间节点。

也可以显式调用：`/commercial-real-estate-expert 帮我做一份商户星级评定方案`。

---

## 适合谁

- **招商 / 营运 / 资产管理人员**：需要快速拿到带数据的方案框架与表单
- **商业地产团队负责人**：想把团队经验沉淀成可复用的 AI 助手
- **AI 应用开发者**：需要一个垂直行业 Skill 作为集成示例
- **产业园 / 街区运营方**：政策申报、商户管理、物业标准化的日常参考

## 不适合什么

- 具体城市的规划报建、消防验收等行政审批细节（以主管部门口径为准）
- 医疗、教育、宗教等特殊业态的专业规范（超出本 Skill 覆盖范围）
- 法律诉讼的最终判断（会给出路径建议，但会提示咨询专业律师）

---

## 使用须知

本 Skill 输出的内容**供专业参考**：

- 租金定价、招商政策等随城市、区域、时点变化，请结合当地行情调整
- 政策申报具有时效性，请以最新政策文件为准
- 涉及合同条款解释与诉讼推进，请咨询专业律师确认

---

## 贡献

欢迎补充知识库、修正数据、改善文档，详见 [CONTRIBUTING.md](./CONTRIBUTING.md)。提交 PR 前请确认：

- Markdown 格式规范（CI 会自动校验）
- 新增或重命名 reference 时，同步更新 `SKILL.md` 的「知识库索引」
- 在 [CHANGELOG.md](./CHANGELOG.md) 的 `Unreleased` 段落记录变更

觉得有用的话，点个 ⭐ 支持一下。

---

## 许可证

[MIT](./LICENSE) — 自由使用、修改、分发，保留版权声明即可。

## 致谢

由 [@baefu828](https://github.com/baefu828) 基于 12 年商业地产招商运营实战经验整理发布。问题与建议请提交 [Issue](https://github.com/baefu828/commercial-real-estate-expert-skill/issues)。

---

<a id="english"></a>

## English

A standard [Agent Skills](https://agentskills.io) package encoding **12 years of commercial real estate leasing & operations experience** — industrial parks, office buildings, and commercial districts — from a practitioner who ran 6 flagship projects (17 万㎡ / 200+ tenants) at Vanke and Hangzhou's Wensan Digital Life Block.

**What's inside**

- `SKILL.md` — persona, capabilities, trigger keywords, and the reference index (loaded first)
- `references/` × 10 — collection strategy, contract review, industry insights (82 articles), leasing strategy, merchant rating, policy subsidies, property management, rent benchmarks, startup checklist, Vanke operations system
- `templates/` × 3 — dunning letters, handover inspection checklist, project launch countdown

**Install**

```bash
npx skills add baefu828/commercial-real-estate-expert-skill
# or
git clone https://github.com/baefu828/commercial-real-estate-expert-skill.git \
  ~/.claude/skills/commercial-real-estate-expert
```

**Use** — just describe the task in natural language and the agent loads the matching module:

```
A tenant owes 3 months of rent. How do I escalate collection and when should I send a lawyer's letter?
→ loads collection-strategy.md + dunning letter template
```

**Caveats** — rent benchmarks and policy content are China (Hangzhou)-specific and time-sensitive; legal escalation advice should be confirmed with a licensed lawyer. MIT licensed. Issues and PRs welcome.
