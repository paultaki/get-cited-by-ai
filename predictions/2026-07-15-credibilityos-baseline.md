# Registered: credibilityos.ai citation baseline

- **Registered:** 2026-07-15 (this file's first commit date is the receipt)
- **Context:** First audit of credibilityos.ai found it absent from every AI-citation
  instrument in the portfolio (never enrolled in the Bing AI Performance rotation or
  the LLM-mentions pulls — only GSC/GA4 existed, which cannot see AI engines). These
  predictions register BEFORE enrollment, so the first pull scores them cold. Full
  audit: `examples/credibilityos-audit.md`.
- **Instrument:** Bing Webmaster AI Performance exports (canonical apex host);
  optional DataForSEO LLM-mentions for #3.
- **Amendment note:** conditions tightened same-day (2026-07-15) after an adversarial
  logic review, before any scoring data existed — the original #1 had a boundary
  overlap at exactly 10 and no named statistic; the original #2's refutation was not
  the complement of its band. Template rule 5 was added because of these defects.

| # | Prediction (band) | Refutation | Score-by | Outcome | Rules tested |
|---|---|---|---|---|---|
| 1 | First full Bing AI Performance pull (≥3 days data) after enrollment shows a **mean of 0 to <10** Copilot-grounded citations/day over the pull window | Mean **≥10/day** over that window | 2026-08-01 | HOLDS | A1, A5 — demand gates citation; new low-demand site starts near zero (cf. ailooplibrary, 2.5/day mean) |
| 2 | The two /research/ data pages (mortgage-ai-citations, two-camp-engine-model) together earn **>50%** of cited-page citations in the first 30-day window, **conditional on ≥20 total cited-page citations** | The two pages together earn **≤50%** on the same ≥20 floor. Below 20 total: stays UNSCORED (insufficient data, not a miss) | 2026-08-15 | UNSCORED | F3 — original first-party numbers are the retrieval-forced content. Registered caveats: F3's receipt is chat-engine behavior, this scores on the Bing counter (F1/F2 cross-camp tension); modal risk per A5 is homepage-dominance |
| 3 | [Contingent on DataForSEO enrollment] Bing/Copilot page-citation rank and DataForSEO open-web mention rank **do NOT correlate** (Spearman < 0.5) across pages in month 1, **scoreable only if ≥5 pages have nonzero values on both instruments** | Spearman **≥0.5** on the same ≥5-page floor. Below the floor: stays UNSCORED | 2026-08-15 | UNSCORED (contingent) | F1/F2 — the two-camp thesis tested on the site that published it |

- **Scored 2026-09-11 (claude-code), instrument: Bing Webmaster AI Performance daily export, mia pipeline pack generated 2026-09-11 05:09 (series 2026-01-17 → 2026-09-09).** Enrollment landed between registration (2026-07-15) and the first query-pull status row for credibilityos.ai (2026-07-19 09:10); the first archived pack containing the site is 2026-07-27 (series to 07-25). Per the public site rollup (`data/site-rollup-2026-09-09.csv`): **7 citations lifetime** through 2026-09-09, peak day 2, trailing-7 = 0. (Per-site daily rows stay private by the 2026-08-09 disclosure rule; the scoring below needs only the lifetime total.)
  - **#1 → HOLDS.** With 7 lifetime citations in total, the mean over ANY window of ≥3 days is at most 7/3 ≈ 2.3/day, and over the first full pull window after enrollment it is below that. Every admissible window gives a mean in [0, <10); the result is invariant to the window choice. Refutation (≥10/day) not reached under any reading.
  - **#2 → stays UNSCORED per its own registered terms.** Total cited-page citations in the first 30-day window ≤ 7, below the ≥20 floor, so the conditional never triggers ("insufficient data, not a miss"). Note also that Bing's page-level sample for this site has not refreshed in the pipeline since 2026-08-07, so the page split could not be read even if the floor were met.
  - **#3 → stays UNSCORED (contingent instrument not enrolled).** credibilityos.ai was never enrolled in the DataForSEO LLM-mentions pull; no month-1 mention ranks exist, so the ≥5-page both-instruments floor cannot be evaluated.
  - Band untouched. Raw pack archived at `~/Documents/Research/AI Citation Update 2026-09-11/raw/` (private; per-site daily rows are not published).

