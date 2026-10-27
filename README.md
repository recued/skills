# Recued skills

Agent skills for working with [Recued](https://recued.com), a server you run on a computer you
control. It keeps your notes, tasks, mail, calendar and the things you own, and it stands between
your data and any AI: it checks every request against what you granted, asks you before a change,
and keeps a record of what was done.

| Skill | What it does |
|---|---|
| [`recued`](skills/recued/SKILL.md) | Tells an AI app how to work with Recued's MCP tools: reads run at once, and a change waits for your approval in Recued. |

The skill follows the [Agent Skills](https://agentskills.io) format, so it works in any app that
reads `SKILL.md` files. It installs nothing and runs no commands.

## Install

With the [skills CLI](https://skills.sh):

```sh
npx skills add recued/skills
```

Or copy [`skills/recued`](skills/recued) into your app's skills folder, for example
`~/.claude/skills/recued` for Claude Code.

The skill does not connect your app to Recued. To connect it, make a contract for the app in the
Recued web app and follow the contract's Connect tab, which shows the setup for Claude Desktop,
Claude Code, Cursor, Cline, Codex, OpenClaw and other AI apps.

Also available for OpenClaw on [ClawHub](https://clawhub.ai/recued/skills/recued), and for
DeepSeek Harness as the [`dsh-recued`](https://github.com/recued/dsh-recued) plugin.

## License

MIT
