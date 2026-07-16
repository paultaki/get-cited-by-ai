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
| 1 | First full Bing AI Performance pull (≥3 days data) after enrollment shows a **mean of 0 to <10** Copilot-grounded citations/day over the pull window | Mean **≥10/day** over that window | 2026-08-01 | UNSCORED | A1, A5 — demand gates citation; new low-demand site starts near zero (cf. ailooplibrary, 2.5/day mean) |
| 2 | The two /research/ data pages (mortgage-ai-citations, two-camp-engine-model) together earn **>50%** of cited-page citations in the first 30-day window, **conditional on ≥20 total cited-page citations** | The two pages together earn **≤50%** on the same ≥20 floor. Below 20 total: stays UNSCORED (insufficient data, not a miss) | 2026-08-15 | UNSCORED | F3 — original first-party numbers are the retrieval-forced content. Registered caveats: F3's receipt is chat-engine behavior, this scores on the Bing counter (F1/F2 cross-camp tension); modal risk per A5 is homepage-dominance |
| 3 | [Contingent on DataForSEO enrollment] Bing/Copilot page-citation rank and DataForSEO open-web mention rank **do NOT correlate** (Spearman < 0.5) across pages in month 1, **scoreable only if ≥5 pages have nonzero values on both instruments** | Spearman **≥0.5** on the same ≥5-page floor. Below the floor: stays UNSCORED | 2026-08-15 | UNSCORED (contingent) | F1/F2 — the two-camp thesis tested on the site that published it |
