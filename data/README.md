# Public data pack — AI citation dataset

Daily AI citation counts for the six-website portfolio behind this skill's
rulebook and the statistics page at
https://www.paultakisaki.com/insights/ai-seo-statistics/. Instrument: Bing
Webmaster Tools, AI Performance report, exported daily per verified property
and summed. Window: 2026-01-17 through 2026-11-01. A client site that shares
the same pipeline is excluded from every file and total here. A product site
that earned 7 citations in July 2026 left the pipeline in October 2026; its
citations are no longer in any file, so totals that include July read up to 7
lower than the 2026-10-05 and earlier editions (50,065 through 2026-08-05, not 50,072). License: CC BY 4.0
(cite Paul Takisaki with a link).

## Files

| File | What it is |
|---|---|
| `daily-portfolio-citations.csv` | Daily citations, all six sites summed (289 rows) |
| `weekly-cumulative-citations.csv` | Weekly totals + running total, weeks ending Sundays; the first row covers 2026-01-17 to 01-18 only, and the final row is a full week ending on the 2026-11-01 cutoff (42 rows) |
| `site-rollup-2026-11-01.csv` | Per-site lifetime, peak day, and trailing-7-day as of the cutoff |
| `page-rollup-2026-08-05.csv` | Page-level citation counts from Bing's Pages tab (a *sample*, per Bing; counters are rounded); retained at its original 2026-08-05 pull |

## Which file backs which statistic

The statistics page's claims (S01–S12) trace here:

- **S01 (260,771 total), S09 (October = 108,472), S11 (first citation Feb 22, 50,000 crossed Aug 5, 100,000 crossed Sep 9, 200,000 crossed Oct 19, 260,000 crossed Nov 1)** —
  `daily-portfolio-citations.csv`; the total is the column sum.
- **S08 (+37,467 week)** — `weekly-cumulative-citations.csv`, week ending 2026-10-25.
- **S05 (8,800+ single page), S12 (top-3 concentration)** —
  `page-rollup-2026-08-05.csv`, dated to its 2026-08-05 pull.
- **Site concentration (gaming site = 41.5%)** — `site-rollup-2026-11-01.csv`.
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
- Bing's dashboard shows daily per-site counts of 1,000 or more rounded to the
  nearest hundred (for example 2.5K). Those readings are summed as shown, so the
  last three digits of large totals are approximate; daily values under 1,000 are
  exact as reported.
- The Pages tab is labeled a sample by Bing and rounds large counters
  (8,800, 3,200, 1,400). Do not cross-foot page rollups against the daily series.
- The page rollup is retained at its 2026-08-05 pull because Bing's page-level
  sample has not been re-pulled in the pipeline since then; the portfolio total
  has since passed 260,000 while the page-level breakdown has not been refreshed.
- Rules in `../RULEBOOK.md` stay pinned to their frozen 26,767-citation study
  corpus (through 2026-07-13); this pack is the growth series, not new rule
  evidence.
