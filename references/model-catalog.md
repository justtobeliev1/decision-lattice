# Model Catalog

Use this file after `routing-matrix.md`. Its job is to choose the smallest useful reference set.

## Load Rules

- Start with one reference file.
- Open a second file when the decision clearly spans two domains, such as product plus org design, or risk plus resource allocation.
- Open a third file only when the decision is high stakes and strongly coupled across domains.
- If you need a challenger lens, add the file that contains `paradigm shift`, `dialectics`, `map is not the territory`, `bounded rationality`, or `black swan`.

## Reference Map

| Need | Open this file | Covers |
| --- | --- | --- |
| truth, diagnosis, evidence quality | [models-epistemic.md](models-epistemic.md) | first principles, reasoning modes, falsifiability, information, map vs reality, simplicity |
| feedback, lock-in, system response | [models-systems.md](models-systems.md) | feedback loops, emergence, network effects, entropy, path dependence, leverage points |
| choice quality, tradeoffs, judgment limits | [models-decisions.md](models-decisions.md) | expected value, prospect theory, inversion, opportunity cost, marginal thinking, second-order thinking, bounded rationality, biases, circle of competence |
| actors, competition, institutions, hidden motives | [models-social.md](models-social.md) | natural selection, game theory, incentives, comparative advantage, social construction, defense mechanisms |
| growth, scale, ruin, survivability | [models-growth-risk.md](models-growth-risk.md) | compounding, scaling laws, diminishing returns, black swan, antifragility, ergodicity |
| reframing, invariants, recurring patterns, synthesis | [models-structure-meta.md](models-structure-meta.md) | paradigm shift, symmetry, recursion, latticework, dialectics |

## Common Two-File Pairings

- `models-epistemic.md` plus `models-decisions.md` for decisions with contested evidence.
- `models-systems.md` plus `models-social.md` for org, market, and platform moves.
- `models-decisions.md` plus `models-growth-risk.md` for bets with meaningful downside.
- `models-systems.md` plus `models-growth-risk.md` for scaling under fragility or operational decay.
- `models-social.md` plus `models-structure-meta.md` for institution design or frame conflicts.

## Suggested Bundle Patterns

- `clean frame`: `models-epistemic.md`
- `risky choice`: `models-decisions.md` plus `models-growth-risk.md`
- `messy system`: `models-systems.md`
- `competition`: `models-social.md` plus `models-decisions.md`
- `resource allocation`: `models-decisions.md` plus `models-growth-risk.md`
- `deep reframe`: `models-structure-meta.md` plus the main domain file
