# Troubleshooting

## Worker not responding

Check status:

```bash
npx codex-mem status
```

Restart it:

```bash
npx codex-mem restart
```

## Codex does not pick up memory

Restart Codex after install so it reloads:

- `~/.codex/hooks.json`
- `~/.codex/config.toml`
- `~/.codex/AGENTS.md`

## Port conflict

If `37777` is already taken, update the worker port in settings and restart.

## No memories yet

That is normal on a fresh install. Finish a Codex session first, then check:

```bash
npx codex-mem search "your project"
```

## Remove codex-mem completely

```bash
npx codex-mem uninstall
```
