## ML04:2023 Membership Inference Attack - Cheatsheets

Membership inference asks whether a particular person's record was included
in a model's training data. An attacker may compare the model's behavior on
candidate records with behavior on records known to be outside the training
set. The following OWASP guidance helps reduce this disclosure risk:

- [Secure AI Model Ops](https://cheatsheetseries.owasp.org/cheatsheets/Secure_AI_Model_Ops_Cheat_Sheet.html)
  recommends differential privacy or anonymization when training on sensitive
  data. It also covers access controls and abuse monitoring for inference APIs.
  Evaluate the privacy impact of the chosen training method against the actual
  model and dataset; simply hiding the training set is insufficient.
- [REST Security](https://cheatsheetseries.owasp.org/cheatsheets/REST_Security_Cheat_Sheet.html)
  covers authentication, authorization, and request limits for APIs. Apply
  these to prediction endpoints to limit automated probing, including across
  accounts and API keys.
- [Logging](https://cheatsheetseries.owasp.org/cheatsheets/Logging_Cheat_Sheet.html)
  describes how to record security events while excluding sensitive data.
  Monitor repeated queries and unusual output patterns without copying private
  prediction inputs into logs.

Rate limits and monitoring can make large-scale probing harder, but they do
not remove information already exposed by a model's outputs. Test membership
inference risk before releasing a model trained on sensitive records.
