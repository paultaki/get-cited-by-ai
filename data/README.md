# Public data pack — AI citation dataset

Daily AI citation counts for the seven-website portfolio behind this skill's
rulebook and the statistics page at
https://www.paultakisaki.com/learn/ai-seo-statistics/. Instrument: Bing
Webmaster Tools, AI Performance report, exported daily per verified property
and summed. Window: 2026-01-17 through 2026-08-05. License: CC BY 4.0
(cite Paul Takisaki with a link).

## Files

| File | What it is |
|---|---|
| `daily-portfolio-citations.csv` | Daily citations, all seven sites summed (201 rows) |
| `weekly-cumulative-citations.csv` | Weekly totals + running total, weeks ending Sundays; the final row is a 3-day partial through 2026-08-05 |
| `site-rollup-2026-08-05.csv` | Per-site lifetime, peak day, and trailing-7-day as of the cutoff |
| `page-rollup-2026-08-05.csv` | Page-level citation counts from Bing's Pages tab (a *sample*, per Bing; counters are rounded) |

## Which file backs which statistic

The statistics page's claims (S01–S12) trace here:

- **S01 (50,072 total), S09 (July = 31,324), S11 (first citation Feb 22)** —
  `daily-portfolio-citations.csv`; the total is the column sum.
- **S08 (+8,859 week)** — `weekly-cumulative-citations.csv`, week ending 2026-07-12.
- **S05 (8,800+ single page), S12 (top-3 concentration)** —
  `page-rollup-2026-08-05.csv`.
- **Site concentration (gaming site = 48.5%)** — `site-rollup-2026-08-05.csv`.
- **S02 (112:1), S03 (4.42 odds), S04 (84% zero), S06 (99% vs 66%), S07 (7x),
  S10 (4 vs 64 days)** — derived in the frozen study corpus documented in
  `../RULEBOOK.md` (receipts G2, A1, B3, and the time-to-citation study); the
  regression inputs include unpublished per-page internals. Method and exact
  receipt values are in the rulebook; further cuts available on request.

## Honest caveats

- Bing's counter only sees Microsoft AI surfaces (Copilot, Bing AI). Totals are
  floors, not internet-wide counts.
- The last day or two of any pull can restate upward on later exports; treat
  tail values as floors.
- The Pages tab is labeled a sample by Bing and rounds large counters
  (8,800, 3,200, 1,400). Do not cross-foot page rollups against the daily series.
- Rules in `../RULEBOOK.md` stay pinned to their frozen 26,767-citation study
  corpus (through 2026-07-13); this pack is the growth series, not new rule
  evidence.
