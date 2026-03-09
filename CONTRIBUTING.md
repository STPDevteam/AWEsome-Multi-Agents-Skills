# Contributing

Welcome to contributing new Skills to AWEsome Multi-Agents Skills!

## Data structure

This repo uses a **structured index**:

- Each Skill has machine-readable metadata in `skills/<slug>/entry.json`
- The actual `SKILL.md` files live in each project’s repo root and **are not stored here**
- The Dashboard (AWEsome Dashboard) reads from `entry.json` automatically
- The index uses `type` for entry shape and `tags` for topics/capabilities

```
AWEsome-Multi-Agents-Skills/
├── skills/
│   ├── edict/
│   │   └── entry.json
│   └── star-office-ui/
│       └── entry.json
├── tag-groups.json
├── README.md
└── CONTRIBUTING.md
```

---

## Option 1: Pull request (recommended)

After your PR is merged, the Dashboard will pick up the new Skill on the next build; **no need to update the README by hand**.

### Steps

**1. Fork this repo**

**2. Create entry.json**

```bash
mkdir -p skills/<your-slug>
```

Add `skills/<your-slug>/entry.json` with (**English is the primary language**; Chinese is optional):

```json
{
  "slug": "your-skill-name",
  "name": "your-skill-name",
  "description": "English description (primary, ≤ 120 chars)",
  "description_zh": "中文描述（可选，80 字以内）",
  "github": "owner/repo",
  "tags": ["multi-agent"],
  "added": "2026-03-06",
  "type": "tool"
}
```

**3. Open a PR**

- Title format: `feat: add <your-skill-name>`
- In the PR description, explain why this Skill is recommended

**4. Automated checks**

CI will run `validate-entry` and check:

- `entry.json` is valid (required fields present)
- `github` points to a public repo
- Repo root contains a `SKILL.md` file

---

## Option 2: Issue

If you prefer not to send a PR, you can submit an issue:

[Open Add Skill issue →](https://github.com/STPDevteam/AWEsome-Multi-Agents-Skills/issues/new?template=add-skill.yml)

Maintainers can create the `entry.json` and update the index for you.

---

## entry.json field reference

| Field | Type | Required | Description |
|-------|------|----------|-------------|
| `slug` | string | ✅ | Unique id, lowercase + hyphens, same as directory name |
| `name` | string | ✅ | Display name |
| `description` | string | ✅ | **Primary (English) description**, ≤ 120 chars |
| `description_zh` | string | — | **Optional Chinese description**, ≤ 80 chars |
| `github` | string | ✅ | `owner/repo`, without `https://github.com/` |
| `tags` | string[] | ✅ | At least one topic/capability tag; see `tag-groups.json` |
| `added` | string | ✅ | Date added, `YYYY-MM-DD` |
| `type` | string | ✅ | Entry type: `skill`, `mcp`, `agent`, `framework`, `app`, `tool`, `protocol`, `model`, `other` |

## Recommended tags

See [`tag-groups.json`](./tag-groups.json) for recommended tag groups. Summary:

| Tag group | Example tags |
|----------|----------------|
| Infrastructure | `infrastructure` `tooling` `protocol` `cli` |
| Multi-Agent | `multi-agent` `orchestration` `collaboration` `coordination` `benchmark` |
| Visualization | `visualization` `dashboard` `monitoring` |
| Go-to-Market | `gtm` `marketing` `distribution` |
| Identity | `identity` `auth` `wallet` `did` |
| Payment | `payment` `transaction` `transfer` |

## Repo requirements

- Repo must be **public**
- Repo root must have `SKILL.md` with frontmatter including `name` and `description`
- Project must be **actively maintained** (not archived)

## Review criteria

- Skill must be relevant to AWE / Autonomous World / Multi-Agent
- Descriptions must be clear so that AI can recommend the Skill when appropriate
- Avoid listing multiple Skills that do the same thing
