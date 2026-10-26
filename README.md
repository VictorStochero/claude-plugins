# Stochero — Claude Code plugins

A [Claude Code](https://claude.com/claude-code) **plugin marketplace**. Add it once and install any plugin below — new plugins show up here automatically.

## Add the marketplace

```
/plugin marketplace add VictorStochero/claude-plugins
```

Then install a plugin:

```
/plugin install <plugin>@stochero
```

## Plugins

| Plugin | Description | Repo |
|---|---|---|
| **laravel-worktree** | Create, inspect, and clean up isolated git worktrees for Laravel projects across Herd, DDEV, and Sail — full parallel environments (DB, `.env`, domain) in one command. | [VictorStochero/laravel-worktree](https://github.com/VictorStochero/laravel-worktree) |
| **fluxo-orca** | (pt-BR) Orca workflow for Laravel, Python and JS/TS on Windows, Linux or macOS: Orca worker delegation, per-task worktrees with their own database, writer/reviewer/verifier agents, machine-wide test queue, quota check, GitHub board rules, local environment profile, methodology skills, and hooks that enforce them. AI-driven installer in `GUIA.md`. | [VictorStochero/fluxo-orca](https://github.com/VictorStochero/fluxo-orca) |
| **auditoria-pre-subida** | (pt-BR) Mandatory pre-push audit: the branch diff is checked against the project's architecture guide, security and stack best practices, with an adversarial second pass; a hook blocks PR creation, merge and pushes to base branches until the commit has an approved verdict. Any project, Claude Code only. | [VictorStochero/auditoria-pre-subida](https://github.com/VictorStochero/auditoria-pre-subida) |

### Example

```
/plugin marketplace add VictorStochero/claude-plugins
/plugin install laravel-worktree@stochero
```

## How it works

Each plugin lives in its own repository (independent issues, versioning, and releases). This repo only holds the marketplace manifest (`.claude-plugin/marketplace.json`) that references them, so adding a future plugin is a one-line change here.

## License

MIT © Victor Stochero. Each referenced plugin carries its own license.
