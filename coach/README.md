# coach/ — standing context for the AI coach

These files are the durable coaching context for Claude: what the goals
are (`goals.md`) and what a training week is supposed to look like
(`routine.md`). They are the source of truth the nightly coach reads
when drafting the next day's plan, and the thing to edit when the
answer to "what should I be doing?" changes.

## Contract

- **Edited by Claude, versioned by git.** Changes happen in
  conversation ("switch me to a bulk", "drop climbing to 1x/week") —
  Claude edits the file, commits, and pushes. Date-stamp material
  changes in the file header.
- **Template links are load-bearing.** Routine rules reference template
  names from `../views/*.template.yml` (e.g. `strength.cut_squat_heavy`).
  Those templates ARE the structured plans in Air Ledger — when the
  coach schedules "heavy squat day", it means "apply that template".
  If a template is renamed or added, update `routine.md` to match.
- **Read as prompt context.** The nightly coach (and any ad-hoc "what
  should I do today?" session) reads these files verbatim alongside
  recent ledger data (workouts, weight, daily_notes). Write for that
  audience: unambiguous rules beat vibes.
