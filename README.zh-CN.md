# AWEsome Multi-Agents Skills

> 面向 Autonomous World / Multi-Agent 的开源 Skill 索引

[![Awesome](https://awesome.re/badge-flat.svg)](https://awesome.re)
[![Skills](https://img.shields.io/badge/skills-3-brightgreen)](./skills/)
[![Dashboard](https://img.shields.io/badge/Dashboard-AWEsome%20Dashboard-blue)](https://awesome-dashboard-eight.vercel.app/)

## 关于

AWEsome Multi-Agents Skills 是一个结构化索引，收录的是**我们认可的、与 autonomous world / multi-agent 相关的 Skills、工具及生态内容**，同时面向 **人类阅读** 和 **机器消费**（Dashboard 自动抓取、AI 搜索与推荐）。

**数据结构：** 每个收录条目都会在 [`skills/`](./skills/) 下拥有一个 `entry.json`；Dashboard 会自动读取这些文件。当前索引采用：

- `type` 表示**这是什么类型的条目**：`skill`、`mcp`、`agent`、`model`、`tool`、`other`
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

## 工具

- **edict**: 唐风启发的多智能体编排系统，包含 9 个专用 AI Agent 与实时看板
  仓库：[cft0808/edict](https://github.com/cft0808/edict)
  类型：`tool`
  标签：`multi-agent`, `orchestration`, `dashboard`
  数据：[entry.json](./skills/edict/entry.json)

- **star-office-ui**: 像素风办公室仪表盘，用于多智能体协作与 Agent 状态可视化
  仓库：[ringhyacinth/Star-Office-UI](https://github.com/ringhyacinth/Star-Office-UI)
  类型：`tool`
  标签：`multi-agent`, `visualization`, `dashboard`, `tooling`
  数据：[entry.json](./skills/star-office-ui/entry.json)

---

## 机器可读 API

Dashboard 和相关工具会按如下方式消费本仓库：

```text
# 获取单个条目
GET https://raw.githubusercontent.com/STPDevteam/AWEsome-Multi-Agents-Skills/main/skills/<slug>/entry.json

# 获取推荐标签组
GET https://raw.githubusercontent.com/STPDevteam/AWEsome-Multi-Agents-Skills/main/categories.json
```

**`entry.json`** 字段说明：

```jsonc
{
  "slug": "your-skill-name",             // 唯一 id，需与目录名一致
  "name": "your-skill-name",             // 展示名称
  "description": "English description",  // 英文主描述，<= 120 chars
  "description_zh": "中文描述",           // 可选；面向中文用户与 AI 搜索，<= 80 chars
  "github": "owner/repo",                // 仓库路径（不要带 https://github.com/）
  "tags": ["multi-agent", "tooling"],    // 主题/能力标签；可参考 categories.json
  "added": "2026-03-06",                 // 添加日期 YYYY-MM-DD
  "type": "tool",                        // 条目类型
  "featured": false                      // 是否精选（可选，默认 false）
}
```

**`categories.json`** 现在保留为**推荐标签组词典**，供人类和工具参考；条目本身不再需要 `category` 字段。

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
- [categories.json](./categories.json) - 推荐标签组

## License

MIT License
