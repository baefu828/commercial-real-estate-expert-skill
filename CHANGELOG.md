# Changelog

All notable changes to this Skill will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Changed
- README 重写：参照 anthropics/skills、marketingskills 等主流 Skill 仓库的写法，改为「定位 → 触发场景 → 模块索引 → 安装 → 示例 → 边界」结构
- 安装方式扩展为 4 种（CLI / 克隆到各 Agent 目录 / Git Submodule / 手动加载）
- 英文说明压缩为精简 English 段，中文为主

## [1.0.0] - 2026-09-09

### Added
- 首版发布：从 WorkBuddy 商业地产招商运营专家转化为通用 Agent Skill 格式
- 10 个 references 知识库文件（催缴/合同/行业洞察/招商/星级评定/政策/物业/租金/筹开/万科营运体系）
- 3 个 templates 工具模板（催缴函/验房清单/筹开倒排计划）
- SKILL.md 统一入口（合并专家人设与知识库索引）
- 双语 README（中英文）
- MIT 许可证
- GitHub Actions 自动校验 workflow

### Notes
- 本版本基于原 WorkBuddy Expert 包 `commercial-real-estate-expert@1.0.0` 转化
- 移除 `references/file-archive-index.md`（仅指向作者本地资料库路径，对外部用户无意义）
- author 信息从 `liuzhihao9444@agent.qq.com` 替换为 GitHub 用户名 `baefu828`