---
title: Using the ML Top 10 as a Data Engineer
---

# Using the ML Top 10 as a Data Engineer

The data engineer controls the path from a source record to a training-ready
dataset. Use the Top 10 to decide which inputs need a trust check, which
changes need an audit trail, and which datasets may be promoted for training.

## Inventory sources and writers

For each dataset, record its owner, origin, collection method, retention
period, and every role or service that can append records or change labels.
Mark externally supplied feeds and user-generated content as separate trust
boundaries. [ML02 data poisoning](../ML02_2023-Data_Poisoning_Attack.md) can
enter through a legitimate import or annotation job; storage encryption alone
does not tell you whether the contents were trustworthy.

Pin the version of preprocessing code and third-party data packages used by
each run. Review the integrity and source of imported files and dependencies
before they enter the pipeline, as described by
[ML06 supply chain attacks](../ML06_2023-AI_Supply_Chain_Attacks.md).

## Gate dataset changes

Apply schema, type, range, and missing-value checks at ingestion. Add checks
that are specific to the dataset: duplicate identifiers, unexpected label
changes, shifts in class balance, or a sudden concentration of new samples
from one source. Reject or quarantine data that fails a check; keep the reason
and source identifier so a reviewer can investigate it.

Run distribution checks for [ML08 model skewing](../ML08_2023-Model_Skewing.md)
against both the previous approved training set and the data the model sees in
production. A change may be legitimate, but the ML team needs to see it before
retraining. For high-impact labels, use a second review path rather than
assuming that a syntactically valid label is correct.

## Make promotion reversible

Publish an immutable dataset version with a manifest of source versions,
transformation version, validation results, and approval. Restrict who can
replace the approved version or alter its manifest. Hand the ML engineer a
separate evaluation set that was not silently updated by the same import job.

If a later model behaves unexpectedly, this record should answer which input
changed and when. Restore a prior approved dataset version for a retest, then
compare model behavior before promoting another run. Do not copy sensitive
training rows into incident tickets or pipeline logs.
