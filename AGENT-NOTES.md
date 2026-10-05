# Agent Notes

## 2026-10-05 · claude-code (150K milestone refresh)

- **Did:** README state line and RULEBOOK corpus-status → 150,000+ (155,286 through 2026-10-03, more than two thousand a day, September 65,632 record month, WoW −6.6%). Data pack regenerated through 10/03 (daily 260 rows, weekly 38 with the 6-day partial, `site-rollup-2026-10-03.csv`); page rollup retained at 2026-08-05. README states the client site sharing the pipeline is excluded from every total.
- **Why:** Monthly stats refresh; 150K crossed 2026-10-01 (10K milestone rule).
- **Next:** November refresh. Predictions untouched (no new scoring instruments ran).
- **Watch out:** CSVs must stay byte-identical with paultakisaki.com `insights/ai-seo-statistics/data/`.

## 2026-09-11 · claude-code (100K milestone + prediction ledger status)

- **Did:** README state line and RULEBOOK corpus-status → 100,000+ (102,133 through
  2026-09-09, close to two thousand a day). Data pack regenerated through 9/09 (daily 236
  rows, weekly 35 with the 3-day partial, `site-rollup-2026-09-09.csv`); `page-rollup-
  2026-08-05.csv` deliberately retained with a README caveat (Bing page sample not
  re-pulled in the pipeline since then). Prediction ledger, append-only: credibilityos
  #1 scored **HOLDS** (7 lifetime citations; mean/day < 10 under any window); dated
  status notes on credibilityos #2/#3, the F2 Bing-inverse re-probe, and all four TFL
  bets — every one of those is UNSCORED because the instrument was never run after
  2026-07-19 (no chat-engine probe wave, no DataForSEO mentions/AIO pull, grounding-query
  pull frozen). Not hits, not misses. Bands untouched.
- **Why:** Paul asked whether the studies and registered predictions still hold at the
  100K milestone. Memo: `~/Documents/Research/AI Citation Update 2026-09-11/`.
- **Next:** Re-window the TFL and F2 bets only after (a) mia's grounding-query pull
  resumes, (b) a DataForSEO mentions/AIO budget exists, (c) a probe battery is scheduled
  — and per rule 5 register the new window BEFORE reading the data.
- **Watch out:** Disclosure boundary applies to prose in this public repo, not just data
  files: a review caught per-site daily counts and a grounding-query share in my first
  draft of the notes; both removed. Per-site daily series and grounding queries never
  appear here in any form.

## 2026-09-02 · beast (GEO vocab-floor score finalized)

- **Did:** Closed multi-day ChatGPT scraper battery for `predictions/2026-07-16-paultakisaki-geo-hub-vocab-floor.md`. Outcome **HOLDS** (0/9 cited). Days: 2026-08-31, 2026-09-01, 2026-09-02. Raw cells under `data/vocab-floor-score-2026-08-31/`. Live-copy gate passed; instrument OK.
- **Why:** Score-by date 2026-08-31; G6 requires ≥3 separate days (≥9 cells). Null preregistration of vocabulary-floor-only intervention.
- **Next:** Ack loop until Paul replies `ack geo score`. Lever test remains separate.
- **Watch out:** Do not loosen the band. REFUTED would still need confound check before crediting the vocab edit (G8/G5). HOLDS is evidence for floor-not-lever on this page only.

## 2026-09-01 · beast (GEO vocab-floor score day 2/3)

- **Did:** Continued multi-day ChatGPT battery for
  `predictions/2026-07-16-paultakisaki-geo-hub-vocab-floor.md`. Live-copy gate
  PASS; instrument OK. Day-2 scored cells **0/3** cite paultakisaki.com
  (Q1–Q3); supplementary S1/S2 also 0. Running tally **0/6** across
  2026-08-31 + 2026-09-01. Raw under `data/vocab-floor-score-2026-08-31/`.
  Outcome left **UNSCORED**. Runner:
  `~/.hermes/scripts/geo-vocab-floor-score-day.py`.
- **Why:** G6 needs ≥3 separate days (≥9 cells). Day 2 is weather sample 2/3.
- **Next:** Day 3 cron 2026-09-02 09:05 PT finalizes HOLDS/REFUTED at ≥9 cells,
  then pending_ack Telegram confirm (`ack geo score`).
- **Watch out:** Do not loosen the band. Do not set final Outcome on <9 cells.
  Do not set pending_ack final nag until finalized.

## 2026-08-31 · beast (GEO vocab-floor score day 1/3)

- **Did:** Opened the score-by battery for
  `predictions/2026-07-16-paultakisaki-geo-hub-vocab-floor.md`. Scoreability
  floor PASS (live AEO/AI SEO string present; DataForSEO ChatGPT scraper OK).
  Day-1 scored cells **0/3** cite paultakisaki.com (Q1–Q3); supplementary S1/S2
  also 0. Raw under `data/vocab-floor-score-2026-08-31/`. Outcome left
  **UNSCORED** pending ≥2 more separate days (G6). Follow-up crons:
  geo-vocab-floor-score-day2 (2026-09-01 09:05 PT), day3 (2026-09-02 09:05 PT).
  Runner: `~/.hermes/scripts/geo-vocab-floor-score-day.py`.
- **Why:** Score-by date is today; single-day runs are weather. Null
  preregistration must not be closed on one sample.
- **Next:** Day 2 + day 3 auto-runs finalize to HOLDS/REFUTED at ≥9 cells, then
  pending_ack Telegram confirm (`ack geo score`).
- **Watch out:** Do not loosen the band. Do not set final Outcome on <9 cells.
  Bing AI Perf does not list the hub page among cited pages — secondary only.

## 2026-08-07 · claude-code (README current-state line refreshed to 50,000+)

- **Did:** README intro line updated: 40,000+ (39,911 through July 25) →
  50,000+ (50,072 through August 5, 2026, still adding ~900/day). Source:
  2026-08-07 full export, recomputed + decorrelated-verified in
  `~/Documents/Research/AI Citation Update 2026-08-07/`.
- **Why:** Stale current-state claim; the public playbook now says 50,000+ and
  the two surfaces must agree.
- **Next:** Nothing pending here. (Same-day follow-up: RULEBOOK header got a
  dated corpus-status note — portfolio passed 50,000 on 2026-08-05 — and README
  "What this is" got a cross-reference so the frozen 26,767 corpus doesn't read
  as stale next to the live counter. Rules untouched, provenance still pinned.
  Installed skill copy at ~/.claude/skills/get-cited-by-ai synced.)
- **Watch out:** The "26,767 first-party AI citations across six owned sites"
  dataset line is FROZEN study-corpus provenance — never sweep it forward.

## 2026-07-27 · claude-code (README current-state line refreshed)

- **Did:** README intro line updated: six sites / 26,767 → seven sites / 40,000+
  (39,911 through July 25, 2026, dated in-line). Source: 2026-07-27 full export,
  decorrelated-verified in `~/Documents/Research/AI Citation Update 2026-07-27/`.
- **Why:** Line was a stale *current-state* claim; the refreshed public playbook
  now says 40,000+, and the two surfaces must agree.
- **Next:** Nothing pending here.
- **Watch out:** The "26,767 first-party AI citations across six owned sites"
  dataset line further down is FROZEN study-corpus provenance (RULEBOOK evidence
  tags pin to it) — do not "fix" it to the current total.

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
