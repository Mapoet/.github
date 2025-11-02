# Mapoet 贡献指南 / Contributing Guide

感谢你帮助维护 `Mapoet/.github` 仓库。这个仓库提供 Mapoet 账号的全局模板与协作规范，贡献内容会影响所有未覆盖的项目。请在提交前阅读以下指引，确保变更能够顺利传播。

## 核心原则 / Core Principles

- **一致性优先**：模板应适用于大多数 Mapoet 仓库，保持跨项目体验统一。
- **最小惊讶**：避免引入与常见开源流程相悖的约定，必要时提供清晰说明。
- **可复用性**：文档、脚本与工作流要易于扩展，允许单个仓库进一步定制。
- **透明协作**：公开讨论提案背景、目标与影响，确保历史记录清晰可追溯。

## 快速开始 / Getting Started

1. **熟悉目录结构**：阅读 [README](./README.md) 了解模板的适用范围与调用方式。
2. **认领任务**：在 Issue 中确认需求，或发起新 Issue 描述你的提案与影响面。
3. **创建分支**：使用 `meta/描述` 或 `docs/描述` 命名分支，便于识别全局变更。
4. **保持同步**：在开发期间定期同步 `main` 分支，减少后续冲突。

## 编写与测试 / Authoring & Verification

- **文档**：使用中英文双语或确保最少包含中文描述，方便 Mapoet 社区理解。
- **模板**：更新 Issue/PR 模板后，请使用预览或测试仓库验证渲染效果。
- **工作流**：新增或修改 GitHub Actions 时，尽量提供可复用的输入参数与示例调用。
- **本地校验**：针对脚本或配置文件运行必要的 lint/格式化工具，避免语法错误。

## 提交规范 / Commit Style

- 采用 [Conventional Commits](https://www.conventionalcommits.org/) 格式，例如 `feat(template): add security incident issue form`。
- 单次提交聚焦一个主题，便于回滚与审查。
- 在提交描述中说明受影响的模板、仓库或流程。

## Pull Request 自检单 / Pull Request Checklist

在创建 PR 前，请确认：

- [ ] 关联 Issue 或在描述中阐明背景与目标。
- [ ] 解释变更对其他仓库的影响与迁移建议。
- [ ] 更新或新增的模板已经在预览中检查渲染结果。
- [ ] 如涉及工作流，提供 `uses:` 的示例或文档链接。
- [ ] 文档、截图及其他相关资源已同步更新。
- [ ] 已通过相关的 lint / formatter 检查。

## 沟通约定 / Communication

- 使用 GitHub Issues、Discussions 或 PR 评论作为主要沟通渠道。
- 默认响应时间为 2 个工作日内，如需更久请提前说明。
- 若讨论范围超出原始话题，建议开启新的 Issue，保持主题聚焦。

## 发布与同步 / Deployment

- 变更合并后将立即生效。请在 PR 描述中提醒受影响的仓库维护者是否需要手动同步或更新。
- 对于重大变更（如删除模板、调整许可证），请在 `Discussions` 中发布公告或 Changelog。

感谢你的贡献与细心维护，让 Mapoet 的所有仓库都能享受一致、温暖且高效的社区体验。
