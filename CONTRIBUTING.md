# Contributing / 贡献指南

感谢你有兴趣完善这个商业地产 Skill！本项目接受以下形式的贡献：

## 🤝 贡献方式

### 1. 报告 Bug / 提出建议
- 在 GitHub Issues 区提交，说明复现步骤、期望结果、实际结果
- 标题用 `[Bug]` 或 `[Suggestion]` 前缀

### 2. 补充知识库内容
- **新增 reference**：在 `references/` 目录下添加新的 `.md` 文件，建议包含：触发词、核心内容、使用场景
- **更新现有 reference**：直接编辑对应 `.md` 文件，保持章节结构清晰
- **新增 template**：在 `templates/` 目录下添加工具模板

### 3. 改进输出规范
- 编辑 `SKILL.md` 中的"工作流程"或"输出规范"章节
- 增加可量化指标、风险提示模板等

### 4. 完善文档
- 修正错别字、补充使用示例、改善 README 可读性

## 📝 提交规范

### Branch 命名
```
feat/add-collection-template       # 新功能
fix/typo-in-contract-review        # 修 bug
docs/improve-readme                # 文档
refactor/restructure-references    # 重构
```

### Commit 信息
```
type(scope): 简短描述

详细说明（可选）
```

`type` 取值：`feat` / `fix` / `docs` / `refactor` / `test` / `chore`

### Pull Request 流程
1. Fork 本仓库
2. 创建特性分支（`git checkout -b feat/your-feature`）
3. 提交改动（`git commit -m "feat: 新增XX模板"`）
4. 推送到你的 Fork（`git push origin feat/your-feature`）
5. 在本仓库创建 Pull Request，说明：
   - 改动动机
   - 改动内容
   - 测试方法（如果是新模板/新功能）

## ✅ 合并要求

提交 PR 前请确认：

- [ ] Markdown 格式规范（CI 会自动校验）
- [ ] 引用链接有效（CI 会自动校验）
- [ ] 保留了原文档的章节结构
- [ ] 在 `SKILL.md` 的"知识库索引"中同步更新（如新增/重命名 reference）
- [ ] 在 `CHANGELOG.md` 的 `Unreleased` 段落记录变更

## 🚫 不接受的贡献

为保护项目质量和作者权益，以下内容不予合并：

- 商业广告 / 推广链接
- 与商业地产招商运营无关的内容
- 未注明来源的第三方版权材料
- 含有个人隐私信息（手机号、身份证号、内部敏感文档路径等）

## 📞 联系方式

- GitHub Issues：首选沟通渠道
- Email：baefu828（GitHub 用户名对应邮箱可在其 GitHub Profile 找到）

## 📜 许可证

提交 PR 即代表你同意以 MIT 协议授权你的贡献。