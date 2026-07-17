# Demand Probe: Step 1 Gate

No downstream module runs without this block (Iron Rule, SKILL.md).

## 1. Does grounding demand exist

1. Site enrolled in Bing Webmaster Tools? Pull the grounding-queries export (one of
   three AI Performance exports: daily series, page counters, grounding queries):
   the primary free demand instrument. Treat it as partial and thresholded:
   coverage ran 11-43% of page totals across pulls, directional not exhaustive
   (G3c).
2. Not enrolled, or no history yet? Run a manual probe battery of the target queries
   across available engines, plus free proxies (People-Also-Ask, autocomplete) as
   demand HINTS only: label as weaker than a first-party grounding export: query
   interest, not grounding behavior.
3. Either path is one pull. Re-run on ≥3 separate days before treating any rate as a
   finding: single-run probes are weather, not climate (G6).

## 2. What shape is the demand

- Aggregate-comparative (queries name no single entity) → one dense hub, never
  fragment into per-entity pages (A2, strongest rule here: 6 hubs earned ~17× the
  per-page rate of 18 per-entity pages on the same site).
- Single-entity (queries DO name individual entities) → per-entity pages are viable;
  A2's fragmentation warning applies only when demand is aggregate, not
  entity-named.
- Single-question (programmatic Q&A, one query = one question) → one page per
  question, never bundle (B4: CollegeVine earns ~14,000 mentions via 56
  single-question pages).
Let the step-1 query list decide the shape. Do not guess.

## 3. Memory-answerability check

Run the actual target queries (not paraphrases) across the engines you can reach and
note, per engine, whether it searched/grounded or answered from memory. F3: one wave
found 14 of 48 engine-cells never searched (ChatGPT 6/12, Claude 8/12, Gemini 8/12,
Perplexity 12/12); all four memoir-niche queries drew memory answers from three
engines independently. If a topic looks memory-answerable, say so and state the
honest outcome: change topics, or publish only what parametric memory cannot answer:
current prices, comparisons, news, original first-party numbers (F3).
Comparison/alternatives phrasing directionally forces retrieval over memory recall
(B5, thin, directional).

## 4. Ride-along and densify checks

- Flag demand riding a dated event or news cycle rather than durable interest;
  segment it out of trend reads: it fades even as raw citations keep climbing
  in-window (A6).
- Before recommending new pages, check existing capture against the grounding-query
  pool: sites in this dataset captured only ~22-26% of pools they already appear in
  (A8): densify winners first if capture is low.

## Output: DEMAND VERDICT

```
DEMAND VERDICT
- Demand exists: yes / no / unknown
- Instrument: Bing grounding-queries export | manual probe battery (n runs, dates)
- Shape: aggregate-comparative | single-entity | single-question | mixed
- Memory-answerable: yes (engines) / no (engines) / mixed
- Target camp (preliminary): Google camp | open-web camp | Bing/Copilot | unclear
- Ride-along flag: yes/no
- Densify-first flag: yes/no (existing capture %)
```

Downstream modules require this block before they run.
