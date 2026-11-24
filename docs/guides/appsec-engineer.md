---
title: Using the ML Top 10 as an AppSec Engineer
---

# Using the ML Top 10 as an AppSec Engineer

Use the Top 10 to identify trust boundaries in an ML feature, then test the
controls at those boundaries. The list is a starting point for a test plan;
each risk page describes a class of failure, not a test that every application
must pass.

## Map the feature first

Draw the path from data collection through training, model storage, deployment,
and inference. For each step, record who can supply input, who can change it,
and who can read the output. Include the dataset and model registries, batch
jobs, third-party packages, and any public prediction API. A model served only
to employees still depends on the integrity of its upstream data and artifacts.

## Build tests from the relevant risk pages

| Boundary | Risk pages | Questions to test |
| --- | --- | --- |
| User input to prediction | [ML01](../ML01_2023-Input_Manipulation_Attack.md), [ML09](../ML09_2023-Output_Integrity_Attack.md) | Can a caller change preprocessing, input shape, or output handling so the application makes a different decision than intended? |
| Data and labels to training | [ML02](../ML02_2023-Data_Poisoning_Attack.md), [ML08](../ML08_2023-Model_Skewing.md) | Who can add or relabel samples? Are imported datasets versioned, reviewed, and checked against a separate trusted set? |
| Packages and models to deployment | [ML06](../ML06_2023-AI_Supply_Chain_Attacks.md), [ML10](../ML10_2023-Model_Poisoning.md) | Can an untrusted dependency or model artifact enter the build or registry? Is promotion restricted to reviewed, traceable versions? |
| Predictions to outside callers | [ML03](../ML03_2023-Model_Inversion_Attack.md), [ML04](../ML04_2023-Membership_Inference_Attack.md), [ML05](../ML05_2023-Model_Theft.md) | What does the API reveal through labels, confidence scores, embeddings, or repeated queries? Are access and query limits enforced across identities? |

Start with the boundaries the feature actually exposes. For example, a batch
classifier with no public prediction endpoint needs data provenance and
deployment review before a model-extraction test. A public prediction API
needs both authorization tests and a privacy review of its outputs.

## Record evidence and hand off fixes

Keep a reproducible test input, the observed output, the model or dataset
version, and the expected control for each finding. Use test accounts and
synthetic records; do not put real training records into reports or logs.
Confirm the result against a clean version before calling a changed prediction
an attack. When handing the issue to the ML or MLOps team, name the control
owner and a retest: a blocked import, a rejected artifact, or a prediction
endpoint that no longer exposes the measured signal.
