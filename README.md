# todomove (Claude Code plugin)

Reports session lifecycle to Todomove — `UserPromptSubmit` → `running`,
`PermissionRequest` → `requestPermission`, `Stop` → `needReview`, `StopFailure` →
`failure`, `SessionEnd` → `idle` — and bundles the Todomove MCP server, so there's no
separate `claude mcp add` step.

## Install

```
/plugin marketplace add Todomove/claude-code-plugin
/plugin install todomove@todomove-claude-code-plugin
```

Claude Code prompts for your Todomove connector token and API base URL once, at enable
time. Both then drive the bundled MCP server and the hooks — nothing else to configure.

## Commands

```
/todomove:todo
```

List/create/complete tasks or subtasks, or change a due date, in plain language.

## License

MIT — see `LICENSE`.
