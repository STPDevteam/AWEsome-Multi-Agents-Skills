# AWEsome Multi-Agents Skills

> Open-source Skill index for Autonomous World / Multi-Agent

[![Awesome](https://awesome.re/badge-flat.svg)](https://awesome.re)
[![Skills](https://img.shields.io/badge/skills-3-brightgreen)](./skills/)
[![Dashboard](https://img.shields.io/badge/Dashboard-AWEsome%20Dashboard-blue)](https://awesome-dashboard-eight.vercel.app/)

## About

AWEsome Multi-Agents Skills is a structured index of **Skills, tools, and related ecosystem resources that we recognize as relevant to autonomous world / multi-agent**, for both **human readers** and **machine consumption** (Dashboard auto-fetch, AI search and recommendations).

**Data structure:** Each listed entry has an `entry.json` under [`skills/`](./skills/); the Dashboard reads from these files automatically. The index now uses:

- `type` for **what the entry is**: `skill`, `mcp`, `agent`, `model`, `tool`, `other`
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

## Tools

- **edict**: Tang Dynasty-inspired multi-agent orchestration with 9 specialized AI agents and a real-time kanban
  Repo: [cft0808/edict](https://github.com/cft0808/edict)
  Type: `tool`
  Tags: `multi-agent`, `orchestration`, `dashboard`
  Data: [entry.json](./skills/edict/entry.json)

- **star-office-ui**: Pixel office dashboard for multi-agent collaboration and agent state visualization
  Repo: [ringhyacinth/Star-Office-UI](https://github.com/ringhyacinth/Star-Office-UI)
  Type: `tool`
  Tags: `multi-agent`, `visualization`, `dashboard`, `tooling`
  Data: [entry.json](./skills/star-office-ui/entry.json)

---

## Machine-readable API

The Dashboard and tooling consume this repo as follows:

```text
# Fetch one entry
GET https://raw.githubusercontent.com/STPDevteam/AWEsome-Multi-Agents-Skills/main/skills/<slug>/entry.json

# Fetch recommended tag groups
GET https://raw.githubusercontent.com/STPDevteam/AWEsome-Multi-Agents-Skills/main/categories.json
```

**entry.json** field reference:

```jsonc
{
  "slug": "your-skill-name",             // unique id, same as directory name
  "name": "your-skill-name",             // display name
  "description": "English description",  // primary description, ≤ 120 chars
  "description_zh": "中文描述",            // optional; for Chinese users & AI search, ≤ 80 chars
  "github": "owner/repo",                // repo path (no https://github.com/)
  "tags": ["multi-agent", "tooling"],    // topic/capability tags; see categories.json
  "added": "2026-03-06",                 // date added YYYY-MM-DD
  "type": "tool",                        // what the entry is
  "featured": false                      // featured flag (optional, default false)
}
```

**`categories.json`** is retained as a **recommended tag-group dictionary** for humans and tooling. Entries do **not** need a `category` field anymore.

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
- [categories.json](./categories.json) – Recommended tag groups

## License

MIT License
