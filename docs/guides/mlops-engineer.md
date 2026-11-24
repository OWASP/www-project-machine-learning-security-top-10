---
title: Using the ML Top 10 as an MLOps Engineer
---

# Using the ML Top 10 as an MLOps Engineer

An MLOps engineer turns a reviewed training result into a running service.
Use the Top 10 to check the handoffs among training jobs, model registries,
deployment pipelines, and inference APIs. Record which team owns each handoff;
an approval in one system does not automatically protect the next one.

## Control the path to production

For [ML06 supply chain attacks](../ML06_2023-AI_Supply_Chain_Attacks.md),
inventory the packages, base images, preprocessing code, and external models
used by a run. Limit who can publish to the model registry. Keep a record of
the dataset version, training code revision, test result, and artifact digest
for each candidate release.

For [ML10 model poisoning](../ML10_2023-Model_Poisoning.md), promote by
immutable artifact identity rather than a mutable name such as `latest`.
Verify the artifact at deployment and restrict replacement of a running
model. A signed artifact proves the identity of a publisher, so the publisher
and the review step still matter.

## Guard the inference service

Restrict access to model administration and prediction endpoints separately.
Public prediction access may be intended; model download, configuration
changes, and registry writes usually need narrower roles. Apply limits and
monitoring to repeated queries relevant to
[ML03 model inversion](../ML03_2023-Model_Inversion_Attack.md),
[ML04 membership inference](../ML04_2023-Membership_Inference_Attack.md), and
[ML05 model theft](../ML05_2023-Model_Theft.md). Ask the ML team whether the
service needs to return confidence scores or embeddings at all.

Log the caller, model version, request outcome, and policy decision. Avoid
putting sensitive inputs or full predictions into operational logs by default.

## Monitor and recover

Track input distribution, output distribution, error rates, and model version
after release. A shift may point to [ML08 model skewing](../ML08_2023-Model_Skewing.md),
an upstream data change, or an ordinary business change; investigate before
labelling it an attack. Keep a known-good artifact and its dataset manifest so
the team can compare behavior and roll back a bad deployment. Exercise that
rollback path before an incident, including the route that updates the model
pointer and the route that verifies the version now serving.
