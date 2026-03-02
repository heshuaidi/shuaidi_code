# AGENTS.md

## Build rules
- Must follow docs/codex-spec.txt exactly.
- Every PR must pass GitHub Actions CI (mvn test).
- Never delete meta/lock (zombie lock strategy).
- All file writes must be tmp -> atomic rename.
- Do NOT scan/list directories under NAS_ROOT; only operate on provided reportDir.

## Output rules
- Prefer CSV outputs as spec.
- Keep changes small and testable; add/adjust tests for new behavior.