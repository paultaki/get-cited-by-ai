# get-cited-by-ai

**Get cited by AI, or find out you can't.**

I run seven sites. Bing has logged 50,000+ AI citations across them (50,072
through August 5, 2026, still adding roughly nine hundred a day), and I compared
the pages that get cited constantly against the hundreds that never get picked
once. Most of the standard advice did not survive that comparison. My
highest-citation page earned its first 5,000 citations with zero JSON-LD on
the page (the markup came later). My uncited pages have MORE schema,
tables, and FAQs than my cited ones. The most polished llms.txt in the whole
portfolio belonged to the site with zero live chat-engine citations.

This skill is what survived. It runs one honest check before anything else: is
anyone actually asking AI the questions your site could answer? If nobody is,
no amount of on-page work will get you cited, and the skill tells you so before
you spend a week on it. If they are, it sorts your fixes into floors (worth
doing, but they won't get you cited on their own) and the few levers that
actually correlate with citations. Then it gives you a free way to measure
whether any of it worked.

Built for anyone running Claude Code on their own site or a client's. This work
goes by a few names: GEO (generative engine optimization), AEO (answer engine
optimization), AI SEO. Same problem, different labels. Every recommendation
here traces to an evidence-tagged rule instead of industry folklore.

## What this is

A demand-gated workflow. Probe for grounding demand first, split by engine
camp, then audit, entity-check, and benchmark a vertical. No craft
recommendation before the demand gate. Every rule cites a measured dataset:
26,767 first-party AI citations across six owned sites, a 751-page
same-template controlled regression (observational, see RULEBOOK "Honest
limits"), an 820K-citation vertical archive study (mortgage), and a
registered-predictions ledger with scored outcomes. `RULEBOOK.md` holds the
full rule set, evidence tags, and receipts. (The rules stay pinned to that
frozen study corpus; the live counter, 50,000+ per the line up top, is a
growth update, not new evidence, until rules are re-scored. The daily series,
weekly rollup, and site/page rollups are published as CSV in `data/`, with a
claim-to-file map in `data/README.md`.)

## Why it's different

Before shipping this, I tested a capable agent without it. Three scenarios.
All three skipped the demand question and prescribed the same checklist:
schema everywhere, question-shaped H2s and FAQs, llms.txt, "ship SSR."
`tests/BASELINE-2026-07-15.md` is the receipt. My dataset falsifies most of
that checklist on the sites it was tested against. That is the reason this
skill exists.

## What's inside

- `SKILL.md`: the workflow orchestrator (six steps: demand probe, engine
  split, site audit, entity check, vertical leaderboard, measurement)
- `RULEBOOK.md`: the evidence base. Every rule, its tag, its receipt, its
  scope.
- `modules/`: procedures for five of the six steps (engine split lives in
  SKILL.md step 2): `demand-probe.md`, `site-audit.md`, `entity-probe.md`,
  `vertical-leaderboard.md`, `measurement-harness.md`
- `templates/`: `audit-report.md` and `prediction-ledger.md`, the
  fill-in-the-blank outputs
- `predictions/`: the public preregistration ledger. One file per registered
  prediction, committed before its scoring data exists, so the git timestamp
  is the receipt. Some are still open. That's the point. If a rule is wrong,
  its scored file will say so in public.
- `examples/`: a complete worked audit produced by this skill on a real
  site, including what it refused to recommend
- `tests/`: `BASELINE-2026-07-15.md`, the pre-skill failure record this
  skill was built to correct, plus the edit log (every post-release change
  traces to a documented failing check)

## Install

Clone into `~/.claude/skills/get-cited-by-ai` for use across all projects, or
into `<project>/.claude/skills/get-cited-by-ai` for a single project.

```
git clone https://github.com/paultaki/get-cited-by-ai ~/.claude/skills/get-cited-by-ai
```

## The data behind it

Four published sources back the rulebook:

- Playbook and ongoing headline stats: https://paultakisaki.com/learn/how-to-get-cited-by-ai/
- Mortgage vertical archive methodology: https://credibilityos.ai/research/mortgage-ai-citations/
- Two-Camp Engine Model: https://credibilityos.ai/research/two-camp-engine-model/
- Local-professional entity-probe pilot: https://credibilityos.ai/learn/ai-visibility-for-local-professionals/

The prediction ledger is public in `predictions/` and the portfolio's daily,
weekly, site, and page series are public as CSV in `data/`. The per-site
receipts and regression internals behind the remaining rules are unpublished;
ask if you need a cut. The sites named are real. I own and operate them.

## Honest limits

The evidence base is n=6 owned sites across five verticals (gaming, college
merit aid, memoir, AI tools, personal brand) plus one mortgage vertical
archive study. Bing Copilot-heavy, US/English. It is observational and
demand-confounded throughout. The demand gate is the one thing it lets you
bet on hard. This skill tells you what was measured on those sites, not
what's universal. Its own measurement harness is how you validate any rule
against your own site.

## License

MIT
