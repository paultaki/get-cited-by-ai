# Prediction Ledger

Register every prediction before the scoring data arrives (G1) — a prediction
written after you've seen the result is hindsight, not evidence. Score
against the registered band only; do not loosen it after seeing data.

| Date registered | Prediction (numeric band) | Refutation condition | Score-by date | Outcome | Notes |
|---|---|---|---|---|---|
| 2026-07-13 | Merit reaches ≥100 cited pages in a single day by the first August Bing Webmaster pull | Fails to reach ≥100 cited pages/day by the first August pull | ~2026-08-01 | HIT | 127 cited pages hit on 07/13 — three weeks early — plus a 669-citation day, both site records. Source: A4, G1; STUDY-2; UPDATES. |
| [YYYY-MM-DD] | [numeric band, not a vague direction — e.g. "X settles at N–M citations/day post-event"] | [what observed result falsifies this — state it now, not after scoring] | [YYYY-MM-DD] | UNSCORED | [rule ID(s) this prediction tests] |

## Outcome definitions

- **HIT** — result landed inside the band, or beat it in the predicted
  direction ahead of schedule (e.g. A4).
- **HOLDS** — result landed inside the band, in-window, no directional
  surprise (e.g. G1 ledger items 1, 3, 4).
- **REFUTED** — result fell outside the band or met the refutation
  condition.
- **UNSCORED** — score-by date hasn't arrived yet (e.g. the F2 Bing-inverse
  re-probe, per G1).

## Rules

1. Every prediction needs a numeric band and an explicit refutation
   condition — "citations should improve" is not scoreable.
2. Score at or after the score-by date, against the band as registered.
3. Cross-validate the scoring call against a second read of the raw data
   before finalizing HIT/REFUTED on your own prediction (G9).
4. A rising "share of citations since X shipped" is not itself a scored
   prediction and never substitutes for one — flat rates accumulate
   mechanically (G8).
