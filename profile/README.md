<p align="center">
  <img src="assets/escoffier-labs-banner.jpg" alt="Escoffier Labs banner: a chef at the pass ringing the service bell" width="900">
</p>

# Escoffier Labs

Home of [Brigade](https://brigade.tools), the local operator layer for AI agents.

Brigade keeps agent loops receipted, reviewed, and portable. The supporting Escoffier Labs tools provide the stations around it: agent skills, code search, sealed secrets, notifications, screenshots, and durable workflow records. MiseLedger, GraphTrail, and agent-notify ship inside the [Brigade monorepo](https://github.com/escoffier-labs/brigade) and install via `brigade setup`. Publish-safety scanning ships inside Brigade itself (`brigade scrub` / `brigade guard`).

## Flagship

- [Brigade](https://github.com/escoffier-labs/brigade) - local operator layer for AI agent memory, handoffs, and guardrails across every harness.

## Skills & guides

- [Skillet](https://github.com/escoffier-labs/skillet) - agent skills suite: repo audits, bug hunting, security sweeps, publish gates, releases, and memory handoffs.
- [Solos Cookbook](https://github.com/escoffier-labs/solos-cookbook) - how one engineer runs a 24/7 multi-agent AI stack on bare metal.

## Agent ops

- [Agent Pantry](https://github.com/escoffier-labs/agentpantry) - secure browser session and secret sync for agent machines.
- [Memory Doctor](https://github.com/escoffier-labs/memory-doctor) - maintenance CLI for the Claude Code and OpenClaw memory systems.
- [Bootstrap Doctor](https://github.com/escoffier-labs/bootstrap-doctor) - audits and trims oversize OpenClaw prefix files into reference cards.
- [Agent Notify](https://github.com/escoffier-labs/brigade/tree/main/stations/notify) - privacy-first push notifications for AI coding agents (`stations/notify/` in Brigade; install via `brigade setup`).
- [Cloche](https://github.com/escoffier-labs/cloche) - agent-neutral app screenshot capture.

## Dev tools

- [GraphTrail](https://github.com/escoffier-labs/brigade/tree/main/engines/code-graph) - local code-graph CLI and read-only MCP server: callers, callees, impact, and context (`engines/code-graph/` in Brigade; install via `brigade setup`). The archived [graphtrail](https://github.com/escoffier-labs/graphtrail) repo is a frozen mirror.
- [Code Search API](https://github.com/escoffier-labs/code-search-api) - local semantic code search with Ollama embeddings, SQLite, and hybrid search.
- [Usage Tracker](https://github.com/escoffier-labs/usage-tracker) - token usage and cost analytics for OpenClaw sessions across models.
- [Mise en Scene](https://github.com/escoffier-labs/mise-en-scene) - turns source material into self-contained interactive HTML/SVG technical explainers.
- [Plating](https://github.com/escoffier-labs/plating) - reproducible, sanitized terminal-demo SVGs for READMEs and websites.
- [Escoffier Fleet Kit](https://github.com/escoffier-labs/escoffier-fleet-kit) - shared theme, OG cards, and hands-off publishing for the Escoffier Labs website fleet.
- [Token Glace](https://github.com/escoffier-labs/token-glace) - deterministic output compaction that trims terminal noise before it hits agent context. The Token Glace fork of vincentkoc/tokenjuice.

## Evidence stack

- [MiseLedger](https://github.com/escoffier-labs/brigade/tree/main/engines/evidence-ledger) - local-first evidence ledger for AI work history (`engines/evidence-ledger/` in Brigade; install via `brigade setup`). Built-in crawlers: `miseledger crawl sessions|files|gitlog|...`. The archived [miseledger](https://github.com/escoffier-labs/miseledger) repo is a frozen mirror. StationTrail and SourceHarvest were absorbed in v0.3.0.

## Start here

```sh
pipx install brigade-cli
brigade setup
```

Read the [Brigade docs](https://brigade.tools/docs), then use the supporting stations as your workflow needs them.
