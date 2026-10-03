# Scientific Software Testing Policy

## Test the science, not only the syntax

A passing build or absence of crashes is insufficient for scientific software.

Use the applicable layers:

### Unit tests
Test small functions and equations.

Examples:
- conversion factors;
- constitutive correlations;
- individual balance terms;
- interpolation;
- boundary-condition helpers.

### Integration tests
Test connected components.

Examples:
- reactor heat -> process model;
- data parser -> model -> result writer;
- material properties -> solver -> release estimator.

### Regression tests
Protect previously verified scientific behavior.

Use carefully: a historical output is only a valid regression target if that output was itself accepted.

### Property/invariant tests
Often especially valuable for engineering mathematics.

Examples:
- mass cannot become negative;
- mole fractions sum appropriately;
- conserved inventory closes within tolerance;
- zero source gives zero source contribution;
- symmetric problem preserves symmetry;
- increasing a monotonic parameter produces the expected direction where mathematically established.

### Analytical/reference benchmarks
Whenever an exact or independently trusted reference exists, test against it.

### Convergence tests
For discretised models, investigate refinement in the relevant independent variables:
- mesh;
- timestep;
- tolerance;
- Monte-Carlo sample count;
- interface/capture resolution.

### Edge and limiting cases
Test physically meaningful limits, not only nominal cases.

## Tolerances

A numerical tolerance must have a rationale.

Do not loosen tolerances merely because CI fails.

Distinguish:
- floating-point tolerance;
- discretisation error;
- sampling uncertainty;
- model discrepancy.

## CI

CI should run the affordable subset of checks needed to detect accidental breakage.

Expensive validation studies may be separate reproducibility workflows, but their accepted evidence should be preserved.

## Scientific change rule

If a code change alters a canonical scientific result:
1. identify why;
2. determine whether it is correction, model change, parameter change or numerical effect;
3. update provenance;
4. rerun affected verification;
5. update manuscript only after the new result is accepted.
