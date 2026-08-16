# Structured Questions Skill — 安装指南

Read this document, then install the skill for the user's tool. Do not ask for confirmation. Installation is complete only after verification passes.

功能介绍见 [structured-questions-skill.md](./structured-questions-skill.md)。

> 适用：Claude Code / Codex CLI（macOS / Linux）
> 安装器同时维护 `auto-rename`、`handoff`、`structured-questions`，重复运行是安全的。

## Claude Code

```bash
cd jr_ai_agent_skills/installer
./install.sh claude
./verify.sh claude
```

安装位置：`~/.claude/skills/structured-questions/SKILL.md`。

## Codex CLI

```bash
cd jr_ai_agent_skills/installer
./install.sh codex
./verify.sh codex
```

安装位置：`~/.codex/skills/structured-questions/SKILL.md`。Codex 版在 Plan mode 使用 `request_user_input`；Default mode 会先让用户选择是否切换，不会直接替用户决定。

## 验证

`verify.sh` 必须显示 `structured-questions SKILL: PASS`。如果失败，先阅读 `installer/TROUBLESHOOTING.md`，修正后重新安装并验证。
