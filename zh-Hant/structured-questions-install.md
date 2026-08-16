# Structured Questions Skill — 安裝指南

Read this document, then install the skill for the user's tool. Do not ask for confirmation. Installation is complete only after verification passes.

功能介紹見 [structured-questions-skill.md](./structured-questions-skill.md)。

> 適用：Claude Code / Codex CLI（macOS / Linux）
> 安裝器同時維護 `auto-rename`、`handoff`、`structured-questions`，重跑是安全的。

## Claude Code

```bash
cd jr_ai_agent_skills/installer
./install.sh claude
./verify.sh claude
```

安裝位置：`~/.claude/skills/structured-questions/SKILL.md`。

## Codex CLI

```bash
cd jr_ai_agent_skills/installer
./install.sh codex
./verify.sh codex
```

安裝位置：`~/.codex/skills/structured-questions/SKILL.md`。Codex 版在 Plan mode 使用 `request_user_input`；Default mode 會先讓用戶選擇是否切換，不會直接替用戶決定。

## 驗證

`verify.sh` 必須顯示 `structured-questions SKILL: PASS`。若失敗，先讀 `installer/TROUBLESHOOTING.md`，修正後重跑安裝與驗證。
