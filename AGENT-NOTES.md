# Agent Notes

## 2026-07-17 · claude-code (author-voice pass)

- **Did:** Voice pass across the public repo. README rewritten in Paul's register
  (PaulVoice pack, register 9, voice-lint PASS); 244 em/en dashes recast across
  RULEBOOK/SKILL/modules/templates/example plus 18 more inside fenced output
  templates, meaning-preserving only. Verify gate: numeric fingerprint (all numbers
  extracted and hashed per file) byte-identical before and after on every edited
  file. Logged in tests/EDITS as presentation-only.
- **Why:** Repo is authored under Paul's name and promoted from his account; 300+
  em dashes read as machine-written and violate his published voice contract.
- **Next:** None for this pass. Prediction score dates unchanged (nearest 08-01).
- **Watch out:** predictions/ and tests/ history stay dash-y ON PURPOSE (append-only
  receipts). Future prediction files should be written to the voice contract at
  registration time. One em dash survives in SKILL.md's rationalization table inside
  a verbatim quoted baseline claim. Do not "fix" any of these.

## 2026-07-16 · claude-code (prediction registered, later same day)

- **Did:** Ran the skill's own step-1 demand probe on the skill's own topic
  (DataForSEO). Result: topic PASSES the gate (ChatGPT grounds + cites on all 3
  target queries), paultakisaki.com cited in 0/3, and query demand sits under the
  aliases "AI SEO" (8,100/mo) + "answer engine optimization / AEO" (2,400/mo) while
  "generative engine optimization" and "get cited by AI" show no reportable volume.
  Registered a preregistration: `predictions/2026-07-16-paultakisaki-geo-hub-vocab-floor.md`,
  committed BEFORE the intervention it describes.
- **Why:** Dogfood + credibility. The prediction registers the NULL on purpose (A1/
  C1/B3 say on-page vocabulary is a floor, not a lever), so a confirmed 0 is public,
  timestamped evidence for the thesis on the author's own property.
- **Next:** Score-by 2026-08-31 via the ChatGPT-scraper battery (≥3 runs, G6); verify
  page indexation first or VOID. The LEVER test (demand/source-depth) is a separate
  later prediction.
- **Watch out:** Do NOT loosen the band after registration. The intervention was a
  deliberately reasonable floor (meta + one body line, branded title left intact),
  not a maximal stuffing — a null does not rule out that an aggressive version would
  differ, and the file says so.

## 2026-07-16 · claude-code

- **Did:** Promotion-readiness pass on the public README. Added a plain-language
  lead paragraph above the formal descriptor (the front door assumed the reader
  already shared the vocabulary — no hook, undefined GEO/AEO, terms of art before
  any value prop); expanded GEO/AEO on first use. Logged the change in the edit
  log as presentation-only. Nothing in SKILL.md / RULEBOOK / modules changed.
- **Why:** Prepping the repo to promote. The rigor is the asset, so the fix was
  additive (a plain on-ramp above the depth), not a dumbing-down.
- **Next:** Optional — verify the four published research URLs still resolve before
  driving traffic at the repo. Score predictions at their score-by dates.
- **Watch out:** Deliberately did NOT add causal lift metrics (portfolio +272% /
  +154% / +13%). Framing the repo around "deploy these practices → +N% citations"
  self-refutes under the skill's own G5 (ramp non-stationarity) and G8 (mechanical
  accumulation) and would spend the honesty moat that is the whole differentiation.
  If lift numbers are ever used, they go in as observed-correlational portfolio
  context with the demand confound stated, never as attributed lift, and never in
  the hook.

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
