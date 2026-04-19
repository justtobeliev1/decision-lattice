# Decision Lattice

Decision Lattice is an open-source Codex skill for routing hard decisions through the right mental models.

It gives the agent a 38-model lattice and a practical routing workflow so it can decide which models to use, why they fit the current situation, and how to turn them into a recommendation.

## What It Does

- classifies a decision by stakes, reversibility, uncertainty, actor count, and system complexity
- selects a compact bundle of mental models instead of dumping all 38 on every prompt
- combines epistemic, systemic, social, and temporal lenses
- outputs a recommendation, evidence gaps, guardrails, and revisit triggers

## Best Use Cases

- strategy choices
- architecture or product bets
- roadmap prioritization
- hiring and org design
- market and competitive analysis
- planning under uncertainty
- risk review and pre-mortem work

## Repository Layout

```text
decision-lattice/
├── SKILL.md
├── agents/openai.yaml
└── references/
    ├── model-catalog.md
    └── routing-matrix.md
```

## Install

Clone this repository into your Codex skills directory:

```bash
git clone git@github.com:justtobeliev1/decision-lattice.git \
  "${CODEX_HOME:-$HOME/.codex}/skills/decision-lattice"
```

## Example Prompts

```text
Use $decision-lattice to analyze whether we should build this feature in-house or buy from a vendor.

Use $decision-lattice to pressure-test this product strategy under uncertainty and tail risk.

Use $decision-lattice to pick the best mental models for this hiring and org design decision.
```

## Design Principles

- choose the smallest useful set of models
- include a challenger model when the frame may be wrong
- protect survivability before optimization in tail-heavy situations
- separate reasoning quality from evidence quality

## License

MIT
