# Resource and Runtime Policy

## Why record compute requirements?

Reproducibility includes feasibility. A command that requires undocumented hardware, memory or days of runtime is not meaningfully reproducible.

## Record when relevant

- CPU architecture/cores;
- RAM;
- GPU/accelerator and driver;
- compiler/toolchain;
- approximate runtime;
- storage requirement;
- parallelism;
- cluster/scheduler assumptions.

## Lightweight vs full reproduction

For expensive models provide, when possible:

### Smoke reproduction
Confirms installation, interfaces and a small representative calculation.

### Verification reproduction
Runs analytical/reference/convergence checks.

### Full scientific reproduction
Regenerates the canonical result set.

Keep these distinct. A smoke run is not validation.

## Coursework principle

Do not add heavyweight infrastructure merely to satisfy this policy. A short README table may be sufficient.
