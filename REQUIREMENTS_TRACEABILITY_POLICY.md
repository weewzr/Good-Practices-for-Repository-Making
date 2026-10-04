# Requirements Traceability Policy

## Principle
Every consequential project requirement should state why it exists, what implements it, how it will be verified, and what evidence demonstrates closure. Define verification when the requirement is created, not after implementation.

## Requirement classes
Use as applicable: SCI scientific; ENG engineering/design; NUM numerical; DATA evidence/data; REP reporting; EXT external/course/regulatory.

## Lifecycle
PROPOSED -> ACCEPTED -> IMPLEMENTED -> VERIFIED.

Other states: DEFERRED, SUPERSEDED, NOT APPLICABLE, FAILED.

Never reuse stable IDs.

## Required fields
- stable ID
- requirement statement
- source/need
- rationale
- acceptance criterion
- verification method
- implementation/model location
- verification evidence
- status
- affected downstream claims/results

## Coverage audit
Before a major gate identify:
- requirements without source/need;
- requirements without implementation;
- requirements without verification;
- tests without requirements;
- final claims depending on failed or unverified requirements.

## Change management
When a requirement changes, record why, identify affected model/code/data/results, rerun impacted verification, and reassess downstream claims.
