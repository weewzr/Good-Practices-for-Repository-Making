# Verification, Validation and Uncertainty Quantification Policy

## Keep these questions separate

Conceptual-model validity: are the chosen mechanisms, boundaries and assumptions appropriate?

Code verification: are the intended equations and algorithms implemented correctly?

Solution verification: how large is numerical error in this computed solution?

Validation: how well does the model represent relevant physical observations under matched conditions?

Uncertainty quantification: how do uncertain inputs, numerical uncertainty and model discrepancy affect quantities of interest?

## Minimum record
For each important quantity of interest identify:
- physical/model assumptions;
- parameter uncertainty;
- input/data uncertainty;
- numerical/discretisation uncertainty;
- stochastic/sampling uncertainty;
- model-form limitations;
- validation evidence, if available.

## Verification
Use as applicable: analytical solutions, manufactured solutions, conservation/invariant tests, independent implementations, limiting cases, mesh/time/tolerance refinement, stochastic convergence and accepted benchmarks.

## Validation
Match geometry, material/state, initial conditions, boundary conditions, operating conditions and measured-quantity definition as closely as possible.

Do not label a loose literature-range comparison as physical validation when conditions materially differ.

Validation evidence may be labelled NONE, QUALITATIVE, TREND, BENCHMARK-COMPARISON, QUANTITATIVE-MATCHED or MULTI-CONDITION.

## Uncertainty
Choose methods appropriate to the model: local sensitivity, scenario/envelope analysis, Monte Carlo, structured sampling, surrogate/emulator, Bayesian methods, or bounded/interval analysis.

Do not attach probabilistic meaning to an arbitrary scenario range.

Keep model-form uncertainty separate from parameter uncertainty.

## Reporting
Final claims identify which uncertainty sources were quantified and which remain qualitative or unresolved.
