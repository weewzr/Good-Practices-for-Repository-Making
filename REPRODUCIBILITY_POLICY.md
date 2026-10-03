# Reproducibility Policy

## Minimum reproducibility contract

A project should answer:

1. What exact inputs are required?
2. Where did they come from?
3. What software/environment is required?
4. What command regenerates the core results?
5. What command runs the verification/tests?
6. Which outputs are canonical?
7. Which outputs are generated and should not be edited manually?
8. What external dependencies cannot be archived in the repository?

## One-command principle

Where practical, expose simple commands such as:

```
make check
make reproduce
make paper
```

or equivalent scripts:

```
sh scripts/check.sh
sh scripts/reproduce.sh
sh paper/build.sh
```

The command names are not important. The ability to execute the complete dependency chain is.

## Clean-environment test

Before final closure, verify the documented workflow from a clean or freshly configured environment when practical.

A workflow that works only because of undocumented local state is not reproducible.

## Environment record

Record as applicable:
- operating system;
- compiler/interpreter;
- package/tool versions;
- dependency lockfile;
- environment variables that affect science;
- external executable versions;
- random seeds;
- hardware constraints when numerically relevant.

## Generated artifacts

Figures, tables and reported numerical outputs should preferably be regenerated from code/data rather than edited manually.

Track:
input -> script/model -> intermediate -> figure/table -> manuscript.

## Determinism

If deterministic:
- repeated execution should reproduce results within declared numerical tolerance.

If stochastic:
- record seed policy;
- sample size;
- uncertainty estimator;
- stopping/censoring rules;
- stochastic tolerance.

## Failure visibility

Do not disable a test or loosen a tolerance merely to obtain a passing build. Record and resolve the scientific cause.
