# Vertical Leaderboard — Step 5

Runs when the user asks "who wins in my space" or needs to pick build
targets. Free path first; the paid path is optional and bring-your-own-key —
never a prerequisite.

## 1. Free path: manual probe battery

1. Assemble a query set spanning the vertical's head terms to its long tail.
2. Probe each query across the engines, log cited/mentioned domains. Re-run
   ≥3× on separate days before citing any rate — single-run probes are
   weather; one site's cited-cell rate churned 1/6 → 0/48 between waves (G6).
3. Classify each winning domain by source type: government, national
   editorial, UGC (forums/wiki/video), vendor/brand. Head terms skew hard to
   aggregators — Reddit, YouTube, and Wikipedia ranked #1 in all 36 head-term
   leaderboards measured; the mortgage archive shows the same shape
   (HUD.gov, va.gov, Bankrate, NerdWallet, YouTube, Reddit dominant; 11 named
   working loan officers appeared zero times) (A7).
4. Find the tail cutoffs: several tail top-10 cutoffs sat at 1–9 mentions
   (A7) — single digits get a new entrant in. Flag these as entry points.
5. Run the two-camp overlap check per query: compare the Google-camp cited
   set against the open-web-camp cited set for the same queries. Cross-camp
   top-10 overlap on the same mortgage topics measured 4/10, 3/10, 6/10 (F1,
   TWO-CAMP) — expect partial overlap, report camp-by-camp, not one merged
   leaderboard.

## 2. Paid path (optional, bring-your-own-key): LLM-mention leaderboards

Only if the user has or wants an LLM-mentions key (e.g. DataForSEO). Apply
every G4 instrument rule before making any claim from this data:

- Read one month in arrears — ChatGPT corpora batch-ingest monthly, ≥2-week
  lag (G4a).
- Small domains may have no usable pre-history (G4b).
- Treat matches as word-bag, not phrase-level — one series showed 4,257
  mentions for a product season before that season existed (G4c).
- Compare share/ratio metrics only, never raw counts — raw counts are
  corpus-growth-dominated, a ~10–20× uniform rise across unrelated topics
  (G4d).
- New/Lost deltas measure sampling churn on small targets, not decay (G4e).
- One keyword per request — brand endpoints can AND-match multi-keyword
  targets (G4f).
- Check coverage before making a site claim — a site can be #1 first-party
  and absent from the corpus entirely (G4g).
- Never single-snapshot a leaderboard — same-day reruns showed only ~32–43%
  source overlap (G4h).

## Output: LEADERBOARD READ

Deliver an entry-point list plus a camps analysis. Every row cites its rule
ID; paid-path rows additionally cite which G4 sub-rule was applied.

```
LEADERBOARD READ
- Entry points (thin, single-digit top-10 cutoffs): [query — cutoff count] (A7)
- Source-type breakdown at head: [gov/editorial/UGC/vendor %] (A7)
- Two-camp overlap per query: [N]/10 shared domains (F1)
- Paid-path data used: yes/no — G4 rules applied: [list sub-rules] (G4)
- Re-run count: [N] (G6)
```
