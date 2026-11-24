---
title: Using the ML Top 10 as an ML Engineer
---

# Using the ML Top 10 as an ML Engineer

An ML engineer can use the risk pages at three decision points: when choosing
training data, when evaluating a candidate model, and when deciding what a
prediction endpoint will reveal. Keep the model version, dataset version,
preprocessing code, and evaluation results together so a later regression can
be traced to a specific change.

## Before training

For [ML02 data poisoning](../ML02_2023-Data_Poisoning_Attack.md) and
[ML08 model skewing](../ML08_2023-Model_Skewing.md), document where labels and
features come from, who can change them, and which checks run before training.
Split a trusted evaluation set before accepting new data. Compare label
frequencies, feature ranges, and performance across important subgroups with
the previous dataset version. A schema-valid sample can still carry the wrong
label, so review unexpected shifts rather than treating validation as proof of
trust.

If starting from a third-party model, record its source and version before
fine-tuning. [ML07 transfer learning](../ML07_2023-Transfer_Learning_Attack.md)
and [ML06 supply chain attacks](../ML06_2023-AI_Supply_Chain_Attacks.md) are
relevant even when your own training data is clean.

## Before promoting a model

Keep ordinary accuracy tests, then add security-oriented cases for the
interfaces your model exposes:

- For [ML01 input manipulation](../ML01_2023-Input_Manipulation_Attack.md),
  test small changes that should preserve the label, including preprocessing
  differences between training and serving.
- For [ML09 output integrity](../ML09_2023-Output_Integrity_Attack.md), verify
  that the application receives the same class, score, and model version that
  the approved inference service produced.
- For [ML10 model poisoning](../ML10_2023-Model_Poisoning.md), evaluate the
  exact artifact that will be deployed, not an earlier checkpoint with the
  same display name.

Record both a pass threshold and the observed result. A test that only shows
the model still runs will miss a targeted change in behavior.

## Before exposing predictions

Decide whether callers need confidence scores, embeddings, or only a class
label. Detailed outputs and unlimited queries can increase the opportunities
for [model inversion](../ML03_2023-Model_Inversion_Attack.md),
[membership inference](../ML04_2023-Membership_Inference_Attack.md), and
[model theft](../ML05_2023-Model_Theft.md). Test the released output format
against sensitive training records using approved test data. Share findings
with the API owner, who can enforce access and query limits at the service
boundary.
