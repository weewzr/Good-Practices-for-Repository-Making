# Good Practices for Scientific Research Repositories

A reusable operating framework for AI-assisted engineering and scientific research projects.

This repository distils lessons from:
- CN4252 nuclear-assisted SMR + CCS implementation
- TRISO source-term mathematical derivation and numerical verification
- current scientific-agent workflow practices, including the K-Dense AI scientific-agent-skills repository

The goal is not to make every research project identical. It is to provide a common governance, provenance, verification, GitHub, and manuscript framework while allowing each project to use the scientific workflow appropriate to its problem.

## Start here

1. Read `MASTER_WORKFLOW.md`.
2. Copy `templates/PROJECT_BRIEF.md` and `templates/RESEARCH_FRAMING.md` into a new project.
3. Select the project mode in `PROJECT_MODES.md`.
4. Establish the canonical state and provenance policy before substantive work.
5. Work in bounded gates. Do not use repeated unstructured "continue" cycles.
6. Stop at each gate and record exactly what changed and what remains.

## Core principles

- The repository is the durable project memory; chats are temporary workers.
- Evidence, assumptions, models, derivations, results, and claims remain distinguishable.
- A calculation running successfully is not the same as numerical verification.
- Agreement between two numerical methods is not automatically physical validation.
- Reviews are triggered by substantive gates, not by elapsed conversation length.
- Historical work remains auditable but cannot silently replace the current canonical result.
- Figures are scientific artifacts and require provenance and topology checks.
- Manuscripts are downstream of the verified model and evidence; they must not create unsupported certainty.

## Project family

### System-integration research
Use for process systems, reactor integration, techno-economics, lifecycle assessment, or deployment studies.

Typical chain:
problem -> reference system -> proposed architecture -> boundary/design basis -> balances -> subsystem models -> integration -> sensitivity/uncertainty -> alternatives -> deployment -> economics -> conclusion

### Mathematical/model-development research
Use for derivations, PDE models, numerical methods, source terms, transport models, or code redevelopment.

Typical chain:
physical problem -> definitions -> conservation -> constitutive laws -> governing equations -> boundary/interface conditions -> analytical solution/reference -> discretisation -> implementation -> verification -> validation

Both modes share the same governance and provenance rules.
