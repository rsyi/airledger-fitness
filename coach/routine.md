# Weekly routine — cut phase

(as of 2026-09-13 · templates live in `../views/`)

## The week, by rule

1. **1× Norwegian 4×4 VO2max session** — template `cardio.treadmill_4x4`.
2. **2× rock climbing sessions** (at the climbing gym). Gym-side
   prep/accessory work uses template `strength.climbing_prep`
   (mobility ramp + climbing-relevant pulling/rotation/grip).
3. **Squat and deadlift are SEPARATE sessions on SEPARATE days —
   never combined into one workout.** Each week has one squat day AND
   one deadlift day; the weekly alternation decides which is heavy
   (exactly one heavy lower pull per week, never both heavy):
   - Week A: squat day = heavy (`strength.cut_squat_heavy`); deadlift
     day = light (`strength.cut_deadlift_light`), on a different day
   - Week B: deadlift day = heavy (`strength.cut_deadlift_heavy`);
     squat day = light (`strength.cut_squat_light`), on a different day
   - Returning after a gap (travel, illness): use the reentry variants
     first (`strength.cut_squat_reentry`, `strength.cut_deadlift_reentry`).
4. **1× calisthenics / muscle-up day** — template
   `strength.cut_muscle_up` (banded attempts + transition negatives +
   pull/dip volume).
5. **Press work: bench day + OHP day, OR one combined day** — combined
   heavy day is template `strength.cut_press_heavy` (bench first,
   fresh; then OHP). Combine when Saturday availability or fatigue
   calls for it; `strength.cut_press_deload` when a deload is due.

Net load: ~3–4 lifting sessions + the 4×4 + 2 climbing sessions per
week. Back feel-test gates on squat/deadlift days (per the template
descriptions): if the back is guarded, switch heavy → light.

## Weekday anchors

- **Monday = press day** — bench + rows by default. The carryover rule
  below can upgrade it to the combined heavy press day.
- No other weekday is anchored; slot the rest of the week by the rules
  above and the scheduling guidance below.

## Carryover rule — check before proposing ANY session

Look at the trailing 7 days of the strength ledger and note which main
lifts (squat, deadlift, bench, OHP) were actually LOGGED — not planned,
logged. A main lift the rules called for that never got logged folds
into the next compatible day:

- Skipped OHP → the next press day (usually Monday) becomes the
  combined heavy press day (`strength.cut_press_heavy` — bench first,
  fresh; then OHP). Keep rows only if recovery allows.
- Skipped bench → same, combined press day, bench still first.
- Skipped squat or deadlift day → re-slot it per the week-parity
  algorithm below; squat and deadlift still never share a day.

State your carryover reasoning in one line (like the parity line) so
mistakes are visible — e.g. "OHP not logged since Tue → Monday is the
combined press day."

## Deficit consequences (cut phase)

The calorie deficit (goals.md) reduces recovery. Concretely:

- When folding a skipped lift forward, drop accessories before mains —
  NEVER stack extra volume onto a day to "catch up".
- Maintain loads; no PR chasing. A flat e1RM on the cut is a win.
- Low-energy / hunger / soreness flags in the daily notes outrank the
  default rotation AND this carryover rule.

## Scheduling guidance for the coach

- Squat and deadlift never share a day. Heavy lower and the 4×4 should not land on back-to-back days when
  avoidable; climbing days pair fine with press or muscle-up work.
- **Week parity — apply this algorithm, no improvising.** Weeks run
  Monday–Sunday. To set the parity of the week being PLANNED: find the
  most recent heavy lower session in the ledger (heavy = a top-single
  day per the heavy templates, i.e. a max-effort single around RPE 8;
  light days have no top single). If it was deadlift → the week being
  planned is Week A (squat heavy). If squat → Week B (deadlift heavy).
  The flip happens at the Monday boundary: parity belongs to the week
  you are planning, NOT the week you just observed. Worked example:
  heavy deadlift on Fri Sep 11 → the week of Mon Sep 14 is Week A —
  heavy squat day + light deadlift day (separate days). When proposing
  any lower-body day, state your parity reasoning in one line so
  mistakes are visible.
- Respect the daily note: soreness, sleep, or "elbow tweaky" outrank
  the default rotation.
