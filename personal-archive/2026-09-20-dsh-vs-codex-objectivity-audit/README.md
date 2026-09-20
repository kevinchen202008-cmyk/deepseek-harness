# DSH vs Codex 对比报告客观性审查（2026-09-20）

本目录归档一份元分析：审查两份各自独立生成的「DSH vs Codex」对比分析报告在证据处理方式与呈现框架上的差异，并对哪一方更客观给出判断。

## 归档内容

| 文件 | 内容 | 检视方式 |
|---|---|---|
| [objectivity-audit.html](objectivity-audit.html) | 客观性审查主文档：六项客观性指标对照表、逐项拆解（证据分级、自我纠错、量化评分方法论、呈现框架中立性、批评对称性、结论分布）、本审查的局限性说明 | 浏览器离线打开；引用两份原始报告的相对链接需保持 `reports/` 子目录结构 |
| [reports/dsh-report.html](reports/dsh-report.html) | 被审查对象 A：DSH 自评版对比报告（DSH `0.1.5-rc.2` 基线，原始路径 `SweBench_auto_verify/docs/dsh-vs-codex.html`） | 浏览器离线打开 |
| [reports/codex-report.html](reports/codex-report.html) | 被审查对象 B：Codex 自评版对比报告（DSH `0.1.6-alpha.1` 基线，原始路径 `DeepSeekHarness-Project/deliverables/comparison/DSH-vs-Codex-对比分析-20260918.html`） | 浏览器离线打开 |

## 核心判断

DSH 版在证据分级、自我纠错、批评对称性三方面提供了可复核的具体依据（本机实测/官方文档/第三方证据徽章、"对初版判断的三处更正"专节、带源码路径与 GitHub issue 编号的具体批评）；Codex 版视觉打磨度更高，但缺少逐条证据分级与修正记录，引入了无方法论支撑的 0–100 量化评分，且对比矩阵的结论分布明显偏向自身。综合来看，**DSH 版的方法论纪律更严谨、可验证性更强**。

## 模型边界

- 本审查只针对两份 HTML 报告的文本、结构与呈现方式做比较，未独立复核其引用的每一条底层事实（例如未逐一验证 DSH 版列出的 GitHub issue 编号是否属实）。
- "对象 A 由 DSH 生成 / 对象 B 由 Codex 生成"的归属，来自提问者的标注与文件所在目录路径，未独立确认具体生成流程。
- 审查所用的六项客观性指标（证据分级、自我纠错、量化评分方法论、呈现框架中立性、批评对称性、结论分布）由审查者自行选定，选择维度本身也可能带有倾向性，建议将本文档视为一种审查意见而非最终裁决。
- 本次审查不构成对 DeepSeek Harness 或 OpenAI Codex 产品本身的评测结论。

## 与其他归档的关系

DSH 系统架构、Agent 通信分析与 WSL 部署过程保存在 [`2026-09-15-dsh-architecture-deployment`](../2026-09-15-dsh-architecture-deployment/)；Codex 核心数据对象与关系 UML 保存在 [`2026-09-17-codex-core-domain-model`](../2026-09-17-codex-core-domain-model/)。本目录只存放对两份 DSH/Codex 对比报告的元分析，不重复归档被比较双方的产品架构本身。
