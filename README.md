<p align="center">
  <img src="./assets/header.svg" width="100%" alt="Xiaoping Liao — Agent systems, developer tools, reliable execution" />
</p>

<p align="center">
  <a href="#selected-projects">Projects</a> &nbsp; / &nbsp;
  <a href="#merged-contributions">Open source</a> &nbsp; / &nbsp;
  <a href="https://github.com/kyletser?tab=repositories">Repositories</a>
</p>

I build **agent systems and developer tools**, with a focus on state, recovery, and observable execution. My current projects explore local-first coding agents and evidence-grounded learning agents.

`Python` · `TypeScript` · `Agent runtimes` · `MCP` · `Knowledge graphs`

## Selected projects

<table>
<tr>
<td width="50%" valign="top">
<h3>01 / CodeRook</h3>
<p><strong>A local-first coding agent.</strong></p>
<p>Durable sessions, explicit permissions, reviewable changes, and evidence-backed runs. TUI and web clients share a persistent daemon.</p>
<p><code>Agent runtime</code> <code>Developer tools</code></p>
<a href="https://github.com/kyletser/coderook">Explore CodeRook →</a>
</td>
<td width="50%" valign="top">
<h3>02 / CoursePilot</h3>
<p><strong>A knowledge-grounded learning agent.</strong></p>
<p>Course Q&amp;A and study paths grounded in teacher-reviewed material, with knowledge graphs and reproducible evaluation reports.</p>
<p><code>Retrieval</code> <code>Knowledge graphs</code></p>
<a href="https://github.com/kyletser/coursepilot">Explore CoursePilot →</a>
</td>
</tr>
</table>

Also building [work-hunter](https://github.com/kyletser/work-hunter), a job-search assistant with human approval before outreach, and [Plinth](https://github.com/kyletser/plinth), an inspectable workflow runtime with durable run evidence.

## Merged contributions

Selected contributions to upstream agent frameworks and runtime tooling. Each link includes the implementation and review history.

| Upstream | Contribution | PR |
| :--- | :--- | :---: |
| **Microsoft · Agent Framework** | Declarative DevUI message input, fresh-run state isolation, and deterministic checkpoint regression tests | [#7839 ↗](https://github.com/microsoft/agent-framework/pull/7839) |
| **Hindsight** | Defer retain completion callbacks until store commit so event counts reflect committed memory | [#4203 ↗](https://github.com/vectorize-io/hindsight/pull/4203) |
| **OpenAI · Agents SDK JS** | Remove redundant Computer Use screenshots; cover direct execution, approval resume, and replay | [#1827 ↗](https://github.com/openai/openai-agents-js/pull/1827) |
| **Apache Maka** | Close SQLite stores before test workspace cleanup on Windows | [#3644 ↗](https://github.com/apache/maka/pull/3644) |

<details>
<summary><strong>More contributions · follow the upstream review</strong></summary>
<br />

- [OpenHands SDK #4717](https://github.com/OpenHands/software-agent-sdk/pull/4717) — launch-time skill overlays for profile-based ACP agents.
- [MCP TypeScript SDK #2699](https://github.com/modelcontextprotocol/typescript-sdk/pull/2699) — bounded validator caching for schemas without usable IDs.
- [Strands Agent SOP #78](https://github.com/strands-agents/agent-sop/pull/78) — deterministic recursive discovery of external SOPs.

These are separate from the merged contributions above. Follow each PR for its current status.

</details>

---

<p align="center"><sub>State belongs to a run. Observations follow actions. Completion follows commit.</sub></p>
