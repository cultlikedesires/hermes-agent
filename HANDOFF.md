# Session Handoff → Codex

Context summary so work can continue in Codex (or any tool) without re-explaining.

## What was done this session

Installed the **Karpathy coding principles** as behavioral guardrails for AI tools in this repo, then shipped them through the full GitHub workflow (branch → commit → push → PR → merge).

- **`CLAUDE.md`** (new file, repo root) — full Karpathy guidelines. Read automatically by Claude Code.
- **`AGENTS.md`** (updated) — compact 4-principle section added near the top, pointing to `CLAUDE.md` for full text. **Read automatically by Codex.**
- **PR #1** — merged into `main` via squash merge. Changes are now permanent on `main`.

## Current repo state

- **Default branch `main`**: contains both files. Latest commit:
  `Add Karpathy coding principles to CLAUDE.md and AGENTS.md (#1)`
- **Working branch**: `claude/trusting-davinci-M0gol` (work merged; branch still exists, harmless)
- This repo is a **fork** of `NousResearch/hermes-agent` — changes only affect this fork.

## The four principles (now active in both tools)

1. **Think before coding** — state assumptions, surface tradeoffs, ask when unclear.
2. **Simplicity first** — minimum code, no speculative abstractions.
3. **Surgical changes** — touch only what the task requires, match existing style.
4. **Goal-driven execution** — define verifiable success criteria, loop until verified.

## How the mirroring works (important)

| File | Tool that auto-reads it | Equivalent to |
|------|------------------------|---------------|
| `CLAUDE.md` | Claude Code | — |
| `AGENTS.md` | Codex | Codex's version of `CLAUDE.md` |

**You don't need to copy anything manually.** Both files are committed to `main`, so each tool loads its own file at session start. To change the principles later: edit `CLAUDE.md` (the source of truth), and only touch the `AGENTS.md` headlines if a principle's name changes.

## Picking up in Codex

Nothing to configure — open this repo in Codex and it reads `AGENTS.md` automatically. The principles are live.
