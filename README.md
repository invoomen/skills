# invoomen/skills

A Claude Skills package that exposes Invoomen as slash commands. After
installing, you get `/invoomen:generate`, `/invoomen:status`, and
`/invoomen:characters` inside any Claude Desktop conversation.

## Install

```bash
npx skills add invoomen/skills
```

The skill ships with a reference to the Invoomen MCP server. You also need an
Invoomen API key — easiest path is:

```bash
npm install -g @invoomen/cli
invoomen auth login
```

The CLI writes your key to `~/.invoomen/config.json`. The skill picks it up
automatically.

## Slash commands

| Command | What it does |
|---|---|
| `/invoomen:generate <prompt>` | Generate an image/video/music/audio. The skill picks a model unless you specify one. |
| `/invoomen:status` | Shows credit balance and recent generations. |
| `/invoomen:characters` | Lists saved characters and elements (referenced by `@name` in prompts). |

## What's inside

- `skill.yaml` — package metadata
- `commands/` — three Markdown files, one per slash command, each with the
  prompt Claude follows when the command is invoked

## Source

Published copy: [github.com/invoomen/skills](https://github.com/invoomen/skills).

This directory inside the main Invoomen repo is the editing source — push
changes to the standalone repo with `node scripts/publish-external-repo.mjs
skills invoomen/skills` (force-pushes a fresh snapshot).

## License

MIT
