# Worked example: credibilityos.ai audit (2026-07-15)

A complete, real run of this skill against one of the author's own sites, included
because it demonstrates the path no checklist tool can show: **the demand gate
blocking every craft recommendation**, and the engagement routing to measurement
instead. Names and numbers are real (this repo's receipts policy); the operator's
errors are left visible in the adversarial-pass log at the bottom, because that
discipline is part of the method.

**What makes this run instructive:** credibilityos.ai is a schema-rich site: 158
Question/Answer entries, FAQPage on 16 pages, a textbook Person entity with a 10-URL
sameAs array. A folklore audit reads that and says either "you're optimized" or "add
more." This skill said neither, because step 1 found something that outranks all of
it.

---

## Step 1: DEMAND VERDICT

```
- Demand exists:     UNKNOWN (never measured with a grounding instrument;
                     GSC organic near-zero but wrong instrument for AI grounding, G2)
- Instrument:        NONE of the right kind. Absent from the Bing AI Performance
                     rotation AND every LLM-mentions pull. Only GSC + GA4 exist,
                     and neither can see AI engines.
- Shape:             aggregate-comparative + single-question (inferred from site
                     content, provisional: no real grounding-query list exists yet)
- Memory-answerable: UNKNOWN. No grounding data, manual probe battery not yet run
- Target camp:       open-web + Google camp (the site's own product targets
                     ChatGPT/AIO/Perplexity/Gemini/Claude); Bing/Copilot is the only
                     free first-party instrument
- Ride-along flag:   no
- Densify-first:     N/A, capture % unknowable without a grounding pool
```

**Headline finding:** credibilityos.ai has **no AI-citation measurement footprint**.
The author's other six properties are all wired into Bing AI Performance and/or
LLM-mentions tracking; this one was routed into a one-off GSC/GA4 pull: standard
organic-search tooling that cannot see whether any AI engine cites you. The question
"is this site cited by AI" had never been asked of the data. Per G2
(citations:clicks ≈ 112:1), zero AI-referral sessions in GA4 is NOT evidence of
citation absence: it's the wrong instrument reporting. An adversarial re-check
(below) confirmed the absence claim against every instrument in the portfolio.

**Iron Rule consequence:** with demand UNMEASURED, every craft recommendation is
blocked. No schema advice, no content plan, no "add FAQs." The engagement routes to
step 6: build the instrument first.

## Step 4: Entity check (run because the subject is a person-anchored brand)

One false gap cleared, one real gap found, both only visible at schema level, not
link level:

- **Person graph: UNIFIED.** credibilityos.ai and paultakisaki.com declare the same
  Person with the exact same `@id` (`https://www.paultakisaki.com/#person`),
  character-for-character, with mutual sameAs arrays. The operator's prior hand-guess
  of a cross-property entity gap was falsified here: proper entity resolution
  existed (C3/C4).
- **Organization graph: INCONSISTENT.** credibilityos.ai declares
  `worksFor → https://credibilityos.ai/#organization` (and defines the node);
  paultakisaki.com never references that `@id` and points `worksFor` at a different
  org, plus it binds the brand through a separate `WebApplication` node nothing
  connects to the org node. Conflicting employer contexts, two same-named entities.
- **Honest tag:** entity-consistency **hygiene** (C1/B3: floors, not levers). The fix
  was delivered with NO citation-lift promise and NO citation prediction registered:
  any post-fix citation movement must survive the G8 mechanical-accumulation check
  before anyone calls it an effect.
- **Iron Rule tension, stated openly:** shipping even a hygiene patch while demand is
  unmeasured cuts close to the Rule's letter. It stayed defensible because the patch
  edits paultakisaki.com (a site that IS enrolled in the demand instrument) and
  carries no recommendation dressed as a lever. A future skill edition should draw
  the hygiene-vs-recommendation boundary explicitly.

## Step 6: MEASUREMENT PLAN

```
- Instruments to configure:
  1. Bing Webmaster Tools: verify on canonical apex host, enroll in AI Performance,
     pull all three exports (daily series, page counters, grounding queries) under
     G3's mechanics: tails are floors, exports don't reconcile (state ranges),
     query export is directional only, parse dates never string-sort.
  2. IndexNow: day zero, sitemap/robots current (D4, attribution INFERENTIAL).
  3. GA4: confirm first-data date before any window compare; pull the FULL
     sessionSource list, never a pre-filtered AI list (G7).
  4. [Optional, bring-your-own-key] LLM-mentions index: month-in-arrears,
     share/ratio metrics only, check coverage first (G4).
- Baseline window: opens at enrollment; first solid pull ~2 weeks later.
- Read discipline: ramp-phase series → registered predictions, not before/after
  baselines (G5); re-run probes ≥3× (G6); no "N% since X shipped" claims (G8).
```

**Registered predictions:** three, committed the same day in
`predictions/2026-07-15-credibilityos-baseline.md`: a near-zero first-pull band
(A1/A5), a research-pages-lead-share band with a scoreability floor (F3, with its
cross-camp caveat declared at registration), and a contingent two-camp
non-correlation test (F1/F2). The site that published the Two-Camp Engine Model now
has its own thesis registered against it.

---

## Adversarial-pass log (fresh-context verifier, author ≠ verifier)

The audit's factual spine survived attack: the absence claim held against an
exhaustive re-check of every instrument in the portfolio; the entity `@id` claims
verified character-for-character on the primary HTML; the schema patch validated as
correct JSON-LD where scoped. **Four defects were found and corrected before
publication:** (1) one prediction's refutation condition was not the complement of
its band: outcomes existed where neither fired, and the neither-fires case was the
rulebook's own documented modal outcome (A5 homepage-dominance); (2) another
prediction had a boundary overlap at its threshold and no named statistic; (3) the
entity patch's target-page enumeration was contaminated with the wrong site's page
list, and its first edit was mechanically inapplicable to 14 of 15 real target pages
(three different JSON-LD shapes); (4) "dangling edge" framing overstated the org
defect, and an existing `WebApplication` node that already bound the brand went
unmentioned. One rule miscite (A8→A1) was also corrected. These defects (plus the
same non-complementarity class appearing independently in a second audit the same
day) are the documented failing test behind prediction-ledger rule 5.

**The lesson this example exists to teach:** the facts survive; the precision layer
is where the author's errors live. Run the verifier.
