# Measurement Harness — Step 6 (every engagement ends here)

No engagement closes without this block (SKILL.md).

## 1. Instruments (free path first)

1. Bing Webmaster Tools, verified on canonical host. Pull all three AI Performance
   exports — daily series, page counters, grounding queries — the primary free
   first-party citation counter, read under G3's export mechanics (G2 is why
   referral traffic is no substitute).
2. IndexNow, submitted day zero with sitemap/robots. Onset can be days not months
   (D4: 0/10/64-day spread across 4 sites); causal share is INFERENTIAL, fan-out
   reaches Bing/Yandex only.
3. GA4 confirmed live, each property's first-data date checked before any window
   comparison (G7).

## 2. Instrument rules — apply on every read

- Bing exports (G3): tail days restate upward, read as floors (a). Export types
  don't reconcile by construction — state totals as ranges (b). Grounding-queries
  export is partial/thresholded — directional only (c). Canonicalize www/apex
  before joining (e). Parse dates, never string-sort — a past lexicographic sort
  produced a wrong window that survived two analysts (g).
- Citations ≠ clicks (~112:1 portfolio-wide): treat citations as exposure, not
  traffic; clicks concentrate on interactive tools, not the most-cited pages (G2).
- Ban the mechanical-accumulation fallacy: "N% of citations arrived since X
  shipped" is what a flat rate produces on its own — never treat it as effect
  evidence (G8).
- Non-stationary series break naive before/after reads: one site booked 87.6% of
  all-time citations in its final 30 days — ramp-phase data needs registered
  predictions, not baselines (G5).
- Single-run probes are weather: re-run ≥3× before citing a rate; direction is the
  finding, not the number (G6).
- GA4: pull the full sessionSource list rather than pre-filtering an assumed
  AI-source list (missed copilot.com, undercounted AI sessions ~46% on one site);
  a single user can masquerade as an engine trend (G7).

## 3. Registered predictions

Before shipping any change: dated prediction, numeric band, explicit refutation
condition — score it at the next pull (G1). The refutation must be the band's
logical complement, with a named statistic and a scoreability floor (template
rule 5 — added after two production audits independently registered unscoreable
predictions). Worked example, the book's own ledger:

1. TFL settles 250–500/day post-event → HOLDS, band edge (589/day).
2. Merit reaches ≥100 cited pages in a day by August → HIT early (127 on 07/13).
3. HW stays 25–50/day → HOLDS, watch (53.1/day avg).
4. ailooplibrary under 10/day until demand exists → HOLDS (2.5/day).
5. Fragmentation call (hubs beat per-entity pages) → scored ~17× (A2).
6. Bing-inverse chat-engine re-probe (F2) → registered, unscored.

## 4. Optional paid tier (bring-your-own-key)

LLM-mention indexes (e.g. DataForSEO) add coverage under their own rules (G4):
batch-ingest monthly, ≥2-week lag — read one month in arrears (a); word-bag
matching makes phrase-level claims invalid (c); raw counts are
corpus-growth-dominated — only share/ratio metrics hold over time (d); check
coverage before any site claim, a site can be #1 first-party and absent from the
corpus (g); reruns of archive leaderboards show only ~32–43% overlap — never
single-snapshot a leaderboard (h).

## Output: MEASUREMENT PLAN

```
MEASUREMENT PLAN
- Instruments configured: Bing Webmaster (AI Performance exports) / IndexNow / GA4
  (sessionSource confirmed) / [paid: LLM-mention index if used]
- Baseline window: [start] – [end]; canonical host: [apex/www]
- Registered predictions:
  1. [claim] — band: [X-Y/unit] — refutation: [condition] — registered [date]
  2. ...
- Next review date: [date]
```
