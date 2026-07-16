# Site Audit — Step 3

Runs only after `modules/demand-probe.md` returns a DEMAND VERDICT of "demand
exists" and step 2 names the target camp. Craft is a floor, not a lever (Iron
Rule; A1) — this module audits hygiene and applies the few things with
evidence; it never re-opens the demand question.

## 1. Floors — check and fix; never promise as levers

1. Crawlability for AI bots: robots.txt allows GPTBot/PerplexityBot/ClaudeBot/
   Bingbot, sitemap current. Prerequisite only — a priority-0.9 sitemap entry
   still earned zero citations (D6).
2. Content present per the target camp's fetch behavior: confirm answer text
   exists in served-or-rendered HTML for that camp's fetcher. Bing renders JS
   and cited a 100%-client-JS page at #1; non-Bing fetchers not rendering JS
   is behavior-inferred, not documented (D1) — test per engine, no blanket JS
   blocker.
3. One canonical host, no duplicate-answer URLs: a www/apex split cost one
   site 31.8% of its ChatGPT mentions and undercounts measurement (E1); two
   URLs answering the same question split citations into single-citation
   fragments (E2).
4. Redirects planned for retired URLs: a dissolved page 301'd for two weeks
   still drew citations — engines remember URLs (E3). 301, don't 404.
5. Schema shipped as hygiene, never credited: QAPage / real-FAQPage /
   Organization+sameAs for rich-result eligibility and disambiguation (C2) —
   the dataset's biggest page earned 5,179+ citations with zero JSON-LD, and
   uncited pages carry MORE schema than cited ones (C1).
6. llms.txt shipped as hygiene: expect nothing measurable — ~3% of cited
   pages had one, and the most polished portfolio example belonged to a site
   with zero live chat-engine citations (D5).
7. Day-zero fundamentals on new sites: crawlable pages, sitemap, robots,
   IndexNow from launch — onset can run days (≤3–4) instead of months (64
   without IndexNow) (D4).

## 2. Levers — the few things with evidence

1. Page shape matches demand shape: one dense aggregate hub for aggregate-
   comparative demand, never fragmented into per-entity pages. The strongest
   rule in this book — hubs ran ~17× the per-page rate of fragments (A2,
   PREDICTED-AND-SCORED).
2. Answer-first block, 40–70 words, plain declarative sentences, named
   entities and numbers, top of the rendered DOM. Present on 100% of the 11
   highest-citation templates, absent on a weak same-template control (B1,
   inferential — presence verified, causation not).
3. Structured liftable units on demand-qualified pages only, never as
   length-padding: small real effect (OR 1.49/SD); within the high-demand
   stratum cited rate FALLS as depth increases (B2).
4. Day-zero event pages for date-shaped demand: ship the page the day demand
   arrives (A3, VALIDATED-INTERVENTION, demand-confounded by design).
5. Densify winners before new pages: sites captured only ~22–26% of pools they
   already appear in (A8).
6. One question per page, only against real single-question demand:
   CollegeVine earns ~14,000 ChatGPT mentions from 56 single-question pages
   (B4).
7. Comparison/alternatives pages force retrieval on chat engines — thin,
   single-run evidence, directional (B5).

## 3. What NOT to recommend

- Schema/JSON-LD as the highest-leverage task (C1, B3)
- Question-shaped H2s / FAQs as levers — uncited pages score higher on both
  (B3)
- llms.txt as an edge with no downside (D5)
- Blanket "AI crawlers can't read JS" (D1)
- SSR alone as the fix — shipped on a zero-citation site, still zero 3.5
  weeks later (D2)
- Freshness as a measurable citation factor — no such finding in the dataset
- "Publish more pages" as default strategy (A8)

## Output: AUDIT REPORT

Fill `templates/audit-report.md`; every floor and lever row carries a rule ID.

```
AUDIT REPORT (see templates/audit-report.md)
- Floors: [N] pass / [N] fail / [N] fixed
- Levers recommended: [item — rule ID + tag], ...
- Explicitly NOT recommended: [item — rule ID], ...
```
