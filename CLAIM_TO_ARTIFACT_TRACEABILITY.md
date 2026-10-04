# Claim-to-Artifact Traceability

## Objective

A reader should be able to start from a manuscript claim and trace backward to the exact evidence and computation that supports it.

## Traceability chain

Manuscript claim
-> claim ID
-> canonical result ID
-> equation/model
-> configuration/assumptions
-> source data/parameters
-> verification evidence
-> generating code/commit

The reverse direction should also work:

source/input
-> model
-> result
-> figure/table
-> manuscript claim

## Tables and figures

For every consequential figure/table record:
- stable ID;
- source data;
- generating script/model;
- generating commit;
- key assumptions;
- whether values are source, derived or results;
- manuscript location;
- caption qualifications.

## Publication gate

Before final artifact closure:
- no consequential orphan number;
- no consequential orphan claim;
- no manually altered scientific figure without provenance;
- no table value that disagrees with canonical result data.

## Exact artifact identity

For a final PDF or release bundle, record:
- source commit;
- build command;
- build/run ID if CI is used;
- checksum/hash where useful.

This distinguishes the artifact actually reviewed from later or local variants.
