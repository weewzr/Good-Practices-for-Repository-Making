# Experiment and Analysis Policy

## Purpose

Every substantial computation, numerical experiment, design comparison, or sensitivity study should answer a predeclared question.

## Before running

Record:
- experiment/analysis ID;
- scientific question;
- hypothesis or expected discriminating outcome;
- baseline/reference;
- variables changed;
- variables held fixed;
- parameter ranges and why;
- outputs/metrics;
- acceptance/falsification criterion where applicable;
- required verification;
- computational budget or stopping rule if relevant.

Do not choose the success criterion after seeing the preferred result.

## After running

Record:
- exact code/commit;
- configuration/input set;
- runtime/tool versions when relevant;
- result artifacts;
- verification status;
- interpretation;
- whether the hypothesis survived;
- anomalies;
- next decision.

## Negative results

A failed hypothesis, non-convergent method, infeasible configuration, null sensitivity, or rejected design is a research result when it changes what should be done next.

Do not delete negative results merely because they are unsuitable for the final manuscript.

Preserve enough evidence to prevent future workers from repeating the same dead end.

## Promotion rule

Exploratory work becomes canonical only after:
1. the question is clear;
2. the method is documented;
3. provenance is complete;
4. relevant verification passes;
5. the result is explicitly accepted/promoted.

Exploratory notebooks/scripts must not silently become the source of manuscript numbers.

## Baseline rule

Comparisons require a frozen baseline with the same relevant boundary and metrics.

Do not compare configurations under inconsistent system boundaries without explicitly identifying the mismatch.
