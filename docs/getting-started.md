# Getting Started

## 1. Install

```bash
npx codex-mem install --ide codex-cli
```

## 2. Start the worker

```bash
npx codex-mem start
```

## 3. Restart Codex

Codex needs to reload:

- `~/.codex/hooks.json`
- `~/.codex/config.toml`
- `~/.codex/AGENTS.md`

## 4. Verify

Check worker status:

```bash
npx codex-mem status
```

Open the viewer:

```text
http://127.0.0.1:37777
```

## 5. Use it

Run Codex normally. Memory capture is automatic.

Useful manual recall:

```bash
npx codex-mem search "project auth flow"
```
