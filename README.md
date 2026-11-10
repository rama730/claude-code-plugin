# NetworkBase plugin for Claude Code

Adds the NetworkBase MCP server and a skill that teaches Claude Code the common requests: "how many tasks do I have", "create a task", "change the README".

```
/plugin marketplace add rama730/claude-code-plugin
/plugin install networkbase@networkbase
```

Then in a project folder: `npx @networkbase/cli login` and `npx @networkbase/cli init <workspace>`.

More: https://networkbase.in/docs/agents

## Updating (owner)

The source lives in the NetworkBase repository under `integrations/claude-code-plugin/`; this repository is a copy of that folder. Change it there, then copy the folder's contents here and push. The check workflow starts the MCP server and fails if a tool the skill names is missing.

The server is pinned to `@networkbase/cli@2`.
