# Vicoa Agent Skills

A collection of agent skills for [Vicoa](https://vicoa.ai) products.

## Included Skills

- `live-preview`: Start a local dev service, reuse an occupied port when it belongs to the same project/service, expose it through Cloudflare/ngrok tunnel, and return structured Markdown fields for integration.

## Repository Layout

```text
agent-skills/
  skills/
    live-preview/
      SKILL.md
```

## Install

### Option 1: via skills installer

```bash
npx skills add vicoa-ai/agent-skills
```

Then select `live-preview` when prompted.

### Option 2: manual install (project-local)

```bash
mkdir -p .claude/skills/live-preview
cp -R skills/live-preview/* .claude/skills/live-preview/
```

### Option 3: manual install (global)

```bash
mkdir -p ~/.claude/skills/live-preview
cp -R skills/live-preview/* ~/.claude/skills/live-preview/
```

## Usage

In Claude Code, invoke the `live-preview` skill and optionally pass args such as run command, port, or tunnel provider.
