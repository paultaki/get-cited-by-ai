# Agent Notes

## 2026-07-15 · claude-code (v1.0.1, later the same day)

- **Did:** Precision release after two decorrelated post-release reviews (external
  model review of the repo + fresh-context adversarial pass over the first two
  production audits). Fixed 6 wording/citation overstatements (G2→G3 miscite,
  "controlled experiment"→"same-template controlled regression", E1 "cost"→"sat
  miscounted", D4 INFERENTIAL qualifier restored, README module-count line,
  "independent studies"→"independently-run analyses"); added prediction-ledger
  rule 5 (band/refutation must partition outcomes — failing test: both production
  audits registered unscoreable predictions independently); added `predictions/`
  (public git-timestamped preregistration, 3 files: credibilityos baseline, TFL
  4-prediction set, F2 re-probe transcription); added
  `examples/credibilityos-audit.md` (worked example incl. adversarial-pass log);
  added `tests/EDITS-2026-07-15-v1.0.1.md` (every edit → its failing check);
  RULEBOOK gained a v1.0.1 errata block. No rule, receipt, or number changed.
- **Why:** The credible red-team attack was "preregistrations can't be independently
  timestamped" — `predictions/` makes git the receipt. The wording fixes close the
  gap between the evidence tags and the framing language.
- **Next:** Score predictions at their score-by dates (08-01, 08-15, 08-21, 09-01);
  enroll credibilityos.ai in Bing AI Performance (Paul's manual action); sanitize +
  publish raw baseline transcripts (queued); engine-split module REJECTED until a
  run fails without it (two GREEN runs so far).
- **Watch out:** Prediction files are append/score-only after commit — never loosen
  a registered band. The F2 file is qualitative (pre-rule-5); fix its operational
  band BEFORE the re-probe pull, never after.

## 2026-07-15 · claude-code

- **Did:** Initial public release (v1.0). Built the full skill clean-room from the
  evidence-tagged rulebook: SKILL.md orchestrator, 5 workflow modules, 2 templates,
  README, MIT license. TDD process documented in `tests/BASELINE-2026-07-15.md`
  (RED: 3 baseline scenarios all skipped the demand gate; GREEN: 5/5 criteria pass
  with skill loaded; REFACTOR: depth≠structure counter added and re-tested).
- **Why:** Public authority/distribution play — every rule traces to measured,
  published-receipt data; the baseline-vs-skill contrast is the differentiation.
- **Next:** Dogfood locally on the portfolio sites; score the open F2 re-probe
  prediction and re-score rules as new pulls land; consider a vertical-leaderboard
  worked example as a follow-up commit.
- **Watch out:** RULEBOOK.md receipts are pinned to their study dates — refresh only
  countable stats per the standing refresh rule, never the frozen narrative claims.
  Any future SKILL.md edit requires a failing test first (see tests/).
