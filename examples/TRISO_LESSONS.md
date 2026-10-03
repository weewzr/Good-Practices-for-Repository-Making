# TRISO Mathematical Derivation: Transferable Lessons

## What worked

- The original derivation remained preserved as raw evidence.
- A consolidated first-principles path was created without overwriting the original.
- Every substantive equation received a stable identifier in a canonical equation register.
- Continuous mathematics was separated from deterministic FV and stochastic WOS evidence.
- The exact production verification benchmark was frozen before comparing numerical methods.
- Interface conditions were derived from conservation and kept distinct from concentration-continuity assumptions.
- Numerical approximations such as finite capture distance, inverse-CDF interpolation, floating point and step caps were explicitly separated from physical assumptions.
- Reviews focused on concrete mathematical/numerical objects.
- Verification stages distinguished smoke execution, pilot uncertainty estimation and production verification.
- Supervisor integration was treated as a separate transfer problem with an exact external commit.

## What should not be repeated

- Do not treat one numerical method as validated because another numerical method agrees with it.
- Do not silently merge physically distinct initial-value/source problems.
- Do not call code behavior a physical design choice without evidence.
- Do not overclaim convergence order beyond demonstrated tests.
- Do not push an unfinished method into an authoritative external repository.
- Do not confuse a verification boundary with the final physical boundary.

## Reusable mathematical pattern

physical problem
-> definitions
-> conservation
-> constitutive law
-> governing equation
-> interface/boundary conditions
-> analytical reference
-> discretisation
-> implementation
-> verification
-> validation

## Method-distinction rule

If multiple methods are active, give each a stable identity and evidence stream. Agreement is useful evidence, not automatic proof of equivalence.
