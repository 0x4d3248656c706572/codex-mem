# codex-mem

Norsk

Vedvarende minne for Codex.

## Overview

codex-mem captures Codex session history, registers MCP search tools, watches transcripts, and injects relevant context into future Codex turns.

## Install

    npx codex-mem install --ide codex-cli

## Start the worker

    npx codex-mem start

## Restart Codex

Restart Codex after install so it reloads hooks, MCP config, and AGENTS context.

## Verify

    npx codex-mem status

Open the viewer:

    http://127.0.0.1:37777

## Useful commands

    npx codex-mem install --ide codex-cli
    npx codex-mem start
    npx codex-mem stop
    npx codex-mem restart
    npx codex-mem status
    npx codex-mem search "your query"
    npx codex-mem uninstall

## What gets installed

    ~/.codex/hooks.json
    ~/.codex/config.toml
    ~/.codex/AGENTS.md
    ~/.codex-mem/app
    ~/.codex-mem/transcript-watch.json
    ~/.codex-mem/settings.json
    ~/.codex-mem/logs

## Privacy

Wrap sensitive content with <private> ... </private> if you do not want it stored.

## Need more detail?

Full dokumentasjon finnes i den engelske README-filen.

Read the main README and docs for the full English documentation set.