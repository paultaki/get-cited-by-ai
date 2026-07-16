# Entity Probe — Step 4

Runs when the subject is a person, a local business, or a name that collides
with a bigger meaning (C3, C4). Skip for pure content sites with no personal
or local entity to resolve.

## 1. Build the buyer-language prompt battery

Draft prompts in the phrasing a real buyer would use, not brand-name lookups.
The LOCAL-PRO pilot ran 76 such prompts across 5 engines for 354 answers
(C4) — match that scale for a real read; a handful of prompts is not a
battery. The pilot's five engines: ChatGPT, Google AI Overviews, Perplexity,
Gemini, Claude (LOCAL-PRO). Add Copilot/Bing when the subject also needs the
first-party Bing citation counter (SKILL.md step 2).

## 2. Score the hit-rate baseline

Per prompt/engine cell, record whether the entity surfaces at all, and
whether it's the RIGHT entity. The pilot's baseline mean engine hit rate was
20% for one subject (C4) — a reference floor, not a target; a new subject's
baseline could sit anywhere.

## 3. Audit identity consistency across platforms

Enumerate every online asset — site, Business Profile, directories, review
platforms, socials, press — across platform types. Check name, credentials,
location, and service description for drift. The pilot found 8
inconsistencies across 17 assets spanning 12 platform types (C4); expect
real, fixable drift, not a clean baseline.

## 4. Check for name collision

Does the name (person, brand, or product) collide with a bigger meaning?
"The Finals" runs ~34% contaminated by NBA Finals coverage in mention data;
the same site's brand-entity layer collided separately with Louisville
Slugger "Meta" bats and VALORANT esports entities — two instruments, one
collision pattern (C3). Search the bare name across engines and log every
unrelated sense that surfaces.

## 5. Disambiguate or skip

If a collision is confirmed, bind the entity explicitly: schema
(Person/LocalBusiness + sameAs) plus copy that names the disambiguating
context in the first sentence (C2, C3). If binding isn't feasible, mark the
topic un-ownable rather than shipping content that will be misattributed.

## 6. Two-camp targeting for local pros

Local professionals split hard across the Two-Camp model (F1, TWO-CAMP): the
Google camp (AI Overviews, Gemini) reads Business Profiles, reviews, and
YouTube — a site alone doesn't reach it. The open-web camp (ChatGPT,
Perplexity, Claude) reads open-web indexes, Reddit, and directories —
Business Profile completeness doesn't reach it. Cross-camp top-10 domain
overlap measured 4/10, 3/10, 6/10 on the same queries (F1) — audit and build
for each camp separately.

## Scope and honest limits

C4 is a pilot on one anonymized mortgage professional — method and baseline,
not a validated rule (LOCAL-PRO). F1's overlap counts come from the mortgage
vertical archive (MORTGAGE), not a local-pro-specific dataset — apply the
framework, not the exact overlap numbers, to a new subject.

## Output: ENTITY PROBE FINDINGS

Findings feed `templates/audit-report.md` as additional rows: identity fixes
are floors; entity binding is closer to a lever, tag it OBSERVED-CORRELATIONAL
(C3), not proven.

```
ENTITY PROBE FINDINGS
- Hit rate: [N]% across [N] prompts × [N] engines (C4)
- Identity inconsistencies found: [N] across [N] assets / [N] platform types (C4)
- Name collision: yes/no — colliding sense: [what] (C3)
- Disambiguation action: bind (schema + copy) / topic marked un-ownable (C2, C3)
- Target camp for this entity: Google camp / open-web camp / both (F1)
```
