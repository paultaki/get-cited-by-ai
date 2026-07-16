# get-cited-by-ai

A Claude Code skill for AI-citation optimization (GEO/AEO), where every
recommendation traces to an evidence-tagged rule instead of industry
folklore.

## What this is

`get-cited-by-ai` runs a demand-gated workflow — probe for grounding demand
first, split by engine camp, then audit, entity-check, and benchmark a
vertical — before it emits a single craft recommendation. Every rule it
cites comes from a measured dataset: 26,767 first-party AI citations across
six owned sites, a 751-page controlled template experiment, an
820K-citation vertical archive study (mortgage), and a registered-
predictions ledger with scored outcomes. See `RULEBOOK.md` for the full
rule set, evidence tags, and receipts.

## Why it's different

Stock agents asked to improve AI-search visibility default to a checklist:
schema everywhere, question-shaped H2s and FAQs, llms.txt, "SSR fixed it."
`tests/BASELINE-2026-07-15.md` documents this failure directly — three
scenarios run against a capable agent with no skill loaded, all three
skipping the demand question and prescribing that checklist. The dataset
falsifies most of it: the highest-citation page carried zero JSON-LD;
uncited pages carry MORE schema, tables, and FAQs than cited ones; the most
polished llms.txt in the portfolio belonged to the site with zero live
chat-engine citations. This skill exists because that checklist is
measurably wrong on the sites it was tested against.

## What's inside

- `SKILL.md` — the workflow orchestrator (six steps: demand probe, engine
  split, site audit, entity check, vertical leaderboard, measurement)
- `RULEBOOK.md` — the evidence base: every rule, its tag, its receipt, its
  scope
- `modules/` — one procedure per workflow step: `demand-probe.md`,
  `site-audit.md`, `entity-probe.md`, `vertical-leaderboard.md`,
  `measurement-harness.md`
- `templates/` — `audit-report.md` and `prediction-ledger.md`, the
  fill-in-the-blank outputs
- `tests/BASELINE-2026-07-15.md` — the pre-skill failure record this skill
  was built to correct

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

Everything else in the rulebook — per-site receipts, the prediction ledger,
the internal studies — is unpublished; the sites named are real and
operated by the author.

## Honest limits

The evidence base is n=6 owned sites across five verticals (gaming,
college merit aid, memoir, AI tools, personal brand) plus one mortgage
vertical archive study — Bing Copilot-heavy, US/English. It is
observational and demand-confounded throughout; the demand gate is the one
thing it lets you bet on hard. This skill tells you what was measured on
those sites, not what's universal — its own measurement harness is how you
validate any rule against your own site.

## License

MIT
