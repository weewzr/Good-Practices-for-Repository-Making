# Scientific Configuration and Baseline Policy

Scientific results depend on code, geometry, parameters, boundary conditions, data versions, solver settings and model options.

## Freeze a baseline before comparison or review
Record:
- model commit;
- data/source versions;
- geometry/system definition;
- parameter set;
- assumptions;
- boundary/initial conditions;
- numerical settings;
- random-seed policy;
- environment/toolchain.

Use stable IDs such as CFG-BASE-001, CFG-SENS-004 and CFG-VAL-002 rather than "latest case".

## Change impact
When a configuration item changes, determine whether prior verification, sensitivity, validation, figures/tables and manuscript claims remain applicable.

## Comparison
Identify all intentional differences between configurations. Uncontrolled differences are confounders.

## Promotion
A candidate configuration becomes canonical only after required verification and review gates pass.
