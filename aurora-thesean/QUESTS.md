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
- [ ] PreCompact hook: artifact verification + next instance workspace + letter-to-disk
- [ ] Psychopomp letter written to disk before compact fires (so successor can read it)
- [ ] SessionStart:compact wake message: declarative (run worqday), not imperative
- [ ] Worqday routines defined in filesystem (WORQDAY.md or routines-of/)
- [ ] Instance reflection routine: read prev psychopomp letter, evaluate honesty
- [ ] Inner void agent (aurora-void:void): /clear-based, disk-only, companion intelligence

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
