# Site Audit Report

Fill every bracket. Every row in every table carries a rule ID — a row with
no rule ID is an opinion, not a finding, and doesn't ship.

**Site:** [domain]
**Date:** [YYYY-MM-DD]
**Prepared per:** geo-evidence workflow (SKILL.md steps 1–6)

## Demand Verdict

Paste the DEMAND VERDICT block from `modules/demand-probe.md`:

```
- Demand exists: yes / no / unknown
- Instrument: Bing grounding-queries export | manual probe battery (n runs, dates)
- Shape: aggregate-comparative | single-entity | single-question | mixed
- Memory-answerable: yes (engines) / no (engines) / mixed
- Ride-along flag: yes/no
- Densify-first flag: yes/no (existing capture %)
```

If demand does not exist or the niche is memory-answerable, stop here and
say so (F3, A5) — do not proceed to floors or levers.

## Target Camp

[Google camp / open-web camp / Copilot-Bing / mixed] — state which camp(s)
this report targets and why, per step 2 and F1 (TWO-CAMP).

## Floors

| # | Item | Pass / Fail | Fixed? | Rule ID |
|---|------|-------------|--------|---------|
| 1 | Crawlability for AI bots (robots, sitemap) | | | D6 |
| 2 | Content present per target camp's fetch behavior | | | D1 |
| 3 | Canonical host, no duplicate-answer URLs | | | E1, E2 |
| 4 | Redirects planned for retired URLs | | | E3 |
| 5 | Schema shipped as hygiene (not credited as a lever) | | | C1, C2 |
| 6 | llms.txt shipped as hygiene (not credited as a lever) | | | D5 |
| 7 | Day-zero fundamentals (new sites only) | | | D4 |
| 8 | [entity-probe.md ran? identity consistency / name collision] | | | C3, C4 |
| + | [add rows for anything site-specific found] | | | |

## Levers

| Recommendation | Rule ID + evidence tag | Expected instrument to watch |
|---|---|---|
| [e.g., build one aggregate hub for X demand] | A2, PREDICTED-AND-SCORED | Bing Webmaster page counters, target page |
| [answer-first block, 40–70 words] | B1, OBSERVED-CORRELATIONAL (inferential) | Bing Webmaster daily series |
| [structured units, demand-qualified pages only] | B2, OBSERVED-CORRELATIONAL | Bing Webmaster page counters |
| [day-zero event page] | A3, VALIDATED-INTERVENTION | Bing Webmaster daily series, event window |
| [densify winner page X] | A8, OBSERVED-CORRELATIONAL | Bing Webmaster grounding-query pool |
| [one-question page for query Y] | B4, OBSERVED-CORRELATIONAL | Bing Webmaster page counters |
| [comparison/alternatives page] | B5, OBSERVED-CORRELATIONAL (thin) | Manual probe, re-run ≥3× |
| [row per recommendation actually made — delete unused rows] | | |

## Explicitly NOT Recommended

| Item | Why | Rule ID |
|---|---|---|
| Schema/JSON-LD as the highest-leverage task | Biggest page: 5,179+ citations, zero JSON-LD; uncited pages carry more schema | C1, B3 |
| Question-shaped H2s / FAQs as levers | Uncited pages score higher on both | B3 |
| llms.txt as an edge with no downside | Untestable constant; most polished example on a zero-citation site | D5 |
| Blanket "AI crawlers can't read JS" | Bing renders JS; per-engine, not universal | D1 |
| SSR alone as the fix | Shipped on a zero-citation site, still zero 3.5 weeks later | D2 |
| Freshness as a measurable factor | No such finding in the dataset | — |
| "Publish more pages" as default | Headroom sits in existing winners, ~22–26% capture | A8 |
| [any other rejected recommendation specific to this site] | | |

## Measurement Plan + Registered Predictions

Paste the MEASUREMENT PLAN block from `modules/measurement-harness.md`:

```
- Instruments configured: Bing Webmaster (AI Performance exports) / IndexNow / GA4
  (sessionSource confirmed) / [paid: LLM-mention index if used]
- Baseline window: [start] – [end]; canonical host: [apex/www]
- Registered predictions:
  1. [claim] — band: [X-Y/unit] — refutation: [condition] — registered [date]
  2. ...
- Next review date: [date]
```

Log every registered prediction in `templates/prediction-ledger.md` and score
it there at the next pull — a plan with no registered prediction is folklore
with confidence (G1, SKILL.md).
