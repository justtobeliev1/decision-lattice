---
name: decision-lattice
description: Use this skill for open-ended decisions where the agent should select and combine the most relevant mental models from a 38-model lattice. Trigger it for strategy choices, tradeoff analysis, prioritization, architecture or product bets, hiring, planning under uncertainty, risk review, system interventions, market or org analysis, and any task where choosing the right lens changes the answer.
---

# Decision Lattice

## Overview

Decision Lattice helps Codex decide how to think before deciding what to recommend. It routes a problem through the smallest useful set of mental models, applies those models to the current situation, and produces a recommendation with assumptions, risks, evidence gaps, and revisit triggers.

## Strategy

- Frame the decision before picking models. Write down the objective, available options, main constraints, decision owner, time horizon, reversibility, and downside if the call is wrong.
- Classify the situation along a few practical axes: truth-seeking or option selection, simple or coupled system, single-actor or multi-actor, linear or nonlinear growth, low uncertainty or tail-risk-heavy, and reversible or path-locking.
- Select the smallest set of models that gives real coverage. Most tasks need 3 to 7 models. Use more only when the situation is genuinely cross-domain or high stakes.
- Mix complementary lenses. A good set often includes one model for truth, one for system response, one for incentives or actors, and one for time, uncertainty, or ruin.
- Add one challenger model when the current frame may be misleading. Good challengers include `paradigm shift`, `inversion`, `map is not the territory`, `dialectics`, and `bounded rationality`.
- Do not force full coverage of all 38 models. The skill exists to choose well, not to perform a ritual.
- Re-route when new evidence changes the frame. If the problem shifts from "what is true?" to "what should we do?", swap models instead of piling on more.

## Tool Boundaries

- This skill chooses lenses and analysis structure. It does not replace domain facts, measurements, or current evidence.
- Use normal repo, browser, data, or domain-specific tools to gather the facts that the selected models will operate on.
- For high-stakes legal, medical, financial, or safety decisions, treat the output as a reasoning aid and verify the underlying facts from authoritative sources.

## Routing Workflow

1. Restate the decision in one sentence.
2. Capture the minimum decision frame: objective, options, constraints, time horizon, reversibility, key actors, and major unknowns.
3. Read [references/routing-matrix.md](references/routing-matrix.md) to identify the default bundle for the situation.
4. Read [references/model-catalog.md](references/model-catalog.md) to choose the right reference file or files for this decision.
5. Open only the matching reference files. Default to one file, use two for cross-domain decisions, and use three only for high-stakes cases with genuine coupling across domains.
6. Apply the chosen models one by one.
7. Synthesize the result into a recommendation, an evidence plan, and clear revisit triggers.

## Output Contract

When you use this skill, structure the result in this order:

- `Decision Frame`: objective, options, assumptions, constraints.
- `Selected Models`: list each chosen model with a one-line reason.
- `What The Models Reveal`: show the important insight from each model.
- `Recommendation`: say what to do now and why this action dominates the alternatives given the current frame.
- `Evidence To Gather Next`: identify the missing facts most likely to change the call.
- `Failure Modes And Guardrails`: include downside, tail risk, coordination traps, or lock-in risk when relevant.
- `Revisit Triggers`: list the signals that should cause a fresh pass through the lattice.

## Fact Notes

- A mental model is a lens, not a law.
- Good routing beats exhaustive routing.
- Some models are best used in pairs: `expected value` plus `ergodicity`, `incentives` plus `game theory`, `feedback loops` plus `leverage points`, `first principles` plus `falsifiability`, and `opportunity cost` plus `marginal thinking`.
- When uncertainty is high, protect survivability before optimization.
- When a system is social, stated goals are weaker evidence than incentives and repeated behavior.

## References

- [references/routing-matrix.md](references/routing-matrix.md)
  - Read this first to map situation types to model bundles.
- [references/model-catalog.md](references/model-catalog.md)
  - Read this next to choose which model reference files to open.
- `references/models-*.md`
  - Open only the specific files selected by `model-catalog.md`.
