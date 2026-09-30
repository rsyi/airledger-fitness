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
- **The program is the source of the week (templates retired
  2026-09-30).** `program.yaml`'s `routine:` (base week +
  `phase_overrides`) holds the authoritative day-by-day prescription;
  the app resolves it into a "program slice" (concrete exercises,
  sets/reps, loads) that the nightly coach and the in-app coach read.
  The old `views/*.template.yml` files are deleted — when the coach
  schedules "heavy squat day" it reads that day from the program, not a
  template file. `routine.md` is a deprecated readable fallback only.
- **Read as prompt context.** The nightly coach (and any ad-hoc "what
  should I do today?" session) reads these files verbatim alongside
  recent ledger data (workouts, weight, daily_notes). Write for that
  audience: unambiguous rules beat vibes.
