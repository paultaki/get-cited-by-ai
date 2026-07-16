# The GEO Evidence Rulebook (Public Edition — v1.0)

Rules for earning citations from AI search engines, derived from a measured dataset:
**26,767 Bing-reported AI citations across 6 owned sites (through 2026-07-13), a
751-page same-template controlled regression, two independently-run studies that converged,
four-engine live probes, an 820K-citation vertical archive study, and a registered-
prediction ledger with scored outcomes.**

Every rule carries an evidence class, a named receipt, and a scope limit. This
document tells you what the data supports, what it merely suggests, and what it
cannot support — including where it contradicts common GEO advice. Nothing here is
folklore: if a rule is untested, it says so.

**v1.0 — released 2026-07-15. Every receipt was re-derived from primary sources by
independent reviewers before release (see Methods); the sanitization audit passed
with the author's disclosure decisions applied. Rules are re-scored as the
underlying dataset grows; see the prediction ledger (G1) for what's still open.**

**v1.0.1 errata — 2026-07-15, same day.** Two decorrelated post-release reviews
caught precision overstatements in the framing (not the rules): "controlled template
experiment" → "same-template controlled regression" (the design is observational —
A1's own tag says so); one module miscited G2 where G3's export mechanics apply; one
module said a www/apex split "cost" mentions where E1's receipt says they sat
miscounted on the alternate host; one module dropped D4's INFERENTIAL qualifier on
IndexNow. No rule, receipt, or number changed. The edit log in `tests/` maps each fix
to its documented failing check.

## How to read the tags

| Tag | Meaning |
|---|---|
| PREDICTED-AND-SCORED | A dated, registered prediction later scored against fresh data — the strongest class here |
| VALIDATED-INTERVENTION | A shipped change with a measured before/after citation effect |
| NEGATIVE-RESULT | An intervention or condition that did NOT move citations in the observed window |
| FALSIFIED-AS-UNIVERSAL | A common industry claim contradicted by a named counterexample in this data |
| OBSERVED-CORRELATIONAL | A pattern in the data; no causal claim |
| INSTRUMENT-RULE | A rule about measurement itself — how to read the data without fooling yourself |
| STANDARD-UNTESTED | Industry practice this dataset could not test; kept, marked honestly |
| EXTERNAL-SOURCED | From third-party published data |

Scope discipline: the dataset is n = 6 owned sites (gaming tools, college merit aid,
family-memoir SaaS, AI tools, personal brand) plus one vertical archive study
(mortgage), US/English, with Bing Copilot as the primary first-party counter.
Rules state the sites, engines, and windows they were observed on. Universality is
earned by re-validation on YOUR site via the measurement harness — never asserted
from this dataset alone.

## Source key

| Key | What it is | Availability |
|---|---|---|
| STUDY-1 | Three-site citation study (2026-06-20): ~9,500 citations, 751-page controlled regression, cross-engine probe wave 1, independent dual-analyst design + red team | Findings summarized at PLAYBOOK; full memo unpublished |
| STUDY-2 | Independent replication (2026-07-01): fresh analyst, adversarial two-round verification gate, 4-engine probe wave 2, drift detection | Unpublished; convergence with STUDY-1 is the replication claim |
| UPDATES | Longitudinal update memos (2026-07-13 and 07-15): registered predictions scored, 378 reconciled site-days | Unpublished |
| FINDINGS | DataForSEO Extended LLM-mentions pull findings F1–F9 (2026-07-14); 8/8 headline numbers blind-verified by a fresh-context reviewer | Unpublished |
| PLAYBOOK | paultakisaki.com/learn/how-to-get-cited-by-ai/ | Published, maintained |
| MORTGAGE | credibilityos.ai/research/mortgage-ai-citations/ | Published |
| TWO-CAMP | credibilityos.ai/research/two-camp-engine-model/ | Published |
| LOCAL-PRO | credibilityos.ai/learn/ai-visibility-for-local-professionals/ | Published |

Sites named throughout: thefinalsloadout.com (TFL), meritplaybook.com (Merit),
heritagewhisper.com (HW), ailooplibrary.com, askthree.ai, paultakisaki.com — all
operated by the author. The receipts are real and the sites are inspectable; that is
the point.

---

## A. Demand & topic selection (the gate)

**A1 · OBSERVED-CORRELATIONAL (controlled template; replicated)** — Demand gates
citation; craft cannot substitute for it. Do not build without a confirmed demand
signal.
Receipt: 751 pages on one identical Merit template — pages whose school has a Common
Data Set entry (demand proxy) were cited 46.6% of the time (n=73) vs 6.2% without
(n=678); demand odds ratio 4.42 (p=0.003); word count OR 1.09 (not significant). The
counterexample is pinned: a 2,713-word University of Alabama page with a full dataset
earned zero citations, confirmed three ways. Two independently-run studies converged
on this model.
Scope: meritplaybook.com template, Bing Copilot, through 07/2026.
Source: STUDY-1; STUDY-2.

**A2 · PREDICTED-AND-SCORED** — Match page shape to demand shape: build one dense
aggregate hub for aggregate-comparative queries; never fragment into per-entity pages
when grounding queries don't name single entities. (The strongest rule in this book.)
Receipt: registered in June (0 of 45 TFL grounding queries named a single weapon; the
red team pre-declared per-weapon pages would starve); scored in July: 6 aggregate hubs
earned 179 citations (~30/page; /loadouts alone 127) vs 18 per-weapon pages earning 32
total (~1.8/page) — a ~17× per-page advantage; re-confirmed two weeks later (13 weapon
URLs totaled 84 citations while the hubs above them added thousands).
Scope: thefinalsloadout.com cohort shipped 06/21–23; Bing Copilot.
Qualifier: not the literal zero the refutation implied; the predicted ordering held.
Source: STUDY-1; STUDY-2; UPDATES.

**A3 · VALIDATED-INTERVENTION (demand-confounded by design)** — Ride date-shaped
demand events: regenerate surfaces the day demand arrives; ship the event page
day-zero.
Receipt: TFL's Season-11 regeneration (07/08–09): 327 citations/day → 925/day; peak
day 1,870 (2× prior best); the /season-11 page became the site's #2 page (2,897
citations) in ~5 days; 63.43% share on "the finals season 11 release date".
Qualifier (verbatim from the memo): "the data cannot separate 'fresh supply' from
'new demand,' and doesn't need to."
Scope: thefinalsloadout.com, Bing Copilot, 06/30–07/13.
Source: UPDATES.

**A4 · PREDICTED-AND-SCORED** — A programmatic template on demand-qualified entities
keeps compounding with zero further template changes.
Receipt: prediction registered 07/13 ("Merit reaches ≥100 cited pages in one day by
the first August pull") HIT three weeks early — 127 cited pages on 07/13 (plus a
669-citation day, both site records); +95% citations in 13 days with no citation-side
template change; 255 template URLs cited by 07/15. Cited-template yield had already
climbed 10%→17% across earlier snapshots.
Scope: meritplaybook.com, Bing Copilot.
Source: UPDATES; STUDY-2.

**A5 · NEGATIVE-RESULT + PREDICTED-AND-SCORED** — Probe demand before building
supply: check which grounding queries a site already appears for; if the topics show
no grounding demand, more pages earn nothing.
Receipt: ailooplibrary.com — purpose-built GEO subpages (shipped 06/30) earned 0
citations; all 28 site citations belong to the homepage; the only grounding query is
navigational. Prediction "stays under 10/day until demand exists" HOLDS (2.5/day).
Corollary (kill-rule, untestable by construction): you cannot manufacture demand for
a coined term — demand for an invented term is zero by definition.
Scope: ailooplibrary.com, Bing Copilot, 07/03–13.
Source: UPDATES.

**A6 · OBSERVED-CORRELATIONAL** — Demand pools shift and ride-along demand fades:
segment brand-event demand out of trend reads, and re-check which cluster to densify
each quarter.
Receipt: Merit's #1 page (an explainer on a competitor platform's shutdown) went
109→578 citations; demand-side mentions are fading with the event (56→28 monthly)
even while Bing citations kept climbing in-window (578→1,046) — two instruments,
segment them. TFL's "meta" query cluster modeled −60% YoY while "loadouts" held flat
— and /loadouts was the best new page at study time.
Scope: meritplaybook.com, thefinalsloadout.com; modeled-volume caveat applies (G11).
Source: STUDY-2; UPDATES.

**A7 · OBSERVED-CORRELATIONAL (two datasets)** — Head terms belong to aggregators;
enter through the tail. Reddit, YouTube, and Wikipedia ranked #1 in all 36 head-term
citation leaderboards measured; several tail top-10 cutoffs sat at 1–9 mentions —
single digits get you in. Cross-vertical corroboration: mortgage citation leaderboards
are dominated by government (HUD.gov, va.gov), national editorial (Bankrate,
NerdWallet), YouTube, and Reddit; 11 named working loan officers appeared zero times.
Scope: LLM-mentions leaderboards (owned-site verticals, 06/2026); mortgage archive
(760,099 Google AIO + 61,686 ChatGPT citations, 3 topics, 06–07/2026).
Source: FINDINGS-era pulls; MORTGAGE.

**A8 · OBSERVED-CORRELATIONAL** — Densify existing winners before building new pages:
the sites captured only ~22–26% of the citation pools they already appear in
(implied-pool capture: HW 22.4%, Merit 26.3%, TFL 22.0%; one query alone left ~1,990
citations unclaimed).
Scope: 3 sites, Bing grounding-query data (partial instrument — see G3).
Source: STUDY-1.

## B. Content & page architecture

**B1 · OBSERVED-CORRELATIONAL (explicitly inferential)** — Put an answer-first block
(40–70 words, plain declarative sentences, named entities and numbers) at the top of
the rendered DOM.
Receipt: present on 100% of the 11 highest-citation templates and absent on the
same-template weakly-cited control page (14 citations, identical domain/links/schema).
Presence verified; causation not — the studies' own tag is [INFERENTIAL].
Scope: thefinalsloadout.com same-template comparison; Bing Copilot.
Source: STUDY-1.

**B2 · OBSERVED-CORRELATIONAL (controlled template)** — On demand-qualified pages,
add structured liftable units (stat blocks, lists, FAQs); never pad length.
Receipt: structured-richness odds ratio 1.49 per SD (p=0.017) — small and real; word
count OR 1.09 (n.s.); within the high-demand stratum the cited rate FALLS with depth
(58.3%→45.8%→36.0%); 84% of the 167 deepest pages earned nothing.
Scope: meritplaybook.com 751-page template.
Source: STUDY-1; STUDY-2 (the replication resolved its own "undetermined" richness
verdict in favor of the controlled regression).

**B3 · FALSIFIED-AS-UNIVERSAL** — "Add FAQs / tables / quick answers / question-shaped
H2s to get cited" is false as stated: these are floors that keep a page eligible, not
levers that select it.
Receipt: UNCITED pages score HIGHER on nearly every craft feature (quick-answer 99.0%
vs 65.6%; tables 94.9% vs 58.3%; FAQ schema 95.9% vs 66.3%; source links 97.5% vs
81.6% — 712 uncited vs 163 cited pages). 0% of the 11 highest-citation templates use
question-shaped H2s. TFL's top-3 pages (~90% of its citations) carry FAQPage JSON-LD
with no visible matching Q&A (a post-06/21 observation — the same pages carried zero
JSON-LD before then; see C1).
Qualifier: the data cannot rule out a small positive effect — only that the features
are not necessary and do not discriminate.
Scope: 3 sites, Bing Copilot.
Source: STUDY-1; STUDY-2.

**B4 · OBSERVED-CORRELATIONAL (third-party + own-site)** — For programmatic Q&A: one
page per one specific question; never bundle — but only against demand that exists
(A2 governs when fragmentation is wrong).
Receipt: CollegeVine earns ~14,000 ChatGPT mentions almost entirely via 56 cited
single-question FAQ pages (reverse-engineered from public citation patterns); Merit's
top ChatGPT page follows the same one-question shape. The apparent tension with A2
resolves on demand shape: single-question pages win where the grounding queries ARE
single questions.
Scope: CollegeVine (external), meritplaybook.com; LLM-mentions data, 06/2026.
Source: FINDINGS-era pulls.

**B5 · OBSERVED-CORRELATIONAL (probe-backed, thin)** — Comparison and alternatives
pages ("x vs y", "x alternatives") force retrieval on chat engines — the model cannot
answer them from memory. Single-run probe evidence; treat as directional (G6).
Source: STUDY-1/STUDY-2 probes.

**B6 · OBSERVED-CORRELATIONAL** — New aggregate hubs convert to cited status in days;
expect power-law concentration (a few pages carry most volume) with the top share
diluting fast as the tail grows.
Receipt: /loadouts +664 citations in-window, class hubs zero→cited; TFL's top page
fell from 78.5% to 54.9% of page-counter citations in 13 days; portfolio top-page
share 50.5%→~36%; HW's cited-URL set stayed identical (18 URLs) while page-counter
volume grew +46% — re-use deepening, not new coverage.
Scope: TFL, HW, portfolio; Bing Copilot, 07/01–14.
Source: UPDATES.

## C. Schema & entity binding

**C1 · FALSIFIED-AS-UNIVERSAL** — "Schema markup is required to earn AI citations" is
false. Pairing guard: only volume earned while a page had no schema may support the
claim.
Receipt: TFL's /meta-weapons earned 5,179 citations (June study time; 6,000+ by the
frozen public claim at PLAYBOOK) with zero JSON-LD — schema landed only on 06/21, so
later volume (8,136 total by 07/15) may NOT be attributed to the no-schema condition.
Sitewide, uncited pages carry MORE schema than cited pages; Merit runs the richest
schema vocabulary of the three sites and earns mid-pack.
Scope: 3 sites, Bing Copilot. The studies' red team labeled this "weakened," not
refuted — topic-confounded. Ship schema for hygiene; don't credit it (→ C2).
Source: STUDY-1; STUDY-2; UPDATES; PLAYBOOK.

**C2 · STANDARD-UNTESTED** — Ship schema anyway: QAPage for single-question pages,
FAQPage only for real multi-Q&A, Organization + sameAs sitewide, domain types
(VideoGame etc.) for disambiguation. Untested as a citation lever here (a within-site
schema A/B at n=19 per arm was killed as statistically underpowered); justified by
rich-result eligibility and C3.
Source: STUDY-1.

**C3 · OBSERVED-CORRELATIONAL** — Disambiguate or die on colliding names: when your
entity shares a name with a bigger meaning, bind the entity explicitly (schema +
copy) or skip the topic.
Receipt: "The Finals" (video game) is ~34% contaminated by NBA Finals coverage in
response-text mention data; at the brand-entity layer the same ambiguity surfaces
differently: the top brands in the site's own "meta" slice are Louisville Slugger
"Meta" baseball bats and VALORANT esports entities — two instruments, one collision.
The site's twelve-month zero in one major mention corpus has the unshipped entity
binding as its standing prime suspect [INFERENCE].
Scope: thefinalsloadout.com; heritagewhisper.com phrase collisions.
Source: FINDINGS.

**C4 · OBSERVED-CORRELATIONAL (pilot)** — For people and local businesses, AI
visibility = can engines find you, resolve you to the right individual, and describe
you accurately. Audit identity consistency across platforms before optimizing content.
Receipt: 76 buyer-language prompts × 5 engines → 354 answers; baseline mean engine
hit rate 20% for one subject; 17 online assets across 12 platform types → 8
inconsistencies found.
Scope: one anonymized mortgage-professional case + pilot battery; treat as method +
baseline, not a validated rule.
Source: LOCAL-PRO.

## D. Rendering & technical access

**D1 · FALSIFIED-AS-UNIVERSAL (with an explicit self-correction)** — "SSR/static HTML
is required for AI citation" is false — and the studies' own "fetcher-readable
structure is the price of admission" framing was itself downgraded on review:
retrieval/index presence is the gate; structure's value is removing dependence on any
single engine's renderer and shaping what gets quoted.
Receipt: the portfolio's biggest page was 100% client-rendered JavaScript (0 of 38
weapon names in its static HTML) through ~85% of its citation volume; Bing renders JS;
Perplexity cited it at position 1 and ChatGPT quoted its rendered stats before/at the
moment a structural retrofit landed. The retrofit produced no visible step-change in
citation pace (~71→~105→~85/day, noisy). That GPTBot/PerplexityBot/ClaudeBot don't
render JS is behavior-inferred, not documented.
Scope: thefinalsloadout.com; multi-engine.
Source: STUDY-2 (incl. its post-comparison addendum); STUDY-1 live probes.

**D2 · NEGATIVE-RESULT** — SSR alone does not create citations. Shipping static
render did not move a zero.
Receipt: TFL shipped its static-render fix on 06/21 (noscript data table + answer
block + JSON-LD in served HTML); Google AI Overviews — whose corpus carries
current-month data — still read zero 3.5 weeks later. The render-gap hypothesis alone
no longer explains the zero.
Scope: thefinalsloadout.com, Google AIO mention corpus.
Source: FINDINGS.

**D3 · NEGATIVE-RESULT (confound stated)** — A wave of AEO technical fixes (visible
FAQ, IndexNow, authority page) did not bend the curve in a memory-answerable,
demand-limited niche.
Receipt: HW's 06/20–23 wave: 28.1 citations/day (14 days before) → 30.8/day (21 days
after), +10%. Guard: a rising "share of citations since X shipped" (38% for HW) "is
not evidence the changes worked" — flat rates accumulate mechanically (→ G8).
Qualifier: a declining demand pool is a plausible offsetting confound; "zero effect"
is NOT claimed.
Scope: heritagewhisper.com, Bing Copilot.
Source: UPDATES.

**D4 · OBSERVED-CORRELATIONAL** — Ship GEO fundamentals from day zero (crawlable
pages, sitemap, robots, IndexNow); onset can be days, not months.
Receipt: ailooplibrary.com — repo created 06/29, fundamentals 06/30, citations
visible 07/03 (≤3–4 day onset, left-censored) vs HW's 64-day first-citation lag
without IndexNow. Time-to-first-citation spread across sites: 0 / 10 / 64 days.
Qualifier: IndexNow attribution is INFERENTIAL — publish-event pings are confounded
with site and topic; IndexNow's fan-out reaches the Bing/Yandex ecosystem only.
Scope: 4 sites, Bing Copilot.
Source: UPDATES; STUDY-1.

**D5 · STANDARD-UNTESTED (explicitly untestable here)** — llms.txt and AI-crawler
allowlists: keep them as hygiene; expect nothing measurable. Constants across a
portfolio can't explain variance ("absence-of-lever ≠ tested-null"); only ~3% of
cited pages had a page-level llms.txt entry; by the second study all three sites
shipped an llms.txt and the most polished belonged to the site with zero live
chat-engine citations.
Scope: 3-site portfolio (n too small; feature constant).
Source: STUDY-1; STUDY-2.

**D6 · STANDARD-UNTESTED (consensus-confirmed)** — Crawlability is a prerequisite,
not a differentiator; sitemap priority does nothing (a priority-0.9 page earned zero
citations).
Source: STUDY-1.

## E. Host & URL hygiene

**E1 · OBSERVED-CORRELATIONAL (verified split; fix instrumented)** — One canonical
host. A www/apex split dilutes citation identity and misjoins analysis.
Receipt: 7 of 22 of HW's ChatGPT mentions (31.8%) sat on the www host
(blind-verified); default corpus queries count apex-only, so the split also
undercounts measurement. Live www already 308-redirects to apex — the remaining www
mentions are engine-side URL memory; the subdomain-vs-apex diff decaying to zero is
the named verification instrument for the fix.
Scope: heritagewhisper.com; ChatGPT mention corpus.
Source: FINDINGS.

**E2 · OBSERVED-CORRELATIONAL (single case)** — Never publish two URLs answering the
same question: one HW page existed on both hosts and split its citations into
single-citation fragments.
Source: FINDINGS-era pulls.

**E3 · OBSERVED-CORRELATIONAL (small)** — Retired URLs keep earning: a dissolved page
301'd for two weeks still drew citations — engines remember URLs. Plan redirects;
don't assume retirement stops citation flow.
Scope: paultakisaki.com.
Source: UPDATES.

## F. Platform targeting & engine divergence

**F1 · OBSERVED-CORRELATIONAL + published framework** — The Two-Camp Engine Model:
the Google camp (AI Overviews, Gemini) reads Google's walled garden (Business
Profiles, reviews, YouTube); the open-web camp (ChatGPT, Perplexity, Claude) reads
open-web indexes (Bing's; Claude rides Brave Search), Reddit, directories, and public
sites. Optimize the camps separately; wins don't transfer.
Receipt: cross-camp top-10 domain overlap on the same three mortgage topics: 4/10,
3/10, 6/10. The framework is interpretive; the overlap counts are measured.
Scope: mortgage vertical archive (820K+ citations), 07/2026.
Source: TWO-CAMP.

**F2 · OBSERVED-CORRELATIONAL (single wave — the registered re-probe is open)** —
Bing's cited/uncited list does not predict chat-engine behavior; for one site it
approached an inverse.
Receipt: all four of ChatGPT's Merit citations (Santa Clara p5, Fordham p10, Loyola
Marymount p7, Alabama p5) were pages with ZERO Bing citations; Ole Miss — Merit's
heaviest Bing college page (201 at study-1 → 250 by 07/01; 477 by 07/13), cleanly
indexed — was cited by neither chat engine. Santa Clara was cross-validated by
Perplexity (p4). The studies' own verdict: if this holds on the registered re-probe
it is "the single most publishable finding either study produced; if it churns... it
was noise."
Scope: meritplaybook.com, wave-1 probe only (06/20–21).
Source: STUDY-1; STUDY-2; UPDATES.

**F3 · OBSERVED-CORRELATIONAL (direction replicated across 2 waves)** — Engines often
never search: on memory-answerable topics, citation is structurally impossible
regardless of page quality. Publish what parametric memory cannot answer — current
prices, comparisons, news, original first-party data.
Receipt: wave 2: 14 of 48 engine-cells never searched; search rates ChatGPT 6/12,
Claude 8/12, Gemini 8/12, Perplexity 12/12. All four memoir-niche queries drew memory
answers from ChatGPT, Claude, AND Gemini independently. HW holds the portfolio's most
citation-dense pages per-URL (80.8/page) yet drew zero live chat-engine citations in
wave 2. The lever is editorial, not structural.
Scope: 4 engines, 2 waves, single runs per cell — exact fractions indicative (G6).
Source: STUDY-2.

**F4 · OBSERVED-CORRELATIONAL** — Mention ≠ link ≠ click; conversion differs by
engine. Google AIO cites ~100% of its mentions (the lever there is breadth of
indexable coverage); ChatGPT linked 18 of 80 brand mentions (22.5%, mention-index
denominator); on the retrieval side its backend retrieved the same site 66 times and
cited 18 (27%). Normalize per-engine before comparing wins: average citations per
answer ran ChatGPT 2.1 / Claude 3.3 / Gemini 5.8 / Perplexity 8.4.
Scope: LLM-mentions pulls + wave-2 probe, meritplaybook.com.
Source: FINDINGS-era pulls; STUDY-2.

**F5 · OBSERVED-CORRELATIONAL (single observation)** — Stale model memory shapes
retrieval queries; whoever ranks for the stale phrasing wins the citation. ChatGPT
fanned out "Season 7" queries when the live game was on Season 10; the domain ranking
for the stale query took the citation despite fresher data existing elsewhere.
Scope: thefinalsloadout.com, ChatGPT fan-out, wave 2.
Source: STUDY-2.

**F6 · INSTRUMENT-RULE** — Gemini cannot be measured first-party (its citations
resolve to Google's vertexaisearch grounding proxy, not source URLs); serve AI
Overviews well and treat Gemini as covered indirectly.
Source: FINDINGS-era pulls.

## G. Measurement & instrumentation (the harness spine)

**G1 · PREDICTED-AND-SCORED (the method that powers this book)** — Register
falsifiable predictions before data arrives; score them publicly. This is the
cheapest way an observational dataset gets causal teeth.
Ledger to date: (1) TFL settles at 250–500/day post-event → HOLDS in direction, band
edge (ran hot at 589/day). (2) Merit ≥100 cited pages in a day by August → HIT three
weeks early (127 on 07/13). (3) HW stays 25–50/day → HOLDS, watch (53.1/day averaged
over 7/07–13, nudged above band by a single-day record of 84). (4) ailooplibrary
under 10/day until demand exists → HOLDS (2.5/day). (5) June fragmentation call →
scored ~17× (A2). (6) The Bing-inverse re-probe (F2) → registered, still unscored.
Source: UPDATES; STUDY-2.

**G2 · OBSERVED-CORRELATIONAL (robust across pulls)** — Citations ≠ clicks: ~112:1
portfolio-wide (11,609 citations vs 104 AI-referral sessions in one 13-day window).
One site ran ~460 in-window citations against zero copilot.com sessions and exactly
one chatgpt.com session. Treat citations as brand exposure until click-through is
instrumented per engine. Clicks concentrate on interactive tools, not cited flagships
(53% of TFL's AI sessions land on an interactive tracker holding 5.4% of its
citations; the #1 cited Merit page got zero landings). The engine counting your
citations is not the engine sending clicks (ChatGPT out-referred Copilot). Referral
rate rises with citations directionally, at roughly 1/150th scale.
Scope: TFL/Merit/HW, GA4 vs Bing, through 07/13.
Source: UPDATES; STUDY-2.

**G3 · INSTRUMENT-RULE (Bing Webmaster export mechanics)** — (a) The tail 1–2 days of
any daily export restate upward — treat them as floors. (b) The three export types
(daily series / page counters / grounding queries) do not reconcile by construction;
the gap can be structural, site-specific, and growing (one site: 32%→~35% across
pulls; others ~1–3%) — state totals as ranges where gaps exist. (c) The query export
is partial and thresholded — coverage ran 11–42% of page totals at one pull and
15–43% at another; partial AND drifting, directional only. (d) Window anchors shift
between pulls; verify key events fall inside both windows; never compare cross-site
daily totals on different window lengths. (e) Bing splits URLs across www/apex —
canonicalize hosts before joining. (f) Export filename date stamps lie; parse the
data's actual tail. (g) Parse dates — never string-sort them (a lexicographic sort
produced a wrong analysis window that survived two analysts before an adversarial
verifier caught it).
Source: STUDY-1; STUDY-2; UPDATES.

**G4 · INSTRUMENT-RULE (third-party LLM-mention indexes)** — (a) ChatGPT corpora are
batch-ingested roughly monthly with a ≥2-week lag — read monthly, one month in
arrears. (b) Small domains may have no usable pre-history. (c) Keyword targets can be
word-bag matched — phrase-level claims are invalid (one series showed 4,257 mentions
for a product season before that season existed). (d) Raw counts are
corpus-growth-dominated (a ~10–20× uniform rise across unrelated topics) — only
share/ratio metrics are interpretable across time. (e) New/Lost deltas measure
sampling churn for small targets — a presence tripwire, not a decay meter. (f) Brand
endpoints may AND-match multi-keyword targets — one keyword per request. (g) Coverage
gaps are real: a site can be #1 on first-party volume and absent from the corpus
entirely — check coverage before making site claims. (h) Same-day reruns of archive
leaderboards showed only ~32–43% source overlap — never single-snapshot a leaderboard.
Source: FINDINGS (8/8 blind-verified); MORTGAGE (methodology note).

**G5 · INSTRUMENT-RULE** — Non-stationary series break naive before/after analysis:
one site booked 87.6% of its all-time citations in the final 30 days of a study
window; a historical-baseline pre/post test was red-team REFUTED on this basis.
Ramp-phase data needs registered predictions and controls, not baselines.
Source: STUDY-1.

**G6 · INSTRUMENT-RULE** — Single-run live probes are weather, not climate. Results
churned between waves (one site went 1/6 cited cells → 0/48); search-triggering is
stochastic and prompt/version-sensitive. Re-run at least 3× before citing rates;
treat direction as the finding.
Source: STUDY-2.

**G7 · INSTRUMENT-RULE** — GA4 AI-referral measurement: pull the full sessionSource
list and identify AI sources from it — pre-filtering by an assumed list missed
copilot.com and undercounted AI sessions ~46% on one site. Check each property's
first-data date before any window comparison. A single user can masquerade as an
engine trend (37 "gemini" sessions traced to one reader).
Source: UPDATES; STUDY-2.

**G8 · INSTRUMENT-RULE** — The mechanical-accumulation fallacy: "N% of our citations
arrived since X shipped" is what a flat rate produces over time; never present it as
effect evidence. It will be the most tempting false claim in any GEO report you write.
Source: UPDATES.

**G9 · INSTRUMENT-RULE (method)** — The author never verifies their own claims;
cross-validate analysis with a second independent system and resolve disagreements
against raw data. Track record behind this book: the first study triangulated three
independent analysts; a fresh-context blind verifier confirmed 8/8 headline numbers
of the mentions pull; adversarial verification caught a string-sort window bug,
blank-row inflation, and a GA4 undercount; and this rulebook itself went through a
three-verifier decorrelated pass that corrected 19 items before release.
Source: STUDY-1; STUDY-2; FINDINGS; this document's Methods.

**G10 · INSTRUMENT-RULE** — Coverage and process gaps hide real activity: one site
had been earning citations for 2.5 months before anyone noticed — it had simply never
been pulled. Enumerate properties before concluding absence. "Top page" claims go
stale within days — re-verify leaders before publishing.
Source: UPDATES; STUDY-2.

**G11 · INSTRUMENT-RULE** — Demand instruments are non-substitutable: grounding-query
implied pools count one engine's retrieval events; modeled AI-keyword volume
estimates chat-assistant demand (the same term measured ≈3,157 vs 27). Winning
long-tail queries often show NO modeled volume while carrying real grounding pools —
the long tail shows up in grounding data before keyword tools see it.
Source: STUDY-2.

## H. What this evidence does NOT support

- **Causal claims beyond the tagged interventions and predictions.** The core
  datasets are observational, N=1 per cell, demand-confounded throughout — the
  studies' own red-team language. The demand gate is "the only thing the data lets
  you bet on hard."
- **Transfer beyond the tested surface.** Bing Copilot dominates the first-party
  counts; chat-engine behavior is probe-thin; the verticals are gaming, education,
  memoir, personal brand, plus one mortgage archive study. US/English only.
- **The procedural-framing rule** ("how-to phrasing triggers retrieval") — one
  observation for, one against; do not ship it without re-testing.
- **The "be specific where authorities are vague" principle and "niche retrieval-fit
  beats domain authority"** — explicit HYPOTHESES; no authority/backlink data exists
  in the corpus to confirm either.
- **The Bing-inverse map as established fact** (F2) — single wave; the registered
  re-probe is unscored.
- **llms.txt effects in either direction** (constant across the portfolio —
  untestable).
- **IndexNow as the isolated cause of onset speed** (confounded; suggestive timing
  only).
- **Month-over-month raw counts from mention indexes**, phrase claims from word-bag
  keyword series, or New/Lost deltas as decay measurements (G4).
- **Depth/word count as a lever** — actively contradicted (B2). "Publish more pages"
  as a default strategy — contradicted by the headroom data (A8).

## Methods & verification

The first-party dataset is Bing Webmaster AI-citation exports (daily series, page
counters, grounding queries) across six owned sites, reconciled across pulls with
zero mismatches on 378 overlapping site-days, joined to codebase forensics
(commit-dated interventions) and GA4 referral data. Two full studies were run by
independent analyst systems three weeks apart and converged; disagreements were
resolved against raw data and are documented, including the studies' own downgraded
claims. Third-party corpora (LLM-mention archives) are used with the instrument
limits in G4, several of which were discovered by registering expectations before
pulling. Live-probe waves are single-run and treated as directional only.

This rulebook's own adjudication was checked by three independent fresh-context
reviewers against primary sources before release; 19 corrections were applied in
that pass, and three initially-flagged sub-claims were subsequently re-verified
against their primary sources. Predictions are registered before data arrives and
scored publicly in later editions (G1).

Headline stats and ongoing updates: PLAYBOOK. Vertical archive methodology: MORTGAGE.
Framework: TWO-CAMP. Entity-probe pilot: LOCAL-PRO.
