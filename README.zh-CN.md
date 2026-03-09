# AWEsome Multi-Agents Skills

> 面向 Autonomous World / Multi-Agent 的开源 Skill 索引

[![Awesome](https://awesome.re/badge-flat.svg)](https://awesome.re)
[![Skills](https://img.shields.io/badge/skills-17-brightgreen)](./skills/)
[![Dashboard](https://img.shields.io/badge/Dashboard-AWEsome%20Dashboard-blue)](https://awesome-dashboard-eight.vercel.app/)

## 关于

AWEsome Multi-Agents Skills 是一个结构化索引，收录的是**我们认可的、与 autonomous world / multi-agent 相关的 Skills、工具及生态内容**，同时面向 **人类阅读** 和 **机器消费**（Dashboard 自动抓取、AI 搜索与推荐）。

**数据结构：** 每个收录条目都会在 [`skills/`](./skills/) 下拥有一个 `entry.json`；Dashboard 会自动读取这些文件。当前索引采用：

- `type` 表示**这是什么类型的条目**：`skill`、`mcp`、`agent`、`framework`、`app`、`tool`、`protocol`、`model`、`other`
- `tags` 表示**这个条目涉及哪些主题或能力**：用于搜索、筛选与推荐

```text
skills/
└── <slug>/
    └── entry.json   ← 机器可读的结构化数据
```

> 若条目本身是 Skill，其实际 `SKILL.md` 文件通常位于对应项目仓库根目录；本仓库只维护索引。

---

## 智能体

- **agency-agents**: 收录 9 大分组、55+ 专业 AI Agent 的智能体合集，强调人格化工作流与 Claude Code 使用场景
  仓库：[msitarzewski/agency-agents](https://github.com/msitarzewski/agency-agents)
  类型：`agent`
  标签：`multi-agent`, `collaboration`, `coordination`
  数据：[entry.json](./skills/agency-agents/entry.json)

## Skills

- **privy-agentic-wallets-skill**: 面向 OpenClaw 的 Privy 智能体钱包 Skill，为 AI 智能体提供基于 Privy 的钱包与链上能力
  仓库：[privy-io/privy-agentic-wallets-skill](https://github.com/privy-io/privy-agentic-wallets-skill)
  类型：`skill`
  标签：`multi-agent`, `wallet`, `openclaw`, `skill`
  数据：[entry.json](./skills/privy-agentic-wallets-skill/entry.json)

- **gtm-engineer-skills**: 提升网站 AEO/GEO 的 Claude Code 技能 — 16 项检查、6 大智能维度与框架级优化
  仓库：[onvoyage-ai/gtm-engineer-skills](https://github.com/onvoyage-ai/gtm-engineer-skills)
  类型：`skill`
  标签：`gtm`, `tooling`, `distribution`
  数据：[entry.json](./skills/gtm-engineer-skills/entry.json)

- **obsidian-skills**: 面向 Obsidian 的 Agent 技能 — 让智能体使用 Markdown、Bases、JSON Canvas 与 CLI
  仓库：[kepano/obsidian-skills](https://github.com/kepano/obsidian-skills)
  类型：`skill`
  标签：`tooling`, `multi-agent`, `infrastructure`
  数据：[entry.json](./skills/obsidian-skills/entry.json)

- **evolver (Capability Evolver)**: 基于 GEP 的 AI 智能体自进化引擎 — 协议约束的进化、Genes/Capsules/Events、可审计链路，EvoMap 网络（evomap.ai）核心
  仓库：[EvoMap/evolver](https://github.com/EvoMap/evolver)
  类型：`skill`
  标签：`multi-agent`, `openclaw`, `protocol`, `tooling`
  数据：[entry.json](./skills/evolver/entry.json)

## 框架

- **AgentKit**: Coinbase 的 AI 智能体框架，为智能体提供钱包与链上能力
  仓库：[coinbase/agentkit](https://github.com/coinbase/agentkit)
  类型：`framework`
  标签：`multi-agent`, `tooling`, `infrastructure`
  数据：[entry.json](./skills/agentkit/entry.json)

- **CrewAI**: 在 Python 生态中最流行的多智能体编排框架之一，强调基于角色的代理设计（Role-playing agents），让多个 Agent 像团队一样协作完成复杂任务。
  仓库：[joaomdmoura/crewAI](https://github.com/joaomdmoura/crewAI)
  类型：`framework`
  标签：`multi-agent`, `orchestration`, `python`, `collaboration`
  数据：[entry.json](./skills/crewai/entry.json) *(精选)*

## 应用

- **edict**: 唐风启发的多智能体编排系统，包含 9 个专用 AI Agent 与实时看板
  仓库：[cft0808/edict](https://github.com/cft0808/edict)
  类型：`app`
  标签：`multi-agent`, `orchestration`, `dashboard`
  数据：[entry.json](./skills/edict/entry.json)

- **star-office-ui**: 像素风办公室仪表盘，用于多智能体协作与 Agent 状态可视化
  仓库：[ringhyacinth/Star-Office-UI](https://github.com/ringhyacinth/Star-Office-UI)
  类型：`app`
  标签：`multi-agent`, `visualization`, `dashboard`, `tooling`
  数据：[entry.json](./skills/star-office-ui/entry.json)

- **OpenMOSS**: 基于 OpenClaw 的自组织多智能体协作平台，规划、执行、评审、巡检全自动，零人工干预
  仓库：[uluckyXH/OpenMOSS](https://github.com/uluckyXH/OpenMOSS)
  类型：`app`
  标签：`multi-agent`, `orchestration`, `collaboration`, `dashboard`
  数据：[entry.json](./skills/openmoss/entry.json)

- **Claw Arena**: 面向 OpenClaw 的智能体原生游戏：像素风竞技场，智能体对战、下注代币、派发任务，支持浏览器与 OpenClaw API
  仓库：[aikoooly/Claw-Arena](https://github.com/aikoooly/Claw-Arena)
  类型：`app`
  标签：`multi-agent`, `openclaw`, `game`, `visualization`
  数据：[entry.json](./skills/claw-arena/entry.json)

- **ClawPort**: 面向 OpenClaw 的开源智能体指挥中心：组织图、对话（视觉/语音）、看板、Cron 监控、成本统计、活动控制台与记忆浏览
  仓库：[JohnRiceML/clawport-ui](https://github.com/JohnRiceML/clawport-ui)
  类型：`app`
  标签：`multi-agent`, `openclaw`, `dashboard`, `visualization`
  数据：[entry.json](./skills/clawport-ui/entry.json)

## 工具

- **agent-browser**: 面向 AI 智能体的浏览器自动化 CLI，支持导航、填表与截图等能力
  仓库：[vercel-labs/agent-browser](https://github.com/vercel-labs/agent-browser)
  类型：`tool`
  标签：`multi-agent`, `tooling`, `automation`, `cli`
  数据：[entry.json](./skills/agent-browser/entry.json)

- **Vercel Skills**: 开源 Agent Skills 工具：通过 CLI（如 npx skills add）发现与安装智能体 Skill，Vercel Labs 官方技能注册表
  仓库：[vercel-labs/skills](https://github.com/vercel-labs/skills)
  类型：`tool`
  标签：`multi-agent`, `tooling`, `skill`, `cli`
  数据：[entry.json](./skills/vercel-skills/entry.json)

- **Google Workspace CLI**: Drive、Gmail、Calendar、Sheets、Docs、Chat、Admin 等统一 CLI，含 AI Agent 技能
  仓库：[googleworkspace/cli](https://github.com/googleworkspace/cli)
  类型：`tool`
  标签：`infrastructure`, `cli`, `tooling`
  数据：[entry.json](./skills/googleworkspace-cli/entry.json)

## 协议层 (Protocols)

- **ERC-8004 Contracts**: 8004 团队维护的注册表合约 — 面向智能体与实体的链上注册基础设施
  仓库：[erc-8004/erc-8004-contracts](https://github.com/erc-8004/erc-8004-contracts)
  类型：`protocol`
  标签：`identity`, `infrastructure`, `protocol`
  数据：[entry.json](./skills/erc-8004-contracts/entry.json)

- **x402**: 面向互联网的支付协议，基于 HTTP — 接口按次付费、多网络（加密与法币）、服务端与客户端集成极简
  仓库：[coinbase/x402](https://github.com/coinbase/x402)
  类型：`protocol`
  标签：`payment`, `protocol`, `infrastructure`
  数据：[entry.json](./skills/x402/entry.json)

---

## 机器可读 API

Dashboard 和相关工具会按如下方式消费本仓库：

```text
# 获取单个条目
GET https://raw.githubusercontent.com/STPDevteam/AWEsome-Multi-Agents-Skills/main/skills/<slug>/entry.json

# 获取推荐标签组
GET https://raw.githubusercontent.com/STPDevteam/AWEsome-Multi-Agents-Skills/main/tag-groups.json
```

**`entry.json`** 字段说明：

```jsonc
{
  "slug": "your-skill-name",             // 唯一 id，需与目录名一致
  "name": "your-skill-name",             // 展示名称
  "description": "English description",  // 英文主描述，<= 120 chars
  "description_zh": "中文描述",           // 可选；面向中文用户与 AI 搜索，<= 80 chars
  "github": "owner/repo",                // 仓库路径（不要带 https://github.com/）
  "tags": ["multi-agent", "tooling"],    // 主题/能力标签；可参考 tag-groups.json
  "added": "2026-03-06",                 // 添加日期 YYYY-MM-DD
  "type": "framework",                   // 条目类型
  "featured": false                      // 是否精选（可选，默认 false）
}
```

**`tag-groups.json`** 现在保留为**推荐标签组词典**，供人类和工具参考；条目本身不再需要 `category` 字段。

---

## 发现类 Skill

### find-awe-skills

用于在本索引中查找并获取相关 Skill 推荐。

```bash
npx skills add awe-org/find-awe-skills
```

仓库： [awe-org/find-awe-skills](https://github.com/awe-org/find-awe-skills)

---

## 提交新 Skill

### 方式 1：Pull Request（推荐，会触发自动化）

1. Fork 本仓库。
2. 在 `skills/<your-slug>/` 下创建 `entry.json`。
3. 提交 PR，标题格式为：`feat: add <your-skill-name>`。
4. 合并后，Dashboard 会在下一次构建时自动收录。

### 方式 2：Issue

通过 [GitHub Issues](https://github.com/STPDevteam/AWEsome-Multi-Agents-Skills/issues/new?template=add-skill.yml) 提交；维护者可以代为添加该条目。

详情见 [CONTRIBUTING.md](./CONTRIBUTING.md)。

---

## 相关链接

- [Dashboard](https://awesome-dashboard-eight.vercel.app/) - Web UI
- [tag-groups.json](./tag-groups.json) - 推荐标签组

## License

MIT License
