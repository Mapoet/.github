# Mapoet Global Community Settings

欢迎来到 `Mapoet/.github` 仓库。这个仓库不会存放业务代码，而是集中维护 Mapoet 账号下所有项目的协作约定、默认模板与复用工具链。本项目中的内容会在未显式覆写的仓库中自动生效，帮助你快速搭建一致、友好的协作体验。

## 仓库结构

| 路径 | 作用 |
| --- | --- |
| `CODE_OF_CONDUCT.md` | Mapoet 项目的社区准则。 |
| `CONTRIBUTING.md` | 贡献指南与流程说明。 |
| `LICENSE` | 仓库内文本与模板的授权条款。 |
| `ISSUE_TEMPLATE/` | Issue 模板（缺陷、功能请求、配置说明）。 |
| `PULL_REQUEST_TEMPLATE.md` | 全局 PR 模板。 |
| `.github/workflows/` | 可复用的 GitHub Actions 工作流。 |
| `SECURITY.md` | 漏洞上报流程。 |
| `SUPPORT.md` | 用户与贡献者支持渠道。 |
| `CODEOWNERS` | 默认代码审阅负责人。 |
| `FUNDING.yml` | 统一的赞助与捐助配置。 |

## 如何复用这些模板

- **Issue/PR 模板**：当 Mapoet 账号下的仓库没有自定义模板时，这些模板会自动出现在 GitHub 的 Issue / PR 创建界面。
- **Actions 工作流**：在其他仓库中可以通过以下方式调用本仓库的复用流程：

  ```yaml
  uses: Mapoet/.github/.github/workflows/reusable-ci.yml@main
  with:
    run-tests: true
  ```

- **RayTracy 环境工作流**：针对 `Mapoet/RayTracy` 所需的图形与构建依赖，新增了 `raytracy-environment.yml`。可在仓库中调用以自动完成依赖安装、CMake 构建与 `ctest` 测试：

  ```yaml
  uses: Mapoet/.github/.github/workflows/raytracy-environment.yml@main
  with:
    build-type: RelWithDebInfo
    run-tests: true
  ```

- **社区文档**：`CODE_OF_CONDUCT.md`、`CONTRIBUTING.md`、`SECURITY.md` 等文档会成为其他仓库的默认入口，让贡献者始终能找到一致的协作规范。

## 自定义或覆盖

如果某个仓库需要不同的流程或模板，可在该仓库的 `.github/` 目录中新增对应文件（例如 `PULL_REQUEST_TEMPLATE.md`）。GitHub 会优先使用仓库局部的定义。

## 反馈与改进

欢迎直接在本仓库创建 Issue 或 Pull Request，帮助完善 Mapoet 的全局社区体验。你也可以通过 `SUPPORT.md` 中列出的渠道联系维护者。
