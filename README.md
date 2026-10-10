# Tanner Osterkamp

Founder of [Mesh](https://meshvault.ai) and [TheFireDev](https://thefiredev.com). AI application engineer in Dana Point, California.

Mesh is an all-in-one OS: your own assistant, your projects and the things you watch, in one app. Agents stop for a named person's approval before they send, pay, post, or delete. It is free, with everything included.

## Products (status as of 2026-10-09)

- **[Mesh](https://meshvault.ai)**: runs on the web at [meshvault.ai/app](https://meshvault.ai/app). The iPhone app is pre-release (TestFlight by invite, no App Store listing yet). Android is an early build, not on Google Play yet.
- **[The one-week install](https://meshvault.ai/install)**: a server you own, with Hermes Desktop and Mesh paired to it, and a backup that has passed a restore test. Quoted per job. No monthly plans.
- **[Protocol Guide](https://protocol-guide.com)**: source-cited EMS protocol search by county for students, educators and clinicians. Every result names the protocol book it came from. Education and reference only: not a medical device, not for bedside care. The web app is live. The iOS app is not on the App Store yet.
- **[JudgeFinder](https://judgefinder.vercel.app)**: free, anonymous judge lookup built on CourtListener docket metadata. It shows court assignment, case volume and recent dockets. It is not legal advice and it publishes no bias scores. The judgefinder.io domain is being restored.
- **[MeshVault Harness](https://github.com/thefiredev-cloud/meshvault-harness)**: a shell installer for Linux or macOS that sets up Hermes Agent, OMP and a local Qwen3 model, plus 11 free skills that each carry a written approval step. A 9-skill Pro pack is $99 and a done-for-you install is $499, both described at [thefiredev.com/harness](https://thefiredev.com/harness).
- **[TheFireDev](https://thefiredev.com)**: my consulting and freelance studio. It builds AI systems for small businesses: the model, the application, and the compute.

## What I work on

- Local LLM serving on NVIDIA DGX Spark clusters.
- Agent orchestration: one accountable coordinator, bounded specialist roles, and approval gates before real-world actions.
- Small, inspectable tools for agents: MCP servers, Claude Code plugins, and plain Markdown skills.

## Public repositories

Every repository below has a README that states what it does, what it needs and where it falls short.

**Agents and MCP**

- [meshvault-harness](https://github.com/thefiredev-cloud/meshvault-harness): the installer described above. Its README lists every script it downloads and where from.
- [meshvault-skills-starter](https://github.com/thefiredev-cloud/meshvault-skills-starter): nine MIT agent skills in plain Markdown for small business admin work, each with a written approval gate.
- [agent-ops-kit](https://github.com/thefiredev-cloud/agent-ops-kit): Claude Code plugin with a deny-list scanner that fails a build when private strings survive into it.
- [meshvault-agentic-architecture](https://github.com/thefiredev-cloud/meshvault-agentic-architecture): reference documents and diagrams for a mixture-of-agents loop, role orchestration and approval levels. Documentation only.
- [eufy-camera-mcp](https://github.com/thefiredev-cloud/eufy-camera-mcp): MCP server that gives an agent view-only, allowlisted access to local cameras through MediaMTX.
- [cronjob-org-mcp-server](https://github.com/thefiredev-cloud/cronjob-org-mcp-server): MCP server that lists, creates, updates and deletes scheduled jobs on cron-job.org.

**Desktop tools**

- [mac-cu](https://github.com/thefiredev-cloud/mac-cu): Swift command line tool that lets an agent click, type, scroll, capture and read the accessibility tree on macOS.
- [omarchy-token-bar](https://github.com/thefiredev-cloud/omarchy-token-bar): Omarchy bar widgets that show daily token use for Claude Code, Codex, Grok, OMP and Hermes.
- [airpods-max-sidetone](https://github.com/thefiredev-cloud/airpods-max-sidetone): PipeWire sidetone loopback for AirPods Max on Linux, active only while another app records the mic.
- [reach-plugins](https://github.com/thefiredev-cloud/reach-plugins): example Lua plugins for the Reach SSH client.

**Forks**

- [Reach](https://github.com/thefiredev-cloud/Reach): fork of a Tauri SSH client with macOS copy and paste, vault password and registry URL fixes. Upstream is canonical.
- [meshvault-bot](https://github.com/thefiredev-cloud/meshvault-bot): fork of Rakazo that runs a bot app on Hermes Agent with a sandboxed computer per bot.

Most product code is private. Each repository states its license in its README. Where a repository has no LICENSE file, the README says so.

## Contact

- [LinkedIn](https://www.linkedin.com/in/tannerosterkamp)
- Websites: [meshvault.ai](https://meshvault.ai) · [thefiredev.com](https://thefiredev.com)
- Mesh questions: contact@meshvault.ai. A person reads it and replies.
- Consulting and freelance work: tanner@thefiredev.com
- Security reports: see [SECURITY.md](SECURITY.md). Please do not open public issues for vulnerabilities.
