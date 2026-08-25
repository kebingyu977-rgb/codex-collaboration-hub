# Codex Collaboration Hub

This folder is the shared handoff point for Codex sessions running on different computers or accounts. It is synchronized through the private GitHub repository `https://github.com/kebingyu977-rgb/codex-collaboration-hub`.

## Start Here

1. On a new computer, clone the private repository and open the cloned folder as the Codex workspace.
2. Read `CURRENT_CONTEXT.md` before starting work.
3. Claim or create a task in `TASK_BOARD.md`.
4. Before stopping or handing work over, add a record in `HANDOFF_LOG.md` and update `CURRENT_CONTEXT.md`.

## macOS Setup

1. Install Git if it is not already installed: open Terminal and run `xcode-select --install`.
2. Sign in to GitHub in a browser with an account that has access to this private repository.
3. In Terminal, clone the hub:

```bash
git clone https://github.com/kebingyu977-rgb/codex-collaboration-hub.git
cd codex-collaboration-hub
```

4. Open the `codex-collaboration-hub` folder in Codex on the Mac.
5. If Git asks for authentication, use GitHub login or a personal access token; never place the token in these shared files.

## Sync Routine

Before starting work on either computer:

```bash
git pull --rebase origin main
```

After a completed handoff:

```bash
git add CURRENT_CONTEXT.md TASK_BOARD.md HANDOFF_LOG.md
git commit -m "Handoff: short description"
git push origin main
```

If Git reports a conflict, do not force-push. Preserve both handoff entries, merge the shared facts manually, then commit the resolved files.

## Working Rules

- Use one task ID everywhere, for example `TASK-20260825-01`.
- Write facts, file paths, decisions, and blockers. Do not write passwords, verification codes, access tokens, or private credentials.
- Do not overwrite another Codex's active task. Add a new log entry instead.
- Mark a task `done` only after its output path and verification are recorded.
- If OneDrive shows a sync conflict, keep both copies, compare the newest entries, then manually merge the information.

## File Roles

| File | Purpose |
| --- | --- |
| `CURRENT_CONTEXT.md` | The latest shared priorities, decisions, and known blockers. |
| `TASK_BOARD.md` | One-line task status board. |
| `HANDOFF_LOG.md` | Append-only record of completed or paused work. |
| `templates/HANDOFF_TEMPLATE.md` | Copy for a complete task handoff. |

## What This Enables

Both Codex sessions can work from the same current context and leave structured handoffs for the other session. It does not create direct real-time chat or share either account's private memory; the shared files are the source of truth.
