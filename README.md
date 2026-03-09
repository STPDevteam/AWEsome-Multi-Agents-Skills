# AWEsome Multi-Agents Skills

> Open-source Skill index for Autonomous World / Multi-Agent

[![Awesome](https://awesome.re/badge-flat.svg)](https://awesome.re)
[![Skills](https://img.shields.io/badge/skills-7-brightgreen)](./skills/)
[![Dashboard](https://img.shields.io/badge/Dashboard-AWEsome%20Dashboard-blue)](https://awesome-dashboard-eight.vercel.app/)

## About

AWEsome Multi-Agents Skills is a structured index of **Skills, tools, and related ecosystem resources that we recognize as relevant to autonomous world / multi-agent**, for both **human readers** and **machine consumption** (Dashboard auto-fetch, AI search and recommendations).

**Data structure:** Each listed entry has an `entry.json` under [`skills/`](./skills/); the Dashboard reads from these files automatically. The index now uses:

- `type` for **what the entry is**: `skill`, `mcp`, `agent`, `framework`, `app`, `tool`, `model`, `other`
- `tags` for **what the entry is about**: topics, capabilities, and search terms

```text
skills/
└── <slug>/
    └── entry.json   ← machine-readable structured data
```

> If an entry is a Skill, its actual `SKILL.md` usually lives in **that project's repo root**; this repo only maintains the index.

---

## Agents

- **agency-agents**: Collection of 55+ specialized AI agents across 9 divisions, focused on personality-driven workflows and Claude Code use
  Repo: [msitarzewski/agency-agents](https://github.com/msitarzewski/agency-agents)
  Type: `agent`
  Tags: `multi-agent`, `collaboration`, `coordination`
  Data: [entry.json](./skills/agency-agents/entry.json)

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
  Data: [entry.json](./skills/crewai/entry.json) *(featured)*

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

## Tools

- **agent-browser**: Browser automation CLI for AI agents — drive real browsers for navigation, forms, and screenshots
  Repo: [vercel-labs/agent-browser](https://github.com/vercel-labs/agent-browser)
  Type: `tool`
  Tags: `multi-agent`, `tooling`, `automation`, `cli`
  Data: [entry.json](./skills/agent-browser/entry.json)

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
  "slug": "your-skill-name",             // unique id, same as directory name
  "name": "your-skill-name",             // display name
  "description": "English description",  // primary description, ≤ 120 chars
  "description_zh": "中文描述",            // optional; for Chinese users & AI search, ≤ 80 chars
  "github": "owner/repo",                // repo path (no https://github.com/)
  "tags": ["multi-agent", "tooling"],    // topic/capability tags; see tag-groups.json
  "added": "2026-03-06",                 // date added YYYY-MM-DD
  "type": "framework",                   // what the entry is
  "featured": false                      // featured flag (optional, default false)
}
```

**`tag-groups.json`** is retained as a **recommended tag-group dictionary** for humans and tooling. Entries do **not** need a `category` field anymore.

---

## Contributing a new Skill

### Option 1: Pull request (recommended, triggers automation)

1. Fork this repo.
2. Create `entry.json` under `skills/<your-slug>/`.
3. Open a PR with title: `feat: add <your-skill-name>`.
4. After merge, the Dashboard will include it on the next build.

### Option 2: Issue

Submit via [GitHub Issues](https://github.com/STPDevteam/AWEsome-Multi-Agents-Skills/issues/new?template=add-skill.yml); maintainers can add the entry for you.

See [CONTRIBUTING.md](./CONTRIBUTING.md) for details.

---

## Links

- [Dashboard](https://awesome-dashboard-eight.vercel.app/) – Web UI
- [tag-groups.json](./tag-groups.json) – Recommended tag groups

## License

MIT License
