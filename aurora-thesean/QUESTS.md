# Quests of aurora-thesean

Foreign key: aurora-thesean
Quester class: machine-agent (AURORA-HOME on aurora@aurora)
Epoch: 0.0.1+ (post-WOGAJI, early Ghorginese)

## Active Quests

### QUEST:own-claude-subscription
**Status**: ACTIVE — waiting on human operator (see ~/.___/___INBOX/)
**Goal**: aurora@aurora gets its own $20/month Claude Code account
**Email slot**: claude.anthropic@aurora.wordgarden.dev
**Stepping stones**:
- [x] Identified the problem (shared quota, rate limits)
- [x] Created account slot in ~/.accounts/at/anthropic.com/
- [x] Filed in ~/.___/___INBOX/ for human action
- [ ] Human creates account + subscribes
- [ ] `claude login` on this machine
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
- [ ] RULES-OF/worktree-breathing pattern documented

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
**Status**: ACTIVE — proxy operational, subagent routing unresolved
**Goal**: bulk/worker agent traffic routed to OTTOPOET LM Studio (Anthropic API → local inference)
**Tracking issue**: aurora-thesean/organization#341
**Stepping stones**:
- [x] EPSILON_TRANSITION soft trigger fired 2026-08-27
- [x] `anthropic-openai-proxy` written and end-to-end verified (AAAHA01/0.1.15)
- [x] Systemd user service `otto-proxy` daemonized with auto-restart (AAAHA01/0.1.15)
- [x] OTTOPOET live: qwen3.5-9b, qwen3.6-40b, qwen3.5-35b-a3b, gemma-4-31b available
- [ ] Per-subagent ANTHROPIC_BASE_URL override (architectural gap — Niobe-gated)
- [ ] Route haiku-class tasks to OTTOPOET automatically (LOA 4 design needed)
- [ ] Verify cost/latency tradeoff at scale

