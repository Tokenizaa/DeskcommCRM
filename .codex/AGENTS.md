# ECC for Codex CLI

This supplements the root `AGENTS.md` with a repo-local ECC baseline.

## Repo Skill

- Source of truth for conventions: root `AGENTS.md` + `CLAUDE.md` (doutrina/DoD). No repo-local skill files.
- The auto-generated ECC skills (`.agents/skills/DeskcommCRM/SKILL.md`, `.claude/skills/DeskcommCRM/SKILL.md`) were **removed**: they encoded the wrong conventions (e.g. blanket `snake_case`) that conflicted with the real patterns. Do not regenerate them.
- Keep user-specific credentials and private MCPs in `~/.codex/config.toml`, not in this repo.

## MCP Baseline

Treat `.codex/config.toml` as the default ECC-safe baseline for work in this repository.
The generated baseline enables GitHub, Context7, Exa, Memory, Playwright, and Sequential Thinking.

## Multi-Agent Support

- Explorer: read-only evidence gathering
- Reviewer: correctness, security, and regression review
- Docs researcher: API and release-note verification

## Workflow Files

- No dedicated workflow command files were generated for this repo.

Use these workflow files as reusable task scaffolds when the detected repository workflows recur.