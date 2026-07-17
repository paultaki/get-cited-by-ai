---
name: get-cited-by-ai
description: Use when someone wants their site, brand, or content cited by AI search engines (ChatGPT, Perplexity, Google AI Overviews, Copilot/Bing, Gemini, Claude), asks about GEO / AEO / AI SEO / LLM visibility, asks whether schema, SSR, llms.txt, or FAQ headings will get them cited, wants an AI-citation audit, or wants to measure AI citations or AI-referral traffic.
---

# Get Cited by AI: citation optimization that starts from measured data

## Overview

Every recommendation this skill produces traces to an evidence-tagged rule in
RULEBOOK.md: a rulebook derived from 26,767 measured AI citations, a 751-page
same-template controlled regression, and a scored-predictions ledger. The core
finding, converged on by two independently-run analyses (including an adversarial
verification pass) of the same portfolio:

**Demand selects citations. Craft is a floor, not a lever.**
(RULEBOOK A1: demand odds ratio 4.42, p=0.003; word count 1.09, not significant.
Uncited pages score HIGHER on FAQs, tables, and schema than cited ones, B3.)

**Violating the letter of this workflow is violating its spirit.** The workflow order
exists because untrained agents reliably skip step 1 and prescribe craft.

## The Iron Rule

**NO recommendation before a demand probe.** Not for "quick checklists," not under
time pressure, not when the user asks specifically about schema. If the user's niche
has no grounding demand (or engines answer it from memory without searching),
citation is structurally impossible and every craft-hour is wasted (A5, F3). Run
`modules/demand-probe.md` first, or state exactly what inputs you still need to run it.

## Workflow

1. **Demand probe**: `modules/demand-probe.md`. Establish: does grounding demand
   exist, what shape is it (aggregate vs entity), and do engines actually search this
   niche or answer from memory? Output gates everything downstream.
2. **Engine split**: which camp is the target? Google camp (AI Overviews, Gemini)
   vs open-web camp (ChatGPT, Perplexity, Claude) vs Copilot/Bing. Wins do not
   transfer (F1, F2). State the target camp before recommending.
3. **Site audit**: `modules/site-audit.md`. Floors vs levers, every finding tagged.
4. **Entity check**: `modules/entity-probe.md` when the subject is a person, local
   business, or a name that collides with a bigger meaning (C3, C4).
5. **Competitive read**: `modules/vertical-leaderboard.md` when the user asks "who
   wins in my space" or picks build targets.
6. **Measurement + registered prediction**: `modules/measurement-harness.md`. Every
   engagement ends here: free instruments configured, a dated prediction with a
   refutation condition registered. No exceptions: advice without a measurement plan
   is folklore with confidence.

## Evidence-tag discipline

Every recommendation you emit cites its rule ID and tag, e.g. "(A2,
PREDICTED-AND-SCORED)". If the honest tag is STANDARD-UNTESTED, say "hygiene,
untested as a citation lever." Never present it as a lever. If no rule covers a
claim you want to make, label it SPECULATION or drop it.

## Rationalization table (observed in baseline testing, do not repeat)

| Baseline claim | Reality (rule) |
|---|---|
| "Schema/JSON-LD is the highest-leverage task" | Biggest page in dataset: 5,179+ citations, zero JSON-LD; uncited pages carry MORE schema (C1, B3) |
| "AI crawlers can't read JS — hard blocker" | Bing renders JS; the top page was 100% client-JS through ~85% of its volume; per-engine renderer dependence, structure = insurance (D1) |
| "Rewrite headings as questions; add FAQs" | 0% of the highest-citation templates use question H2s; uncited pages have MORE FAQs (B3) |
| "llms.txt is an edge / no downside" | Untestable constant; most polished one belonged to zero-live-citation site; hygiene only (D5) |
| "SSR fixed it" / "ship SSR to get cited" | SSR shipped on a zero-citation site; still zero 3.5 weeks later (D2) |
| "Measure via referral traffic" | Citations:clicks ≈ 112:1; wrong instrument: use Bing Webmaster AI reports (G2) |
| "Probe queries once now, once next month" | Single-run probes are weather; re-run ≥3× (G6) |
| "N% of citations came after our change" | Mechanical accumulation, not effect (G8) |
| "Freshness is a measurable citation factor" | No such finding in the dataset, untested |
| "Cited rate falls as pages get more structured" | Depth ≠ structure. The falling tertiles (58→46→36%) are WORD-COUNT depth; structured liftable units are the one small POSITIVE effect (OR 1.49/SD). Never conflate the two (B2) |
| "Publish more pages" | Sites captured ~22-26% of pools they're already in; densify winners first (A8) |

## Red flags: STOP and return to step 1

- You are writing craft recommendations and no demand probe has run
- You are prioritizing schema, llms.txt, or heading rewrites as impact items
- Your measurement plan has no registered prediction or uses analytics referrals
- You promised citations from any intervention ("this will get you cited")
- The user's niche looks memory-answerable and you haven't said so

## Free path first

Default instruments cost nothing: Bing Webmaster Tools AI Performance exports,
manual engine probes, page fetches. Paid data (DataForSEO LLM-mentions) is optional
bring-your-own-key and gated behind `modules/vertical-leaderboard.md`. Never make a
paid tool a prerequisite.

## Honest limits

The evidence base is n=6 sites in five verticals plus one 820K-citation vertical
archive study, Bing-Copilot-heavy, US/English (RULEBOOK "Scope discipline" and §H).
This skill inherits those limits: it tells users what was measured, not what is
universal, and its measurement harness is how they validate rules on their own site.
