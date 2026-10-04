# Published Result Contract

## Principle

A number used in a final report, paper, presentation, or formal review should be reproducible from an identifiable repository state.

## Required identity for consequential published results

Record:
- result ID;
- git commit;
- branch/tag if relevant;
- whether working tree was clean;
- exact command;
- input/data versions;
- configuration;
- environment/toolchain;
- output artifact;
- verification status.

## Clean-tree rule

Prefer generating final/published results from a clean committed working tree.

If this is impossible, archive the exact patch/diff and explain why. An unrecorded dirty tree is not an acceptable source for a canonical published number.

## Data pinning

Do not use an unqualified "latest" dataset for a published result.

Use, where possible:
- release/version;
- revision/commit;
- retrieval date;
- checksum;
- archived local snapshot consistent with licensing.

## Expensive workflows

When full recomputation is impractical, preserve:
- exact code;
- exact configuration;
- precomputed intermediate/result artifacts;
- checksums;
- representative smaller verification case;
- resource/time estimate.

This provides an artifact pathway without pretending that expensive execution is free.

## Manuscript mapping

Every consequential final table/figure should be traceable to one or more published-result records.
