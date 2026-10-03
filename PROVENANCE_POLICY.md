# Provenance Policy

## Purpose

Prevent source values, assumptions, derived calculations, model outputs, and claims from becoming indistinguishable.

## Required provenance classes

| Class | Meaning |
|---|---|
| SOURCE | Directly reported by a source |
| SOURCE-DERIVED | Calculated only from reported source information |
| ASSUMPTION | Deliberately selected project assumption |
| DESIGN BASIS | Reference design/configuration selected for modelling |
| MODEL PARAMETER | Parameter used by the mathematical/computational model |
| DERIVED | Direct mathematical consequence of stated inputs |
| RESULT | Output from the implemented model |
| UNRESOLVED | Evidence insufficient to classify/choose |
| HYPOTHESIS | Testable proposition, not established fact |

## Number register

Maintain a master number register for consequential numerical values.

Minimum fields:
- stable ID;
- value;
- unit;
- meaning;
- provenance class;
- source/reference;
- equation or file;
- calculation path;
- status;
- sensitivity relevance.

## Claim register

Maintain a claim/evidence map for consequential scientific statements.

Minimum fields:
- claim ID;
- claim text;
- evidence IDs;
- model/result dependencies;
- uncertainty;
- allowed wording;
- manuscript locations.

## Forbidden transitions

Never:
- source -> result without calculation;
- assumption -> source;
- design basis -> observed deployment fact;
- model result -> experimental validation;
- numerical agreement -> physical validation;
- literature comparison -> direct transferability without checking boundary/assumptions.

## Provenance is part of the result

A number without its origin and calculation path is not considered reproducible scientific evidence.
