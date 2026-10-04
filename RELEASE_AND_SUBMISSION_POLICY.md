# Release and Submission Policy

## Purpose

A final manuscript, report, presentation, or software release is a frozen scientific artifact, not simply the newest file in a folder.

## Pre-release checks

### Science
- canonical results accepted;
- open blockers identified;
- uncertainty/limitations visible;
- claims do not exceed evidence.

### Reproducibility
- core workflow executes;
- tests/verification pass or exceptions are documented;
- dependencies/environment recorded;
- generated figures/tables correspond to canonical results.

### Manuscript
- references resolve;
- equations/cross-references resolve;
- figures/tables are readable;
- terminology is consistent;
- exact artifact visually inspected.

### Repository
- STATUS updated;
- canonical pointers correct;
- historical results distinguishable;
- release/submission commit recorded.

## Release identity

Record:
- commit SHA;
- version/tag if used;
- artifact hash;
- date;
- CI/build run;
- known limitations.

## Archive options

For substantial public research/software, consider:
- GitHub Release;
- CITATION.cff;
- Zenodo DOI/archive;
- software/data metadata.

These are optional for coursework unless required.

## Post-release changes

Do not silently replace the released scientific artifact.

Corrections should create a new version with an explicit change record.
