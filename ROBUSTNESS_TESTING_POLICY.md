# Robustness and Failure-Oriented Testing

## Purpose

Engineering models should be challenged outside the preferred base case.

## Test families

### Boundary tests
Evaluate variables at or near the supported physical/model limits.

### Invalid-input tests
Impossible or malformed states should fail visibly rather than return plausible-looking numbers.

### Conservation and invariant stress
Target cases likely to expose mass, energy, charge, inventory, probability, positivity or symmetry violations.

### Alternative-model challenge
Where credible competing constitutive models/correlations exist, test whether conclusions depend on the model choice.

### Assumption challenge
Remove or reverse a favorable assumption where physically meaningful.

### Adverse-but-plausible scenarios
Test combinations within defensible ranges that are unfavorable to the preferred conclusion.

### Numerical stress
Challenge mesh, timestep, solver tolerance, conditioning, stochastic censoring, sampling and interface resolution where relevant.

### Claim falsification
For each major conclusion ask:
"What observation, parameter range, model choice or external condition would make this conclusion false?"

## Supported-domain behavior

The supported domain of a model should be explicit.

Outside that domain, prefer a clear error/warning to silent extrapolation.

## Interpretation

A challenge test may strengthen a conclusion, narrow its valid domain, expose sensitivity, or invalidate the preferred design. All are scientifically useful outcomes.
