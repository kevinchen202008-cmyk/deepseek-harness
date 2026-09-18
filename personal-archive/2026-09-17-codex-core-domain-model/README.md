# Codex 核心数据对象与关系 UML（2026-09-17）

本目录归档一份 Codex 概念域模型，用于说明分组、项目、文件夹、工作目录、任务、对话、Git 仓库与 Worktree 等核心对象及其关系。

## 归档内容

| 文件 | 内容 | 检视方式 |
|---|---|---|
| [codex-core-domain-model-uml.html](codex-core-domain-model-uml.html) | 核心对象卡片、UML 类图、对象属性矩阵、DeepSeek Harness 当前实例图、关键业务规则和可复用 PlantUML 源码 | 浏览器离线打开；支持打印或导出 PDF |

## 模型边界

- 本模型基于 2026-09-17 可观察到的 Codex Desktop 产品行为和本地项目配置整理。
- 内容用于解释产品概念和对象关系，不代表 OpenAI 内部完整数据库结构或稳定 API 契约。
- DeepSeek Harness 实例部分用于展示导航分组、项目绑定和任务工作目录之间的差异。
- HTML 为单文件交付物，样式与 SVG 均已内嵌，不依赖外部网络资源。

## 与其他归档的关系

DSH 系统架构、Agent 通信分析和 WSL 部署过程保存在相邻的 [`2026-09-15-dsh-architecture-deployment`](../2026-09-15-dsh-architecture-deployment/) 目录。本目录只存放 Codex 工作环境的概念模型，避免与 DSH 产品架构混淆。
