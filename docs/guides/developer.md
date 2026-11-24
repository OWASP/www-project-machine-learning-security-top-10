---
title: Using the ML Top 10 as a Developer
---

# Using the ML Top 10 as a Developer

A developer often connects an application to a model without training it.
Use the Top 10 to review the API boundary, the code that acts on predictions,
and the dependencies that load model artifacts. The application must still
enforce its own authorization and business rules when the model is wrong.

## Treat inference as an external boundary

Define the accepted input shape and size before calling the model. Reject
unexpected fields, malformed arrays, and oversized requests at the service
boundary. For [ML01 input manipulation](../ML01_2023-Input_Manipulation_Attack.md),
test how preprocessing handles missing values, encodings, and values near
decision thresholds. Share these cases with the ML engineer so the serving
path and the training-time expectations can be compared.

Authenticate the caller and authorize the action using application data,
not a model score. Apply per-caller query limits if the endpoint exposes
predictions to untrusted clients. Detailed scores and repeated queries can
aid [ML03 model inversion](../ML03_2023-Model_Inversion_Attack.md),
[ML04 membership inference](../ML04_2023-Membership_Inference_Attack.md), or
[ML05 model theft](../ML05_2023-Model_Theft.md). Return only the output the
feature needs.

## Keep the decision path explicit

For [ML09 output integrity](../ML09_2023-Output_Integrity_Attack.md), identify
the step that turns a model response into a user-visible or state-changing
action. Check the response schema, model version, and allowed values there.
Handle timeouts and invalid output explicitly. If the prediction controls a
high-impact action, require a separate policy check or human review as the
feature requires; a plausible-looking score is not authorization.

In tests, replace the model response with a valid low-confidence result, an
unexpected class, malformed JSON, and an error. Verify that none of these
paths silently takes the privileged action. A model API mock is enough to
exercise the application's decision code without retraining a model.

## Review what the app loads

Loading a model can execute code, depending on the format and library. Pin
and review the libraries and artifacts used by the service, and avoid unsafe
deserialization of untrusted files. See
[ML06 supply chain attacks](../ML06_2023-AI_Supply_Chain_Attacks.md) and
[ML10 model poisoning](../ML10_2023-Model_Poisoning.md) for the upstream
risks. Record the approved artifact identity alongside the application
release so an unexpected model change can be investigated.
