<p align="center">
  <img src="./assets/header.svg" width="100%" alt="Xiaoping Liao — Agent 系统与开发者工具" />
</p>

<p align="center">
  <a href="./README.md">English</a> &nbsp; · &nbsp; <strong>简体中文</strong>
</p>

<p align="center">
  <a href="#代表项目">代表项目</a> &nbsp; / &nbsp;
  <a href="#已合并的开源贡献">开源贡献</a> &nbsp; / &nbsp;
  <a href="#工程关注点">工程关注点</a>
</p>

我主要开发 **Agent 系统与开发者工具**，关注执行过程是否可检查、状态是否可恢复，以及结果是否有可追溯的验证依据。

`Python` · `TypeScript` · `Agent Runtime` · `MCP` · `知识图谱与检索`

## 代表项目

<table>
<tr>
<td width="50%" valign="top">
<p><sub>01 / 编程与执行</sub></p>
<h3><a href="https://github.com/kyletser/coderook">CodeRook ↗</a></h3>
<p><strong>本地优先的 Coding Agent</strong> · <code>公开 Beta</code></p>
<p>TUI 与 Web 共享持久化本地 daemon，围绕会话恢复、权限审批、变更审查和执行记录组织编程流程。</p>
<p><a href="https://github.com/kyletser/coderook/releases/tag/v0.2.0-beta.1">体验 Beta</a> · <a href="https://github.com/kyletser/coderook/blob/HEAD/docs/zh-CN/README.md">中文入门</a> · <a href="https://github.com/kyletser/coderook/blob/HEAD/docs/reference/FUNCTIONAL_ARCHITECTURE.md">架构</a></p>
</td>
<td width="50%" valign="top">
<p><sub>02 / 检索与学习</sub></p>
<h3><a href="https://github.com/kyletser/coursepilot">CoursePilot ↗</a></h3>
<p><strong>知识图谱增强的课程学习 Agent</strong> · <code>MVP</code></p>
<p>以教师审核资料为知识边界，提供带引用问答、诊断测验和学习路径；用冻结评测与原始记录验证检索和问答表现。</p>
<p><a href="https://github.com/kyletser/coursepilot#readme">本地运行</a> · <a href="https://github.com/kyletser/coursepilot/blob/HEAD/docs/evaluation/agent-evaluation-2026-09-05.md">评测报告</a> · <a href="https://github.com/kyletser/coursepilot/blob/HEAD/docs/evaluation/qwen3-final-report.md">微调实验</a></p>
</td>
</tr>
<tr>
<td width="50%" valign="top">
<p><sub>03 / 工作流与运行记录</sub></p>
<h3><a href="https://github.com/kyletser/plinth">Plinth ↗</a></h3>
<p>本地 Agent 工作流运行时，关注可检查的执行过程与持久化运行记录。</p>
</td>
<td width="50%" valign="top">
<p><sub>04 / 应用与人工审批</sub></p>
<h3><a href="https://github.com/kyletser/work-hunter">work-hunter ↗</a></h3>
<p>本地求职助手，通过 AI 排序辅助筛选岗位，对外联系前保留人工审批。</p>
</td>
</tr>
</table>

<details>
<summary><strong>项目验证边界</strong></summary>

- CodeRook 当前为公开 Beta，不等于稳定版 v1 已发布。离线 fixture 测试不作为模型能力成绩；发布条件见 [release scorecard](https://github.com/kyletser/coderook/blob/HEAD/docs/status/RELEASE_SCORECARD.md)，安全假设见 [threat model](https://github.com/kyletser/coderook/blob/HEAD/docs/reference/THREAT_MODEL.md)。
- CoursePilot 的检索与微调结论以各自报告中的样本、模型和实验设置为准。微调是取舍实验，不声称准确率全面提升。

</details>

## 已合并的开源贡献

以下四项均链接到上游 PR，可查看最终实现和评审过程。

| 项目 | 解决的问题 | PR |
| :--- | :--- | :--- |
| **Microsoft Agent Framework** | 修复声明式工作流 DevUI 消息输入，隔离新运行状态，并补充确定性 checkpoint 回归测试 | [#7839](https://github.com/microsoft/agent-framework/pull/7839) |
| **OpenAI Agents SDK JS** | 消除 Computer Use 重复最终截图，覆盖直接执行、审批恢复与重放路径 | [#1827](https://github.com/openai/openai-agents-js/pull/1827) |
| **Hindsight** | 将 retain 完成回调延后至存储提交之后，让事件计数对应已提交的记忆 | [#4203](https://github.com/vectorize-io/hindsight/pull/4203) |
| **Apache Maka** | 在 Windows 测试清理临时目录前关闭 SQLite Store，修复资源生命周期问题 | [#3644](https://github.com/apache/maka/pull/3644) |

其他已提交工作涉及 MCP 缓存、SOP 递归发现、浏览器启动诊断和 Agent 记忆。它们与上述已合并成果分开记录：[查看提交清单](./README.md#contribution-pipeline)。实时状态以上游 PR 为准。

## 工程关注点

- **状态与恢复**：会话边界、checkpoint、持久化执行与中断恢复。
- **工具与协议**：MCP、浏览器操作、审批前后的执行一致性。
- **记忆与验证**：提交顺序、知识来源、回归测试和可复现报告。

通常从复现失败开始，添加回归测试，再通过临时移除修复确认测试能捕获问题。项目功能、实验结果与上游已合并成果分别呈现，不混为一谈。

---

<p align="center"><a href="https://github.com/kyletser?tab=repositories">查看全部仓库 ↗</a> &nbsp; · &nbsp; <a href="./README.md">English profile ↗</a></p>
