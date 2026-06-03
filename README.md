# Amply — Claude Code plugin catalog

This repository is the **Claude Code plugin marketplace** for [Amply](https://amply.tools).
It is a catalog only — the plugins themselves live in their own repositories.

## Install

Inside Claude Code, run two commands:

```text
/plugin marketplace add amply-tools/claude-plugins
/plugin install amply-integration@amply
```

- The first command **registers Amply's plugin catalog** — it installs nothing on its own.
- The second command **installs the skill** from that catalog.

(`amply` is the marketplace name; `amply-integration` is the plugin.)

## Plugins

| Plugin | What it does | Source |
|---|---|---|
| `amply-integration` | Walks an AI agent through integrating the Amply SDK into a mobile app (React Native, Expo, iOS, Android, Kotlin Multiplatform) — analytics audit, event mapping, a single thin wrapper, deeplink wiring, and a Who/When/What campaign-readiness audit. | [amply-tools/sdk-skill](https://github.com/amply-tools/sdk-skill) |

## Other ways to install

The `amply-integration` skill is also installable without Claude Code's plugin system,
via the cross-agent [`skills` CLI](https://skills.sh) (Claude Code, Codex CLI, and more):

```bash
npx skills add amply-tools/sdk-skill
```

## License

Apache License 2.0.
