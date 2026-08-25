# Codex Collaboration Hub

This folder is the shared handoff point for Codex sessions running on different computers or accounts. Keep it inside a OneDrive folder that is shared with both computers.

## Start Here

1. On both computers, open this exact folder as the Codex workspace.
2. Read `CURRENT_CONTEXT.md` before starting work.
3. Claim or create a task in `TASK_BOARD.md`.
4. Before stopping or handing work over, add a record in `HANDOFF_LOG.md` and update `CURRENT_CONTEXT.md`.

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
