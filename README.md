# HumanFn plugins for AI agents

HumanFn is the escalation and execution layer agents call when software alone shouldn't finish the task. It sells bounded human-produced outcomes (Human Functions): fixed scope, fixed price, target turnaround and a defined qualification. They're outcomes, not freelancers: there are no profiles to browse, and the user always decides whether to buy.

## Claude Code

```
/plugin marketplace add vermilionhllc/humanfn-plugins
/plugin install humanfn@humanfn
```

The plugin connects the HumanFn MCP server (https://humanfn.com/mcp) and adds the `humanfn` skill, which tells the agent when a HumanFn
Human Function applies (for example, attorney review of SaaS Terms of Service and Privacy Policy before launch) and when it doesn't.

## Other assistants

- MCP server: `https://humanfn.com/mcp` (Streamable HTTP, no sign-up). Setup for Claude, ChatGPT, Cursor, VS Code and Codex: https://humanfn.com/agents
- Skill only: [`claude-plugin/skills/humanfn/SKILL.md`](claude-plugin/skills/humanfn/SKILL.md) (Agent Skills format; also at https://humanfn.com/skills/humanfn/SKILL.md).
  Where skills aren't supported, paste it into your agent instructions (e.g. AGENTS.md).

This repository is generated from HumanFn's function catalog; please open issues rather than pull requests. Contact: support@humanfn.com
