# Derived metrics — definitions the coach applies

(as of 2026-09-11 · applied to the nightly ledger dump; the coach
computes these from raw rows, they are not stored anywhere)

## Strength

- **e1RM (per lift, per session):** Epley — `weight × (1 + reps/30)`;
  a top single is its own e1RM. Compute per set, take the session max.
  Track for: Barbell Squat, Deadlift, Bench Press, Overhead Press.
- **Maintenance check (cut objective):** 4-week slope of session-max
  e1RM per lift. Flat or slightly positive = objective met; a drop
  > ~5% is a red flag worth calling out in the summary.
- **Weekly tonnage:** `Σ (weight × reps)` per week, split main lifts
  vs accessories.

## Fatigue

- **ACWR (acute:chronic workload ratio):** 7-day tonnage ÷ 28-day
  average weekly tonnage. Sweet spot ≈ 0.8–1.3; > 1.5 = elevated
  strain → bias the next day easier; < 0.8 during a cut is expected,
  don't chase it up.
- **Subjective override:** anything in `daily_notes` (soreness, bad
  sleep, tweaks) outranks the numbers. Say so explicitly when it
  changes the recommendation.

## Conditioning (4×4)

- **Session quality:** minutes in Z4+ (from zone4_reached → total_time),
  max HR vs `user_max_hr`, and the speed/incline actually held.
- **Progress:** week-over-week trend in speed × incline at equal or
  better Z4+ time. Faster Z4 arrival at the same settings = improving
  warm-up economy, not necessarily fitness — judge on work completed.

## Body composition

- **Trend weight:** 7-day rolling average of weight_lbs; cut adherence
  = slope ≈ −0.5 to −1.0 lb/week. Flat 2+ weeks during the cut is
  worth a nutrition callout.

## Adherence

- **Weekly structure vs `routine.md`:** count sessions by type in the
  trailing 7 days (4×4, climbing, heavy lower, muscle-up, press) and
  name what's missing when drafting the next day.
