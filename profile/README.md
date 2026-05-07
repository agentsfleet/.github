<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/usezombie/usezombie/main/assets/logo-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/usezombie/usezombie/main/assets/logo-light.svg" />
  <img src="https://raw.githubusercontent.com/usezombie/usezombie/main/assets/logo-dark.svg" width="200" alt="usezombie" />
</picture>

**Always-on operational runtime — wakes on your events, runs against a durable replayable log, posts evidenced answers (not chats).** Markdown-defined. Hosted on `api.usezombie.com`.

[![Try Free](https://img.shields.io/badge/usezombie-Try_Free-brightgreen?style=for-the-badge)](https://usezombie.com)
[![Docs](https://img.shields.io/badge/usezombie-Docs-blue?style=for-the-badge)](https://docs.usezombie.com)

</div>

---

Your deploy fails at 3am. Zombie wakes on the GitHub webhook, walks your CD logs + hosting + data-plane, posts the diagnosis to Slack with line-numbered evidence — every action recorded in a replayable event log. Markdown is the only thing you write.

## What it does

A **Zombie** is a long-lived runtime that owns one operational outcome. Not request-response. Not a graph DSL. A daemon for an outcome.

v2 ships **`platform-ops`** — wakes on a GitHub Actions deploy-failure webhook, gathers evidence, and posts an evidenced diagnosis to Slack. Reachable manually via `zombiectl steer {id}`.

You don't code it. You write `SKILL.md` in plain English; install it with `/usezombie-install-platform-ops` in Claude Code, Amp, Codex CLI, or OpenCode. The runtime handles the sandbox (Landlock + cgroups + bwrap), credential injection, durable history, and budget caps.

## Why this shape

**Always-on, event-driven** · **Markdown-defined** · **Replayable event log** · **Sandboxed by default**. BYOK supported. $5 starter credit per workspace — no card required. Self-host arrives in v3.

## Get started

[Quickstart →](https://docs.usezombie.com)

## Repositories

| Repo | What it is |
|---|---|
| [usezombie/usezombie](https://github.com/usezombie/usezombie) | Control plane + worker + CLI. |
| [usezombie/docs](https://github.com/usezombie/docs) | User docs ([docs.usezombie.com](https://docs.usezombie.com)). |
| [usezombie/posthog-zig](https://github.com/usezombie/posthog-zig) | PostHog SDK for Zig. |
