# Tanner Osterkamp

Founder of [MeshVault](https://meshvault.ai) and [TheFireDev](https://thefiredev.com). AI application engineer in Dana Point, California.

MeshVault sets up a server a business owns, pairs Hermes Desktop and an iPhone app to it, and keeps a backup that has passed a restore test. Data and inference are local-first, and agents stop for a named person's approval before they send, pay, post, or delete.

## Products (status as of 2026-10-05)

- **[MeshVault](https://meshvault.ai)**: the one-week install of a server you own, with Hermes Desktop and an iPhone app paired to it. The iPhone app is pre-release (TestFlight by invite, no App Store listing yet). There are no paying install clients yet.
- **[Protocol Guide](https://protocol-guide.com)**: source-cited EMS protocol search by county for students, educators and clinicians. Every result names the protocol book it came from. Education and reference only: not a medical device, not for bedside care. The web app is live. The iOS app is not on the App Store yet.
- **[JudgeFinder](https://judgefinder.vercel.app)**: free, anonymous judge lookup built on CourtListener docket metadata. It shows court assignment, case volume and recent dockets. It is not legal advice and it publishes no bias scores. The judgefinder.io domain is being restored.
- **[MeshVault Harness](https://github.com/thefiredev-cloud/meshvault-harness)**: free MIT installer for a private AI agent on your own computer (Linux or Mac): Hermes, OMP, a local model, and 11 skills that stop for approval before they send, pay, post or delete. A 9-skill Pro pack is $99 and a done-for-you install is $499, both described at [thefiredev.com/harness](https://thefiredev.com/harness).
- **[TheFireDev](https://thefiredev.com)**: my consulting and freelance studio. It builds AI systems for small businesses: the model, the application, and the compute.

## What I work on

- Local LLM serving on NVIDIA DGX Spark clusters.
- Agent orchestration: one accountable coordinator, bounded specialist roles, and approval gates before real-world actions.
- Small, inspectable tools for agents: MCP servers, Claude Code plugins, and plain Markdown skills.

## Selected public work

- [meshvault-agentic-architecture](https://github.com/thefiredev-cloud/meshvault-agentic-architecture): reference architecture for MeshVault's mixture-of-agents loop, role orchestration, approval levels, and owned knowledge stack.
- [meshvault-skills-starter](https://github.com/thefiredev-cloud/meshvault-skills-starter): free MIT agent skills in plain Markdown, each with a written approval gate.
- [agent-ops-kit](https://github.com/thefiredev-cloud/agent-ops-kit): Claude Code plugin for evidence before claims, scrubbing data before sharing, and building private and public variants from one source.
- [eufy-camera-mcp](https://github.com/thefiredev-cloud/eufy-camera-mcp): MCP server that gives an agent view-only, allowlisted access to local cameras through MediaMTX.
- [meshvault-bot](https://github.com/thefiredev-cloud/meshvault-bot): self-hostable bot app on Hermes Agent with a sandboxed computer per bot (fork of Rakazo).
- [airpods-max-sidetone](https://github.com/thefiredev-cloud/airpods-max-sidetone): supervised PipeWire sidetone for AirPods Max on Linux.

Most product code is private. The repositories above are public and MIT or Apache-2.0 licensed.

## Contact

- [LinkedIn](https://www.linkedin.com/in/tannerosterkamp)
- Websites: [meshvault.ai](https://meshvault.ai) · [thefiredev.com](https://thefiredev.com)
- Consulting and freelance work: tanner@thefiredev.com
- Security reports: see [SECURITY.md](SECURITY.md). Please do not open public issues for vulnerabilities.
