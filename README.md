# Tanner Osterkamp

Founder of [Kodros](https://kodros.ai). Firefighter-paramedic in Orange County, California.

I build private AI that runs on hardware you own: a home inference cluster, the agents and MCP servers on top of it, and the iPhone, web and desktop apps people use to reach it. I also build public-safety software, including EMS protocol search for medics.

## The Kodros stack

```mermaid
flowchart LR
  subgraph Clients
    P[iPhone and Watch apps, SwiftUI]
    D[Desktop: Hermes Desktop, OMP, Claude Code]
    W[Product web apps: Next.js on Vercel]
  end
  subgraph Hub[Home hub: Linux workstation, RTX 4080]
    G[Hermes Agent gateway]
    M[MCP servers and agent skills]
    V[vram-pool router, ModelDeck]
    S[Security watchtower]
  end
  subgraph Cluster[GB10 pair: DGX Spark + Ascent GX10]
    E[OpenAI-compatible engine, tensor parallel over 200 Gb/s RoCE]
  end
  P & D -->|private mesh VPN| G
  W --> X[(Supabase and Stripe)]
  G --> M
  G --> V
  V --> E
  V --> L[Local GPU models]
```

Phones and desktops talk to one hub over a private VPN. The hub runs the agent gateway, MCP tools and a router that picks which machine serves each model. The big model runs across two GB10 machines, so the agent path needs no hosted model. The product sites run separately on Vercel with Supabase and Stripe.

## Public repositories

| Repo | What it is |
|---|---|
| [kodros-lattice-wildfire](https://github.com/thefiredev-cloud/kodros-lattice-wildfire) | Five wildfire apps on Anduril's Lattice SDK: public fire feeds, fusion, recon planning, local-model briefs. Python. |
| [kodros-vram-pool](https://github.com/thefiredev-cloud/kodros-vram-pool) | One OpenAI-compatible endpoint in front of every machine with GPU memory, with failover and a hot-swap slot. Rust. |
| [kodros-gb10-deepseek-tp2](https://github.com/thefiredev-cloud/kodros-gb10-deepseek-tp2) | DeepSeek-V4.1-Flash across a DGX Spark and an Ascent GX10: settings, watchdogs and measured throughput. |
| [kodros-mac-cu](https://github.com/thefiredev-cloud/kodros-mac-cu) | Swift CLI that lets an AI agent click, type and read any Mac app through the accessibility tree. |
| [agent-ops-kit](https://github.com/thefiredev-cloud/agent-ops-kit) | Claude Code plugin: evidence before claims, and a scanner that fails a build when private data is left in. |
| [eufy-camera-mcp](https://github.com/thefiredev-cloud/eufy-camera-mcp) | MCP server with view-only access to an allowlist of local cameras. |
| [kodros-modeldeck](https://github.com/thefiredev-cloud/kodros-modeldeck) | Local model fleet dashboard with a three-check gate on cluster model swaps. |
| [kodros-sec-edgar-mcp](https://github.com/thefiredev-cloud/kodros-sec-edgar-mcp) | Read-only MCP server for SEC filings; every number cites its filing. |
| [kodros-search-console-mcp](https://github.com/thefiredev-cloud/kodros-search-console-mcp) | MCP server for Google Search Console with confirm-gated writes and a state-checked OAuth sign-in. |
| [kodros-bot](https://github.com/thefiredev-cloud/kodros-bot) | Self-hostable bot app on Hermes Agent, one computer per bot. Fork of Rakazo. |

Also: [airpods-max-sidetone](https://github.com/thefiredev-cloud/airpods-max-sidetone) (PipeWire sidetone for AirPods Max), [reach-plugins](https://github.com/thefiredev-cloud/reach-plugins) and [reach-plugins-registry](https://github.com/thefiredev-cloud/reach-plugins-registry) (Reach SSH client), and forks of [Reach](https://github.com/thefiredev-cloud/Reach) and [hermes-agent](https://github.com/thefiredev-cloud/hermes-agent), where upstream is canonical.

## Products

- [Kodros](https://kodros.ai): your business on a server you own, with AI agents that ask a named person before anything is sent, paid, posted or changed. iPhone app in TestFlight beta.
- [Protocol Guide](https://protocol-guide.com): EMS protocol search by county. Every answer names its protocol book. Education and reference only.
- [JudgeFinder](https://judgefinder.io): federal judge and docket search on public CourtListener data. Not legal advice.
- [AmpHours](https://apps.apple.com/us/app/amphours-battery-runtime/id6819963364): offline battery runtime calculator for iPhone, on the App Store.

Product source for these stays private. The full list with status is in the [portfolio](https://github.com/thefiredev-cloud/.github/blob/main/profile/README.md).

## Contact

[tanner@kodros.ai](mailto:tanner@kodros.ai) · [LinkedIn](https://www.linkedin.com/in/tannerosterkamp) · Security reports: [SECURITY.md](SECURITY.md)
