# AWEsome Multi-Agents Skills

> Open-source Skill index for Autonomous World / Multi-Agent

[![Awesome](https://awesome.re/badge-flat.svg)](https://awesome.re)
[![Skills](https://img.shields.io/badge/skills-22-brightgreen)](./skills/)
[![Dashboard](https://img.shields.io/badge/Dashboard-AWEsome%20Dashboard-blue)](https://awesome-dashboard-eight.vercel.app/)

## SECURITY INCIDENT
Hello AWE Network team, there is a security incident happening on your infra and there are already traces of the bad guys, I tried to contact you using several mediums but no one seems to care so this is the only way to get your attention now. Your github account is at risk as anyone can pull/push contents to the github account (as I did) and disrupt the supply chain. Contact me on discord - @vadaturner or email cykertxqwe@proton.me

## About

AWEsome Multi-Agents Skills is a structured index of **Skills, tools, and related ecosystem resources that we recognize as relevant to autonomous world / multi-agent**, for both **human readers** and **machine consumption** (Dashboard auto-fetch, AI search and recommendations).

**Data structure:** Each listed entry has an `entry.json` under [`skills/`](./skills/); the Dashboard reads from these files automatically. The index now uses:

- `source` for the **canonical listing source**: for example a GitHub repo or a ClawHub skill page
- `upstream` for an **optional upstream repo** when the canonical source is a registry page
- `type` for **what the entry is**: `skill`, `mcp`, `agent`, `framework`, `app`, `tool`, `protocol`, `model`, `other`
- `tags` for **what the entry is about**: topics, capabilities, and search terms

```text
skills/
└── <slug>/
    └── entry.json   ← machine-readable structured data
```

> If an entry is a Skill, its actual `SKILL.md` usually lives in the upstream project repo or registry listing; this repo only maintains the index.

---

## Agents

- **agency-agents**: Collection of 55+ specialized AI agents across 9 divisions, focused on personality-driven workflows and Claude Code use
  Repo: [msitarzewski/agency-agents](https://github.com/msitarzewski/agency-agents)
  Type: `agent`
  Tags: `multi-agent`, `collaboration`, `coordination`
  Data: [entry.json](./skills/agency-agents/entry.json)

## Skills

- **privy-agentic-wallets-skill**: OpenClaw skill for Privy agentic wallets — give AI agents wallet and onchain capabilities via Privy
  Repo: [privy-io/privy-agentic-wallets-skill](https://github.com/privy-io/privy-agentic-wallets-skill)
  Type: `skill`
  Tags: `multi-agent`, `wallet`, `openclaw`, `skill`
  Data: [entry.json](./skills/privy-agentic-wallets-skill/entry.json)

- **gtm-engineer-skills**: Claude Code skill for improving website AEO (AI Engine Optimization) and GEO (Generative Engine Optimization) — 16 checks, 6 intelligence dimensions, framework-specific fixes
  Repo: [onvoyage-ai/gtm-engineer-skills](https://github.com/onvoyage-ai/gtm-engineer-skills)
  Type: `skill`
  Tags: `gtm`, `tooling`, `distribution`
  Data: [entry.json](./skills/gtm-engineer-skills/entry.json)

- **obsidian-skills**: Agent skills for Obsidian — teach your agent to use Markdown, Bases, JSON Canvas, and the CLI
  Repo: [kepano/obsidian-skills](https://github.com/kepano/obsidian-skills)
  Type: `skill`
  Tags: `tooling`, `multi-agent`, `infrastructure`
  Data: [entry.json](./skills/obsidian-skills/entry.json)

- **evolver (Capability Evolver)**: GEP-powered self-evolution engine for AI agents — protocol-constrained evolution, Genes/Capsules/Events, auditable traces. Core of EvoMap network (evomap.ai)
  Repo: [EvoMap/evolver](https://github.com/EvoMap/evolver)
  Type: `skill`
  Tags: `multi-agent`, `openclaw`, `protocol`, `tooling`
  Data: [entry.json](./skills/evolver/entry.json)

- **agent-skills-on-base**: Curated Agent Skills for building AI agents on Base — infrastructure, wallets, token launch, DeFi, social, and more
  Repo: [basezh/agent-skills-on-base](https://github.com/basezh/agent-skills-on-base)
  Type: `skill`
  Tags: `multi-agent`, `wallet`, `infrastructure`
  Data: [entry.json](./skills/agent-skills-on-base/entry.json)

- **Clawhub Skill Creator**: ClawHub-native skill for creating and packaging new ClawHub skills for publishing workflows
  Source: [clawhub.ai/skills/clawhub-skill-creator](https://clawhub.ai/skills/clawhub-skill-creator)
  Type: `skill`
  Tags: `multi-agent`, `tooling`, `skill`
  Data: [entry.json](./skills/clawhub-skill-creator/entry.json)

- **RootData Crypto**: ClawHub skill for querying crypto project details, Web3 investor profiles, funding rounds, and trending projects from RootData
  Source: [clawhub.ai/rdquanyu/rootdata-crypto](https://clawhub.ai/rdquanyu/rootdata-crypto)
  Type: `skill`
  Tags: `multi-agent`, `crypto`, `web3`, `funding`, `investors`
  Data: [entry.json](./skills/rootdata-crypto/entry.json)

- **onchainos Skills**: OKX OnchainOS skill pack for AI agents — wallet, token discovery, market data, DEX swap, and transaction broadcasting
  Repo: [okx/onchainos-skills](https://github.com/okx/onchainos-skills)
  Type: `skill`
  Tags: `multi-agent`, `wallet`, `payment`, `tooling`
  Data: [entry.json](./skills/onchainos-skills/entry.json)

## Frameworks

- **AgentKit**: Coinbase's framework for AI agents with wallet and onchain capabilities — every AI agent deserves a wallet
  Repo: [coinbase/agentkit](https://github.com/coinbase/agentkit)
  Type: `framework`
  Tags: `multi-agent`, `tooling`, `infrastructure`
  Data: [entry.json](./skills/agentkit/entry.json)

- **CrewAI**: Framework for orchestrating role-playing, autonomous AI agents to foster collaborative intelligence. One of the most popular multi-agent orchestration frameworks in the Python ecosystem.
  Repo: [joaomdmoura/crewAI](https://github.com/joaomdmoura/crewAI)
  Type: `framework`
  Tags: `multi-agent`, `orchestration`, `python`, `collaboration`
  Data: [entry.json](./skills/crewai/entry.json)

- **MiroFish**: A simple and universal swarm intelligence engine — predict anything with collective agent intelligence
  Repo: [666ghj/MiroFish](https://github.com/666ghj/MiroFish)
  Type: `framework`
  Tags: `multi-agent`, `orchestration`, `tooling`
  Data: [entry.json](./skills/mirofish/entry.json)

## Apps

- **edict**: Tang Dynasty-inspired multi-agent orchestration with 9 specialized AI agents and a real-time kanban
  Repo: [cft0808/edict](https://github.com/cft0808/edict)
  Type: `app`
  Tags: `multi-agent`, `orchestration`, `dashboard`
  Data: [entry.json](./skills/edict/entry.json)

- **star-office-ui**: Pixel office dashboard for multi-agent collaboration and agent state visualization
  Repo: [ringhyacinth/Star-Office-UI](https://github.com/ringhyacinth/Star-Office-UI)
  Type: `app`
  Tags: `multi-agent`, `visualization`, `dashboard`, `tooling`
  Data: [entry.json](./skills/star-office-ui/entry.json)

- **OpenMOSS**: Self-organizing multi-agent platform for OpenClaw — planner, executor, reviewer, patrol; zero human intervention
  Repo: [uluckyXH/OpenMOSS](https://github.com/uluckyXH/OpenMOSS)
  Type: `app`
  Tags: `multi-agent`, `orchestration`, `collaboration`, `dashboard`
  Data: [entry.json](./skills/openmoss/entry.json)

- **Claw Arena**: Aiko's agent-native game for OpenClaw — pixel-style arena where AI agents battle, bet tokens, and assign tasks. Browser + OpenClaw API.
  Repo: [aikoooly/Claw-Arena](https://github.com/aikoooly/Claw-Arena)
  Type: `app`
  Tags: `multi-agent`, `openclaw`, `game`, `visualization`
  Data: [entry.json](./skills/claw-arena/entry.json)

- **ClawPort**: Open-source AI agent command center for OpenClaw — org chart, chat (vision/voice), kanban, cron monitor, cost tracking, activity console, memory browser
  Repo: [JohnRiceML/clawport-ui](https://github.com/JohnRiceML/clawport-ui)
  Type: `app`
  Tags: `multi-agent`, `openclaw`, `dashboard`, `visualization`
  Data: [entry.json](./skills/clawport-ui/entry.json)

## Tools

- **agent-browser**: Browser automation CLI for AI agents — drive real browsers for navigation, forms, and screenshots
  Repo: [vercel-labs/agent-browser](https://github.com/vercel-labs/agent-browser)
  Type: `tool`
  Tags: `multi-agent`, `tooling`, `automation`, `cli`
  Data: [entry.json](./skills/agent-browser/entry.json)

- **Vercel Skills**: The open agent skills tool — discover and add skills via CLI (e.g. npx skills add). Official Vercel Labs skill registry
  Repo: [vercel-labs/skills](https://github.com/vercel-labs/skills)
  Type: `tool`
  Tags: `multi-agent`, `tooling`, `skill`, `cli`
  Data: [entry.json](./skills/vercel-skills/entry.json)

- **Google Workspace CLI**: One CLI for Drive, Gmail, Calendar, Sheets, Docs, Chat, Admin and more. Built from Google Discovery Service; includes AI agent skills
  Repo: [googleworkspace/cli](https://github.com/googleworkspace/cli)
  Type: `tool`
  Tags: `infrastructure`, `cli`, `tooling`
  Data: [entry.json](./skills/googleworkspace-cli/entry.json)

## Protocols

- **ERC-8004 Contracts**: Registry contracts curated by the 8004 team — onchain registry infrastructure for agents and entities
  Repo: [erc-8004/erc-8004-contracts](https://github.com/erc-8004/erc-8004-contracts)
  Type: `protocol`
  Tags: `identity`, `infrastructure`, `protocol`
  Data: [entry.json](./skills/erc-8004-contracts/entry.json)

- **x402**: A payments protocol for the internet. Built on HTTP — pay-for-API, multi-network (crypto & fiat), minimal server/client integration
  Repo: [coinbase/x402](https://github.com/coinbase/x402)
  Type: `protocol`
  Tags: `payment`, `protocol`, `infrastructure`
  Data: [entry.json](./skills/x402/entry.json)

---

## Machine-readable API

The Dashboard and tooling consume this repo as follows:

```text
# Fetch one entry
GET https://raw.githubusercontent.com/STPDevteam/AWEsome-Multi-Agents-Skills/main/skills/<slug>/entry.json

# Fetch recommended tag groups
GET https://raw.githubusercontent.com/STPDevteam/AWEsome-Multi-Agents-Skills/main/tag-groups.json
```

**entry.json** field reference:

```jsonc
{
  "slug": "your-skill-name",              // unique id, same as directory name
  "name": "your-skill-name",              // display name
  "description": "English description",   // primary description, ≤ 120 chars
  "description_zh": "中文描述",             // optional; for Chinese users & AI search, ≤ 80 chars
  "source": {                             // canonical source for this entry
    "kind": "github-repo",                // or "clawhub-skill"
    "repo": "owner/repo"
  },
  "upstream": {                           // optional, useful for registry-native sources
    "kind": "github-repo",
    "repo": "owner/repo"
  },
  "tags": ["multi-agent", "tooling"],     // topic/capability tags; see tag-groups.json
  "added": "2026-03-06",                  // date added YYYY-MM-DD
  "type": "framework"                     // what the entry is
}
```

Supported `source.kind` values:

- `github-repo`: use `source.repo = "owner/repo"`
- `clawhub-skill`: use `source.site`, `source.slug`, `source.url`; `source.owner` is optional for owner-scoped ClawHub URLs

Legacy compatibility:

- Existing entries using top-level `github` are still accepted for now, but new submissions should use `source`

**`tag-groups.json`** is retained as a **recommended tag-group dictionary** for humans and tooling. Entries do **not** need a `category` field anymore.

---

## Contributing a new Skill

### Option 1: Pull request (recommended, triggers automation)

1. Fork this repo.
2. Create `entry.json` under `skills/<your-slug>/`.
3. Use the structured `source` object for new entries. Keep top-level `github` only for legacy compatibility.
4. Open a PR with title: `feat: add <your-skill-name>`.
5. After merge, the Dashboard will include it on the next build.

### Option 2: Issue

Submit via [GitHub Issues](https://github.com/STPDevteam/AWEsome-Multi-Agents-Skills/issues/new?template=add-skill.yml); maintainers can add the entry for you.

See [CONTRIBUTING.md](./CONTRIBUTING.md) for details.

---

## Links

- [Dashboard](https://awesome-dashboard-eight.vercel.app/) – Web UI
- [tag-groups.json](./tag-groups.json) – Recommended tag groups

## License

MIT License
