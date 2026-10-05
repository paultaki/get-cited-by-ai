# Public data pack — AI citation dataset

Daily AI citation counts for the seven-website portfolio behind this skill's
rulebook and the statistics page at
https://www.paultakisaki.com/insights/ai-seo-statistics/. Instrument: Bing
Webmaster Tools, AI Performance report, exported daily per verified property
and summed. Window: 2026-01-17 through 2026-10-03. A client site that shares
the same pipeline is excluded from every file and total here. License: CC BY 4.0
(cite Paul Takisaki with a link).

## Files

| File | What it is |
|---|---|
| `daily-portfolio-citations.csv` | Daily citations, all seven sites summed (260 rows) |
| `weekly-cumulative-citations.csv` | Weekly totals + running total, weeks ending Sundays; the final row is a 6-day partial through 2026-10-03 (38 rows) |
| `site-rollup-2026-10-03.csv` | Per-site lifetime, peak day, and trailing-7-day as of the cutoff |
| `page-rollup-2026-08-05.csv` | Page-level citation counts from Bing's Pages tab (a *sample*, per Bing; counters are rounded); retained at its original 2026-08-05 pull |

## Which file backs which statistic

The statistics page's claims (S01–S12) trace here:

- **S01 (155,286 total), S09 (September = 65,632), S11 (first citation Feb 22, 50,000 crossed Aug 5, 100,000 crossed Sep 9, 150,000 crossed Oct 1)** —
  `daily-portfolio-citations.csv`; the total is the column sum.
- **S08 (+16,163 week)** — `weekly-cumulative-citations.csv`, week ending 2026-09-27.
- **S05 (8,800+ single page), S12 (top-3 concentration)** —
  `page-rollup-2026-08-05.csv`, dated to its 2026-08-05 pull.
- **Site concentration (gaming site = 35.9%)** — `site-rollup-2026-10-03.csv`.
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
- The page rollup is retained at its 2026-08-05 pull because Bing's page-level
  sample has not been re-pulled in the pipeline since then; the portfolio total
  has since passed 150,000 while the page-level breakdown has not been refreshed.
- Rules in `../RULEBOOK.md` stay pinned to their frozen 26,767-citation study
  corpus (through 2026-07-13); this pack is the growth series, not new rule
  evidence.
