# Master Workflow

## 1. Session recovery

At the start of every substantive session:

1. Read `STATUS.md`.
2. Read `PROJECT_BRIEF.md`.
3. Read `RESEARCH_FRAMING.md`.
4. Read the relevant canonical model/result/provenance files.
5. Read unresolved review findings.
6. Identify the current gate and exact dependency.

Do not restart the project because a new chat starts.

## 2. The bounded research loop

Every pass follows:

recover state
-> inspect the relevant evidence/model
-> identify one highest-value bounded task
-> make only the changes needed for that task
-> preserve provenance
-> run appropriate checks
-> record the new state
-> STOP

The next phase is not automatically executed.

## 3. Gate architecture

### G0 - Project definition
Required:
- primary research question;
- secondary questions;
- hypotheses/competing explanations;
- system boundary;
- intended outputs;
- success/falsification criteria.

### G1 - Evidence foundation
Required:
- search strategy;
- evidence matrix;
- primary-source coverage;
- contradiction search;
- citation metadata verification;
- unresolved evidence gaps.

### G2 - Model formulation
Required:
- assumptions;
- definitions;
- governing equations;
- constitutive relations;
- parameter provenance;
- boundary/interface conditions;
- dimensional checks;
- derivation or model justification.

### G3 - Implementation
Required:
- code/equation mapping;
- unit tests;
- deterministic inputs;
- reproducible execution;
- version/compiler/runtime record.

### G4 - Verification
Use the strongest applicable sequence:
- algebraic checks;
- dimensional checks;
- limiting cases;
- analytical/reference benchmarks;
- grid/time refinement;
- conservation/inventory checks;
- stochastic uncertainty;
- independent reproduction.

### G5 - Robustness
For important outputs:
- parameter sensitivity;
- uncertainty;
- alternate assumptions;
- competing configurations;
- adverse cases;
- evidence of whether conclusions survive.

### G6 - Integrated interpretation
Connect:
physical model -> quantitative results -> engineering meaning -> system-level effect -> constraints.

### G7 - Deployment / external reality
Keep separate from model closure:
- materials and equipment qualification;
- safety;
- regulation;
- siting;
- infrastructure;
- supply chain;
- market;
- logistics;
- financing;
- operational constraints.

### G8 - Manuscript and artifact QA
Verify:
- claim/evidence traceability;
- equations;
- references;
- figure/table provenance;
- reproducible build;
- exact PDF artifact;
- visual readability;
- no overclaiming.

## 4. Evidence -> Model -> Verification -> Claim

For every major conclusion, retain the chain:

CLAIM
-> supporting evidence
-> model/equation
-> assumptions/design basis
-> computation
-> verification
-> uncertainty
-> permitted wording

A claim must not become stronger than its weakest essential dependency.

## 5. Scientific truth labels

Every important value or statement should be classifiable as one of:

SOURCE
SOURCE-DERIVED
ASSUMPTION
DESIGN BASIS
MODEL PARAMETER
DERIVED
RESULT
UNRESOLVED
HYPOTHESIS

Do not silently relabel a literature value as a first-principles result.

## 6. Review policy

A review should answer a concrete question.

Examples:
- Is the governing derivation mathematically correct?
- Does the numerical scheme converge?
- Does the implementation match the mathematical contract?
- Are the economic conclusions robust?
- Does the manuscript exceed the evidence?

Do not initiate a review simply because one research pass has occurred.

## 7. Review lifecycle

REVIEW -> IMMUTABLE FINDINGS -> TARGETED RESOLUTION -> RE-RUN RELEVANT CHECKS -> CLOSURE RECORD

Do not rewrite the review history.

## 8. Canonical state policy

At all times identify:
- active canonical files;
- frozen/historical files;
- external authoritative files;
- unresolved work.

Old results remain useful as evidence but must never silently become current results.

## 9. Definition of done

A task is complete only when:
- the scientific object exists;
- provenance is recorded;
- verification appropriate to the object has run;
- repository state is reproducible;
- the current status is updated.

