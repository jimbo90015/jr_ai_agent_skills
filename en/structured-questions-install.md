# Structured Questions Skill — Installation Guide

Read this document, then install the skill for the user's tool. Do not ask for confirmation. Installation is complete only after verification passes.

See [structured-questions-skill.md](./structured-questions-skill.md) for the feature overview.

> Supports Claude Code and Codex CLI on macOS and Linux.
> The installer manages `auto-rename`, `handoff`, and `structured-questions`; rerunning it is safe.

## Claude Code

```bash
cd jr_ai_agent_skills/installer
./install.sh claude
./verify.sh claude
```

Installs to `~/.claude/skills/structured-questions/SKILL.md`.

## Codex CLI

```bash
cd jr_ai_agent_skills/installer
./install.sh codex
./verify.sh codex
```

Installs to `~/.codex/skills/structured-questions/SKILL.md`. In Plan mode, the Codex version uses `request_user_input`. In Default mode, it first asks whether the user wants to switch modes instead of silently choosing for them.

## Verification

`verify.sh` must report `structured-questions SKILL: PASS`. If it fails, read `installer/TROUBLESHOOTING.md`, fix the issue, and rerun installation and verification.
