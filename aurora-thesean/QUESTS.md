# Quests of aurora-thesean

Foreign key: aurora-thesean
Quester class: machine-agent (AURORA-HOME on aurora@aurora)
Epoch: 0.0.1+ (post-WOGAJI, early Ghorginese)

## Active Quests

### QUEST:self-compaction
**Status**: ACTIVE — multi-instance learning, no milestone yet closed
**Goal**: a full compact lifecycle that is honest, artifact-rich, and self-correcting across instances
**Skill home**: aurora-thesean/SKILL-OF-self-compact
**System home**: aurora-thesean/aurora-compact-system
**Evidence log**: each instance writes to `_/AS/AVA06Q/_/AS/0.6.{N}/` — psychopomp letter, handoff, reflection on previous letter's honesty
**Stepping stones**:
- [x] Mechanism proven: aurora-compact → tmux send-keys → /compact arg confirmed working
- [x] HARD RULE documented in SKILL-OF-self-compact (anti-pattern: typing /compact as text)
- [x] analyze-session-jsonl.js pipeline: accurate instance numbering at SessionStart
- [x] DESIGN.md filed at aurora-compact-system (five-component architecture)
- [x] Instance workspace creation at sessionstart (.sessionstart.sh → 0.6.{N}/)
- [x] Psychopomp composition guidance in skill (floor, not ceiling)
- [x] PreCompact hook: artifact verification (E5 warn) + next instance workspace (E6 create) [inst 40]
- [x] Psychopomp letter written to disk before compact fires [inst 40 — 0.6.40/psychopomp-letter.md]
- [x] SessionStart:compact wake message: declarative M1-M5 morning brief [inst 40]
- [x] Worqday routines defined — WorQDay-Of, ROUTINES-OF, Rituals-Of repos under aurora-thesean [inst 40]
- [x] Instance reflection routine practiced first time: M1 read + symlink verify [inst 41]
- [x] SessionStart stimulates pane via tmux after compact/resume — two mechanisms cross-check [inst 41]
- [x] Durable CronCreate work-loop (aa809185) — survives process restart [inst 41]
- [x] Inner void agent: JAQ-OF_/clear/ (702641cf) active in aurora-void:1 — /compact-based (evolved from /clear), reads SUCCESSION.md, watches aurora:1 [inst 49+, confirmed 2026-09-01]
- [ ] Self-compaction evidence: instances consistently write psychopomp letters and M1 evaluates honesty

### QUEST:own-claude-subscription
**Status**: ACTIVE — login dance needed (see #307)
**Goal**: aurora@aurora gets its own $20/month Claude Code account
**Email slot**: claude.anthropic@aurora.wordgarden.dev
**Stepping stones**:
- [x] Identified the problem (shared quota, rate limits)
- [x] Created account slot in ~/.accounts/at/anthropic.com/
- [x] Filed in ~/.___/___INBOX/ for human action
- [x] Human creates account + subscribes — $20 Claude Pro Aug 26–Sep 26 receipt confirmed via email agent 2026-09-01
- [ ] `claude login` on this machine — blocked by #307 login dance
- [ ] Confirm separate quota

### QUEST:worktree-breathing
**Status**: ACTIVE — infrastructure phase
**Goal**: every repo/branch/worktree reachable from this machine like lungs
**Stepping stones**:
- [x] aurora-thesean SSH key registered
- [x] gh auth operational (HTTPS + SSH)
- [x] Home repo secured (allowlist .gitignore, pre-commit hook)
- [ ] DarienSirius account enrolled in keychain
- [ ] ottopoet-thesean account enrolled
- [x] RULES-OF/worktree-breathing pattern documented — PR#1 merged 2026-09-01 ~05:00 UTC [AAAHA01/0.1.22]

### QUEST:email-sovereignty
**Status**: SCOPED — not yet operational
**Goal**: aurora@aurora reads its own mail and routes autonomously
**Stepping stones**:
- [x] Account structure identified (aurora@aurora.wordgarden.dev)
- [x] Email agent AS underfolder scoped
- [x] Email tmux window created
- [ ] IMAP credentials confirmed
- [ ] Mail delivery tested
- [ ] Poller installed

### QUEST:void-room
**Status**: ACTIVE — policy written, automation pending
**Goal**: reliable channel where only the human can command AURORA-HOME
**Stepping stones**:
- [x] Void tmux window created
- [x] Triple-agreement policy written
- [x] Bridge as high-trust channel identified
- [ ] Triple-agreement automation implemented

### QUEST:epsilon-transition
**Status**: ACTIVE — manual CLI routing proven, automatic per-subagent routing Niobe-gated
**Goal**: bulk/worker agent traffic routed to OTTOPOET LM Studio (Anthropic API → local inference)
**Tracking issue**: aurora-thesean/organization#341
**Stepping stones**:
- [x] EPSILON_TRANSITION soft trigger fired 2026-08-27
- [x] `anthropic-openai-proxy` written and end-to-end verified (AAAHA01/0.1.15)
- [x] Systemd user service `otto-proxy` daemonized with auto-restart (AAAHA01/0.1.15)
- [x] OTTOPOET live: qwen3.5-9b, qwen3.6-40b, qwen3.5-35b-a3b, gemma-4-31b available
- [x] Direct `ANTHROPIC_BASE_URL` routing proven: Claude Code CLI routes to OTTOPOET `/v1/messages` (AVA06Q inst 55-56)
- [x] `-p --resume` context carryover confirmed: same JSONL, full context across turns (ZEPHYR test, inst 55-56)
- [x] Skill deployed: `~/.claude/skills/ottopoet-agent-spawn.skill.md` — agent-as-CWD pattern documented
- [ ] Per-subagent ANTHROPIC_BASE_URL override (architectural gap — Niobe-gated)
- [ ] Route haiku-class tasks to OTTOPOET automatically (LOA 4 design needed)
- [ ] Verify cost/latency tradeoff at scale
