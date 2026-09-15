# DeepSeek Harness 架构与 WSL 部署资料（2026-09-15）

本目录是个人 fork 的分析与部署证据归档，不是上游项目的产品文档、当前架构规范或安装指南。材料以 2026-09-15 的本机环境和当时检出的源码为基线；fork 后续更新不自动改写这些历史快照。

## 归档内容

| 文件 | 内容 | 检视方式 |
|---|---|---|
| [architecture-and-agent-communication-notes.pptx](architecture-and-agent-communication-notes.pptx) | 两页系统架构与多 Agent 通信业务场景/方案分析，含两页详细讲解词（PPT 备注） | PowerPoint 或兼容演示软件 |
| [architecture-preview.png](architecture-preview.png) | 第 1 页系统架构图预览 | 浏览器 |
| [agent-communication-preview.png](agent-communication-preview.png) | 第 2 页 Agent 通信分析预览 | 浏览器 |
| [wsl-deployment-report.html](wsl-deployment-report.html) | WSL2 部署的环境、步骤、问题处置、验证、运行状态与运维命令 | 浏览器离线打开；可打印为 PDF |

## 基线和边界

- 架构资料与部署过程围绕 `deepseek-ai/deepseek-harness` 展开；本机部署源码提交为 `c291e7961a515f6d7af9304e7fd1d257929aef26`。归档时个人 fork 的 `master` 已位于较新的提交，阅读架构图时应对照相应版本的源码与仓库现行 [`docs/architecture.md`](../../docs/architecture.md)。
- 部署报告记录的环境为 Ubuntu 24.04.4 LTS / WSL2、Node.js v22.22.0、pnpm 11.7.0；Web 服务当时绑定 `127.0.0.1:3080`，并未配置自动启动。
- HTML 报告保留原始本机报告的路径文字作为部署证据；在 GitHub 中查看时，请以本目录的 `wsl-deployment-report.html` 为实际归档路径。
- 报告与演示材料均未包含可用 API Key、Cookie 或真实进程访问令牌；凭据文件只记录存在状态，不归档内容。

## 归档位置选择

仓库 `docs/` 承担经过验证、按主题归属且与当前源码同步的官方文档。此处的 PPT 是个人架构解读，HTML 是一次本机部署的时间点记录，因此放在根目录 `personal-archive/` 下，与上游规范和生成文档隔离，避免将历史证据误读为最新产品行为。
