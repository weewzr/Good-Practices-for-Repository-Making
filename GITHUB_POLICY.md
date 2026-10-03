# GitHub and Branch Safety Policy

## Canonical repository

One repository and one branch must be explicitly designated as canonical.

## Branches

Recommended:
- `main`: canonical active research state;
- feature branches: bounded changes;
- frozen tags/commits: historical milestones.

A separate authoritative supervisor/third-party repository must be treated as READ-ONLY unless explicit transfer authorization exists.

## Commit discipline

Prefer:
- one scientific change per commit;
- one targeted remediation per commit;
- one closure/status update after verification.

Commit messages should state what scientific or workflow object changed.

## Transfer rule

Before transferring code to an external repository, record:
- exact external base commit;
- exact source file/path;
- original behavior;
- proposed behavior;
- mathematical justification;
- tests;
- compatibility;
- provenance;
- patch/commit identity.

Do not push unfinished numerical methods into an authoritative production repository.
