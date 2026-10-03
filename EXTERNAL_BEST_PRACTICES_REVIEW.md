# External GitHub Best-Practices Review

## Purpose

This record documents external research-repository practices considered for this framework. Adoption is selective: a practice is included only when it improves scientific reproducibility, auditability, handover, or maintainability without imposing unnecessary infrastructure.

## Repositories and approaches reviewed

### The Turing Way / reproducible-project-template
Useful principles:
- repository templates as reusable starting points;
- reproducibility and collaboration as first-class repository concerns;
- project structure should support sharing research objects.

Adopted:
- template-first project initialization;
- reproducibility-oriented repository structure.

### Turing-Roche reproducible-project-template
Useful principles:
- operationalise reproducibility recommendations in an actual GitHub template;
- keep setup instructions visible and reusable.

Adopted:
- project bootstrap checklist;
- reproducibility checklist.

### CBS-HPC research-template
Useful principles:
- FAIR/open-science orientation;
- explicit code/data/dependency structure;
- environment management;
- testing/CI;
- CITATION metadata;
- data-versioning options;
- archival/publication support.

Adopted:
- data classification;
- environment/dependency recording;
- CITATION template;
- optional archival/release checklist.

Not mandatory:
- DVC/DataLad;
- automatic publication infrastructure;
- language-specific environment tooling.

These are selected only when project scale warrants them.

### timtroendle cookiecutter-reproducible-research / PyPSA project template
Useful principles:
- full workflow automation;
- raw inputs + code + text should regenerate reports;
- tests and workflow files are part of the repository;
- a single top-level build target is valuable.

Adopted:
- one-command reproduction target where feasible;
- manuscript artifacts should be generated from tracked sources;
- tests belong in the reproducibility path.

### yy/project-template
Useful principles:
- explicit src/tests/data/notebooks/paper/results/workflow separation;
- dependency lockfile;
- pre-commit/lint/check target;
- one command for full workflow and paper.

Adopted:
- optional source/test/workflow directories;
- clean check/build commands;
- dependency locking where supported.

### Netherlands eScience Center project-template
Useful principles:
- CITATION.cff;
- Zenodo metadata;
- CodeMeta;
- architecture notes;
- Architecture Decision Records (ADRs);
- software management/handover planning;
- release checklist;
- issue/PR templates;
- metadata validation;
- explicit maturity level;
- test installation from a clean environment.

Adopted:
- CITATION.cff template;
- architecture/decision records for consequential choices;
- handover checklist;
- clean-environment reproducibility check;
- optional release/archive policy.

Optional for coursework:
- Zenodo;
- CodeMeta;
- governance/community files;
- formal release process.

### FAIR4RS / FAIR-IMPACT
Useful principles:
- research software should be findable, accessible, interoperable and reusable;
- metadata should not be an afterthought;
- openness and FAIRness are related but not identical.

Adopted:
- metadata/citation readiness;
- source/version identification;
- reusable outputs and documented dependencies.

### Research software handoff practices
Useful principle:
- setup/handoff instructions should be tested rather than assumed correct.

Adopted:
- handover requires a fresh reader/environment to be able to locate canonical state and reproduce the core result.

## Practices deliberately not made universal

The framework does not require every project to use:
- Python;
- Conda;
- uv;
- Snakemake;
- Make;
- DVC;
- DataLad;
- Docker;
- Zenodo;
- notebooks;
- pre-commit.

Those are implementation choices. The invariant is the scientific requirement: dependencies, workflow, inputs, outputs and provenance must be reproducible.

## Resulting design philosophy

Use the lightest infrastructure that still guarantees:
1. scientific traceability;
2. deterministic recovery of project state;
3. repeatable computation;
4. explicit dependencies;
5. testable handover;
6. clear distinction between canonical and historical evidence.
