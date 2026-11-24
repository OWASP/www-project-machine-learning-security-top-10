---
title: Using the ML Top 10 as a CISO
---

# Using the ML Top 10 as a CISO

Use the ML Top 10 to ask where an ML system crosses an organizational trust
boundary and who owns the control at that point. The list helps start a risk
review; its sample ratings are not a rating of your organization's systems.

## Start with an inventory

For each production ML system, identify the business decision it affects, the
data it trains on, the owner of the model, and the team that operates it. Note
whether outsiders can supply training data or query the model. Record the
third-party datasets, models, libraries, and services it depends on. This
inventory determines which Top 10 risk pages deserve attention first.

For example, a public prediction API makes
[model inversion](../ML03_2023-Model_Inversion_Attack.md),
[membership inference](../ML04_2023-Membership_Inference_Attack.md), and
[model theft](../ML05_2023-Model_Theft.md) relevant to the privacy and API
owners. A private batch model may put
[data poisoning](../ML02_2023-Data_Poisoning_Attack.md) and
[supply chain attacks](../ML06_2023-AI_Supply_Chain_Attacks.md) ahead of
public API abuse. The actual exposure and impact, not the category number,
set the priority.

## Assign controls to owners

Ask the data team to show how a training set is approved and traced back to
its sources. Ask the ML team to show the evaluation result for the exact model
version in production. Ask MLOps to show who can publish or replace that
version and how it can be rolled back. Ask the application team what happens
when the model returns an unexpected or low-confidence result. These checks
connect [model poisoning](../ML10_2023-Model_Poisoning.md) and
[output integrity](../ML09_2023-Output_Integrity_Attack.md) to named owners.

Record a control as implemented only when the owner can point to evidence:
an approval, an artifact identity, an access test, or a monitored event.
For gaps, record a decision, a remediation owner, and a date for a retest.

## Review after changes

Revisit the risk review when a new dataset, model provider, exposed endpoint,
or high-impact use case is introduced. Watch for changes in the input and
output distributions that may indicate
[model skewing](../ML08_2023-Model_Skewing.md), then have the technical team
investigate the cause. Track whether the organization can reproduce a model
release and roll it back, rather than counting only the number of models
scanned or policies written.
