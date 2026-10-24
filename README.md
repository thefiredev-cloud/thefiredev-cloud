# Tanner Osterkamp

Founder of [Mesh](https://meshvault.ai) and [TheFireDev](https://thefiredev.com). AI application engineer in Dana Point, California.

Mesh is a free iPhone app for your own AI assistant. It plans your day, explains a document and drafts a reply. Agents stop for a named person's approval before they send, pay, post, or delete.

## Products (status as of 2026-10-21)

- **[Mesh](https://meshvault.ai)**: the iPhone app is pre-release (TestFlight by invite, no App Store listing yet). Android is an early build, not on Google Play yet. Download details are at [meshvault.ai/download](https://meshvault.ai/download).
- **[The one-week install](https://meshvault.ai/install)**: a server you own, with Hermes Desktop and Mesh paired to it, and a backup that has passed a restore test. $4,950 fixed, 50% deposit.
- **[Protocol Guide](https://protocol-guide.com)**: source-cited EMS protocol search by county for students, educators and clinicians. Every result names the protocol book it came from. Education and reference only: not a medical device, not for bedside care. State and county protocol pages and the blog are open on the web. The iPhone app is submitted to App Review. The Android app is in development.
- **[JudgeFinder](https://judgefinder.io)**: free judge lookup built on CourtListener docket metadata, with no account. It shows court assignment, case volume and recent dockets. It is not legal advice and it publishes no bias scores.
- **[MeshVault Harness](https://github.com/thefiredev-cloud/meshvault-harness)**: a shell installer for Linux or macOS that sets up Hermes Agent, OMP and a local Qwen3 model, plus 11 free skills that each carry a written approval step. A 9-skill Pro pack is $99 and a done-for-you install is $499, both described at [thefiredev.com/harness](https://thefiredev.com/harness).
- **[TheFireDev](https://thefiredev.com)**: my consulting and freelance studio. It builds AI systems for small businesses: the model, the application, and the compute.

## What I work on

- Local LLM serving on NVIDIA DGX Spark clusters.
- Agent orchestration: one accountable coordinator, bounded specialist roles, and approval gates before real-world actions.
- Small, inspectable tools for agents: MCP servers, Claude Code plugins, and plain Markdown skills.

## Public repositories

Every repository below has a README that states what it does, what it needs and where it falls short, and a LICENSE file.

**Agents and MCP**

- [meshvault-harness](https://github.com/thefiredev-cloud/meshvault-harness): shell installer for Hermes Agent, OMP and a local Qwen3 model, with the full download list in its README.
- [meshvault-skills-starter](https://github.com/thefiredev-cloud/meshvault-skills-starter): nine MIT agent skills in plain Markdown for small business admin work, each with a written approval gate.
- [agent-ops-kit](https://github.com/thefiredev-cloud/agent-ops-kit): Claude Code plugin with three habits that keep an agent honest, including a deny-list scanner that fails a build when private strings survive.
- [agent-plugins](https://github.com/thefiredev-cloud/agent-plugins): plugin manifests, installers and rollback guards for a small agent tool set.
- [meshvault-agentic-architecture](https://github.com/thefiredev-cloud/meshvault-agentic-architecture): reference documents and diagrams for a mixture-of-agents loop, role orchestration and approval levels. Documentation only.
- [meshvault-product-plugins](https://github.com/thefiredev-cloud/meshvault-product-plugins): product plugins that expose site and tool surfaces to an agent over MCP.
- [eufy-camera-mcp](https://github.com/thefiredev-cloud/eufy-camera-mcp): MCP server that gives an agent view-only, allowlisted access to local cameras through MediaMTX.
- [mesh-rag](https://github.com/thefiredev-cloud/mesh-rag): shared scrape plus SQLite FTS5 retrieval for agents on one host.

**Desktop and fleet tools**

- [detent](https://github.com/thefiredev-cloud/detent): one Linux desktop panel for keyboard lighting, mouse DPI, per-output audio EQ, USB devices and controllers.
- [voice-orb](https://github.com/thefiredev-cloud/voice-orb): hands-free spoken assistant on a desktop hotkey, with model routing and a spoken reply.
- [modbay](https://github.com/thefiredev-cloud/modbay): game library and mod manager for a Linux desktop, built with no npm dependencies.
- [bar-plugin-audit](https://github.com/thefiredev-cloud/bar-plugin-audit): static audit that finds QML hazards in desktop bar plugins before they crash the shell.
- [airpods-max-sidetone](https://github.com/thefiredev-cloud/airpods-max-sidetone): PipeWire sidetone loopback for AirPods Max on Linux, active only while another app records the mic.
- [vram-pool](https://github.com/thefiredev-cloud/vram-pool): one OpenAI-compatible endpoint in front of every device that has VRAM.
- [modeldeck](https://github.com/thefiredev-cloud/modeldeck): local model inventory and guarded cluster swap review on one page.
- [meshvault-telemetry](https://github.com/thefiredev-cloud/meshvault-telemetry): Rust daemon that collects host health facts and publishes status files.
- [meshvault-bin](https://github.com/thefiredev-cloud/meshvault-bin) and [gx10-bin](https://github.com/thefiredev-cloud/gx10-bin): operator scripts, probes and CI gates in plain shell.
- [hearth-voice](https://github.com/thefiredev-cloud/hearth-voice): living-room voice assistant in an Echo Dot shell, backed by a local agent runtime.
- [mesh-orb-history](https://github.com/thefiredev-cloud/mesh-orb-history): macOS menu-bar panel for chat, voice and screen context over a local agent runtime.
- [meshvault-workspace](https://github.com/thefiredev-cloud/meshvault-workspace): pnpm workspace holding shared packages for one desktop product.
- [home-tools-web-workbench](https://github.com/thefiredev-cloud/home-tools-web-workbench): local web workbench for small home tools, with a QA harness.

**Media and local AI**

- [localclip](https://github.com/thefiredev-cloud/localclip): cuts a long talking video into captioned 9:16 clips with local models and ffmpeg.
- [localavatar](https://github.com/thefiredev-cloud/localavatar): builds talking-head videos from one photo and a script, on your own machine.
- [document-title-page-system](https://github.com/thefiredev-cloud/document-title-page-system): generates titled page systems and PDF covers from a small config.
- [meshvault-scroll](https://github.com/thefiredev-cloud/meshvault-scroll) and [cyberwing-local](https://github.com/thefiredev-cloud/cyberwing-local): scroll-film landing pages, one video timeline scrubbed by scroll.
- [meshchat-site-oneshot](https://github.com/thefiredev-cloud/meshchat-site-oneshot): a static landing page captured as one self-contained build.

**iPhone apps**

- [amphours](https://github.com/thefiredev-cloud/amphours): offline battery runtime calculator. Build a bank, see how long it lasts.
- [drawyears](https://github.com/thefiredev-cloud/drawyears): offline savings drawdown calculator.
- [edgeledger](https://github.com/thefiredev-cloud/edgeledger): offline probability sizer and forecast journal.
- [extraslip](https://github.com/thefiredev-cloud/extraslip): time and materials tickets for contractors, with a signature step.
- [pumpchart](https://github.com/thefiredev-cloud/pumpchart): medication timings at the bedside.

**Web**

- [mirofish](https://github.com/thefiredev-cloud/mirofish): multi-agent simulation engine with a knowledge graph backend and a FastAPI service.
- [nurse-buddy](https://github.com/thefiredev-cloud/nurse-buddy): study companion web app for nursing students.
- [octagon-bot](https://github.com/thefiredev-cloud/octagon-bot): financial research web app with a tool-using assistant.

**Forks, mirrors and plugins**

- [Reach](https://github.com/thefiredev-cloud/Reach): fork of a Tauri SSH client with macOS copy and paste, vault password and registry URL fixes. Upstream is canonical.
- [meshvault-bot](https://github.com/thefiredev-cloud/meshvault-bot): fork of Rakazo that runs a bot app on Hermes Agent with a sandboxed computer per bot.
- [hermes-agent](https://github.com/thefiredev-cloud/hermes-agent), [awesome-remote-mcp-servers](https://github.com/thefiredev-cloud/awesome-remote-mcp-servers), [awesome-medical-mcp-servers](https://github.com/thefiredev-cloud/awesome-medical-mcp-servers) and [awesome-gemini-cli-extensions](https://github.com/thefiredev-cloud/awesome-gemini-cli-extensions): mirrors with no changes of their own. Use the upstream repositories.
- [reach-plugins](https://github.com/thefiredev-cloud/reach-plugins) and [reach-plugins-registry](https://github.com/thefiredev-cloud/reach-plugins-registry): example Lua plugins and the plugin registry index for Reach.

Archived snapshots: [pc-desktop-amphours](https://github.com/thefiredev-cloud/pc-desktop-amphours) and [pc-desktop-drawyears](https://github.com/thefiredev-cloud/pc-desktop-drawyears) are working-tree copies of the two apps above. Use the maintained repositories.

## Contact

- [LinkedIn](https://www.linkedin.com/in/tannerosterkamp)
- Websites: [meshvault.ai](https://meshvault.ai) · [thefiredev.com](https://thefiredev.com)
- Mesh questions: contact@meshvault.ai. A person reads it and replies.
- Consulting and freelance work: tanner@thefiredev.com
- Security reports: see [SECURITY.md](SECURITY.md). Please do not open public issues for vulnerabilities.
