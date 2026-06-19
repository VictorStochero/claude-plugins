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

### Example

```
/plugin marketplace add VictorStochero/claude-plugins
/plugin install laravel-worktree@stochero
```

## How it works

Each plugin lives in its own repository (independent issues, versioning, and releases). This repo only holds the marketplace manifest (`.claude-plugin/marketplace.json`) that references them, so adding a future plugin is a one-line change here.

## License

MIT © Victor Stochero. Each referenced plugin carries its own license.
