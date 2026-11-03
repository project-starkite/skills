# Starkite Agent Skills

Official agent skill definitions for the [Starkite](https://github.com/project-starkite/starkite) automation DSL.

These skills teach autonomous AI coding agents (Claude Code, Cursor, Antigravity, Robo) how to author secure, idiomatic, sandboxed Starkite scripts for infrastructure, operations, and Kubernetes tasks.

---

## Available Skills

| Skill | Directory | Description |
|---|---|---|
| **`starkite`** | `skills/starkite/` | Complete Starkite automation DSL (all built-in standard modules). |
| **`starkite-k8s`** | `skills/starkite-k8s/` | Specialized Kubernetes cluster operations and triage. |
| **`starkite-cloud`** | `skills/starkite-cloud/` | HTTP APIs, cloud services, and concurrent task pipelines. |

---

## Installation

### 1. Universal Skills CLI (`npx skills`)
Install skills directly into your workspace:

```bash
# Add all Starkite skills to your current workspace:
npx skills add project-starkite/skills

# Add only the Kubernetes automation skill:
npx skills add project-starkite/skills --skill starkite-k8s
```

### 2. Claude Code Plugin Marketplace
Add the Starkite skills repository to your Claude Code configuration:

```bash
/plugin marketplace add project-starkite/skills
/plugin install starkite@project-starkite
```

### 3. Cursor & Antigravity IDE
Copy the desired skill directory to `.cursor/skills/` or `.agent/skills/`:

```bash
mkdir -p .agent/skills/starkite
curl -sSL https://raw.githubusercontent.com/project-starkite/skills/main/skills/starkite/SKILL.md \
  -o .agent/skills/starkite/SKILL.md
```

---

## License

Apache-2.0. Copyright (c) 2026 Starkite Authors.
