# Data and Artifact Policy

## Data classes

Recommended separation:

```
data/
  raw/          # immutable source data
  external/     # third-party/reference data
  interim/      # transformed intermediate data
  processed/    # model-ready data
  generated/    # model-generated datasets
```

Small projects may collapse folders, but the semantic distinction should remain documented.

## Raw-data rule

Raw/source data should not be silently modified.

Transformations produce a new derived artifact with:
- generating script;
- source identifier;
- parameters;
- units/schema;
- date/version where relevant.

## Large or restricted data

Do not force large, licensed, sensitive or restricted datasets into Git.

Record:
- source;
- access procedure;
- version;
- checksum if permitted;
- expected local path;
- transformation procedure.

Use DVC/DataLad or another data-versioning system only when the project benefits from it.

## Generated outputs

Separate:
- canonical result data;
- temporary/scratch outputs;
- manuscript-ready tables/figures.

Generated figures and tables should point to their generating data and script.

## Artifact integrity

For final or submission-critical artifacts, record a hash when useful:
- PDF;
- dataset;
- release archive;
- model output bundle.

This establishes which exact artifact was reviewed.
