# How It Works

codex-mem combines three paths:

## 1. Native Codex hooks

Codex hooks run at session start and prompt submit. They ask the worker for context and initialize the current session.

## 2. Transcript watching

The transcript watcher reads `~/.codex/sessions/**/*.jsonl` and turns Codex events into durable memory records.

## 3. MCP tools

The worker exposes a local MCP server so Codex can search past work on demand.

## Storage layout

- `~/.codex-mem/settings.json`
- `~/.codex-mem/logs`
- `~/.codex-mem/transcript-watch.json`
- `~/.codex-mem/app`

## Session flow

1. user starts Codex
2. Codex hooks request context
3. worker responds with recent and relevant memory
4. Codex session proceeds
5. transcript watcher records new events
6. future sessions reuse that context
