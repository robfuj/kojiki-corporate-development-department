# 18 — Corporate Development

> Part of the **Hermes Organizational Decision System**. This repo is the
> **Corporate Development** line. It references the shared ontology in
> [`00-kojiki-ontology`](https://github.com/hermes-ios/00-kojiki-ontology) for the
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

## How to use
1. Read `AGENT.md` — the first-run Orientation Protocol.
2. Read `SCHEMA.md` — how this line maps to the universal schema.
3. Read `data/18-corporate-development.json` — the machine-readable spec.
4. See `data/example.json` — one fully worked decision (Decision Object + Ledger).
5. Use `decision-graph.mmd` — agent-decodable operating tree + state model.
6. Validate new records: `python3 tools/validate.py data/<name>.json`
