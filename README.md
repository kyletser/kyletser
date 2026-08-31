<h1 align="center">Xiaoping Liao</h1>

<p align="center">Agent systems, developer tools, and open-source infrastructure</p>

I build agent runtimes and tools for developers. Most of my work is about making long-running agents easier to inspect, test, and recover when something goes wrong.

Right now I am working on [CodeRook](https://github.com/kyletser/coderook), a local-first coding agent with durable sessions, explicit permissions, reviewable changes, and evidence-backed run results.

## Projects

| Project | What it does |
| --- | --- |
| [CodeRook](https://github.com/kyletser/coderook) | Local-first coding agent with TUI and web clients backed by one persistent daemon |
| [work-hunter](https://github.com/kyletser/work-hunter) | Local job-search assistant that ranks roles and keeps a human approval step before outreach |
| [Plinth](https://github.com/kyletser/plinth) | Local runtime for inspectable agent workflows, durable run evidence, and explicit effect authorization |

## Open-source work

- [Apache Maka #3644](https://github.com/apache/maka/pull/3644): fixed Windows cleanup failures in non-blocking shell runtime tests. Merged.
- [OpenHands software-agent-sdk #4717](https://github.com/OpenHands/software-agent-sdk/pull/4717): added structured launch-time skill overlays for profile-based ACP agents.
- [Model Context Protocol TypeScript SDK #2699](https://github.com/modelcontextprotocol/typescript-sdk/pull/2699): added bounded validator caching for schemas without usable IDs.
- [Microsoft Agent Framework #7839](https://github.com/microsoft/agent-framework/pull/7839): fixed message input for declarative workflows in DevUI.
- [Strands Agent SOP #78](https://github.com/strands-agents/agent-sop/pull/78): added deterministic recursive discovery for SOPs in nested directories.

I work mainly in Python and TypeScript, with Rust, Go, and C++ where they fit the problem.
