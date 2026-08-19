# 18 — Corporate Development

> Part of the **Kojiki Decision System**. This repo is the
> **Corporate Development** line. It references the shared ontology in
> [`00-kojiki-ontology`](https://github.com/robfuj/kojiki-ontology) for the
> canonical schemas, taxonomy, decision-rights, and handoff standards.

## Primary question
> What should we acquire, invest in, or integrate?

## Purpose
Evaluate external assets and transactions against alternative uses of capital and capability.

## Sub-functions
M&A, Investments, Corporate Ventures, Strategic Transactions, Target Intelligence, Due Diligence, Integration

## Typical roles
Chief Corporate Development Officer, VP Corporate Development, Corp Dev Director, M&A Director, Investment Manager, Integration Director

## Inputs
Targets, financials, strategic thesis, diligence, valuation, integration requirements.

## Outputs
Investment theses, diligence findings, transaction decisions, integration plans.

## Learning focus
Acquisition patterns; valuation accuracy; diligence signals; integration failures; synergy realization.

## Operating tree
```text
STRATEGIC NEED →
    TARGET UNIVERSE →
    SCREENING →
    STRATEGIC FIT →
    FINANCIAL FIT →
    OPERATIONAL FIT →
    TECHNOLOGY →
    DUE DILIGENCE →
    VALUATION →
    STRUCTURE →
    NEGOTIATION →
    CLOSE / WALK →
    INTEGRATION →
    VALUE REALIZATION →
    POST-DEAL LEARNING
```

## Decision states
```text
NEED-SET → SCREENING → FIT-TESTED → DILIGENCING → VALUING → STRUCTURING → NEGOTIATING → CLOSING → INTEGRATING → REALIZING → WALKED
```

## Decision outputs
`Pursue · Investigate · LOI · Negotiate · Acquire · Invest · Walk · Divest`

## Critical prompts (what this function thinks about)
> Why do we need this asset?
> Why this company?
> What strategic capability does it provide?
> Can we build it ourselves?
> Can we partner instead?
> What is the financial case?
> What is the downside?
> What are we assuming?
> What does diligence need to prove?
> What could invalidate the thesis?
> What is the target actually worth?
> What is our maximum price?
> What structure reduces risk?
> What happens after acquisition?
> Can we actually integrate it?
> What synergies are real?
> Who owns integration?
> Did we create the expected value?
> What did we learn?

## Canonical record schema (docx Learning Ledger + Decision Object Fields)
Every decision in this line is recorded as:
- a **Decision Object** (docx S9) — see `schema/decision-object.json`
- a **Learning Ledger** entry (docx S7) — see `schema/learning-ledger.json`

and the agent must run the **Orientation Protocol** first (see `AGENT.md`).

## How this line runs on SYNAPSIS (the cognitive substrate)
Every decision in this line is decomposed through the shared SYNAPSIS transformation
chain ([`00-kojiki-ontology/synapsis`](https://github.com/robfuj/kojiki-ontology/synapsis)):
```
SOURCE → RECORD → EVIDENCE → INTERPRETATION → STRATEGY → INTERACTION → OUTPUT → OUTCOME → LEARNING
```
- **Three steps are dedicated niche bots**: `bots/evidence/` (this line's extraction
  specialist); the shared `synapsis/audit-bot/` (independent audit, org-wide) and
  `synapsis/learning-bot/` (cross-line memory). See `AGENT.md` for the full contract.
- The rest run inline inside this line's agent, each bounded to one authority.
- Meta-rule: *evidence ≠ interpretation ≠ belief ≠ doctrine.* Validate with
  `python3 synapsis/validate.py <record.json>` (in the ontology repo).

## How to use
1. Read `AGENT.md` — the first-run Orientation Protocol.
2. Read `SCHEMA.md` — how this line maps to the universal schema.
3. Read `data/18-corporate-development.json` — the machine-readable spec.
4. See `data/example.json` — one fully worked decision (Decision Object + Ledger).
5. Use `decision-graph.mmd` — agent-decodable operating tree + state model.
6. Validate new records: `python3 tools/validate.py data/<name>.json`
