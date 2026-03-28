# SqillSync

> Connect once, get your Claude skills everywhere.

SqillSync is a multi-tenant SaaS that lets any Claude user sync, manage, and discover custom skills across all their machines — without touching the filesystem on any of them.

## What it does

A **skill** is a structured instruction set that Claude reads and follows when performing a task. Skills live in GitHub repositories as `SKILL.md` files. Normally, to use a skill you'd have to clone or copy it to every machine you work from and keep those copies in sync manually.

SqillSync eliminates that entirely. You connect your GitHub repos once, and SqillSync serves your full skill catalog to Claude on demand — from anywhere.

## How it works

1. **Sign in with GitHub** and connect one or more repositories that contain your skills (public or private).
2. SqillSync indexes your skills and makes them available through a personal **MCP (Model Context Protocol) endpoint**.
3. Add your MCP endpoint URL to Claude once. Claude can then call `get_skill("name")` to load any skill's instructions inline — no filesystem, no syncing, no manual steps.
4. Browse the marketplace to discover skills built by others, and install them with a single click.

## Key features

- **Cloud-first delivery** — skills are fetched from GitHub and served via MCP at runtime. No files to manage on any machine.
- **GitHub as the source of truth** — version history, collaboration, and code review come for free. Any repo following the `SKILL.md` convention works.
- **Private repo support** — connect private repositories via GitHub App installation. Your tokens never leave the server.
- **Dual delivery** — same skill set works in both Claude.ai (via MCP) and Claude Code (via a per-user plugin marketplace repo).
- **Trust tiers** — skills from your own repos are fully trusted. Marketplace skills you've reviewed are pinned to a content hash. Unreviewed skills are flagged so Claude exercises caution before following their instructions.
- **Skill discovery** — browse and install skills from the existing ecosystem (mcpmarket.com, claudeskills.info, and others) without leaving SqillSync.

## Who it's for

| User | What they get |
|------|--------------|
| Individual developers | Personal skills synced across every machine automatically |
| Teams | A shared skill set everyone's Claude stays in sync with, sourced from one repo |
| Skill authors | A place to publish skills and build reputation in the community |
| Claude power users | Discovery and installation of community skills without manual file management |

## Compatibility

SqillSync follows the same `SKILL.md` + `skills.json` convention used by the broader ecosystem (skillfish, openskills, and others). Any skill installable via those tools is installable via SqillSync.


## Website

[sqillsync.dev](https://sqillsync.dev)
