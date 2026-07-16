# Agent Notes

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
