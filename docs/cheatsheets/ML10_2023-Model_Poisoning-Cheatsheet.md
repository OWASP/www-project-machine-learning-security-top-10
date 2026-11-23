## ML10:2023 Model Poisoning - Cheatsheets

Model poisoning can happen during training or when a model artifact is replaced
before deployment. These OWASP guides cover different points in that path:

- [Secure AI Model Ops](https://cheatsheetseries.owasp.org/cheatsheets/Secure_AI_Model_Ops_Cheat_Sheet.html)
  covers auditable training pipelines, controlled model registries, signed
  model artifacts and monitoring for changes in behavior.
- [Software Supply Chain Security](https://cheatsheetseries.owasp.org/cheatsheets/Software_Supply_Chain_Security_Cheat_Sheet.html)
  explains artifact provenance and signature verification. Apply those checks
  when moving a trained model from a build or registry into serving.
- [Key Management](https://cheatsheetseries.owasp.org/cheatsheets/Key_Management_Cheat_Sheet.html)
  covers protection and rotation of the keys used to authenticate model
  artifacts. A signature cannot establish provenance if its signing key is
  compromised.
- [Logging](https://cheatsheetseries.owasp.org/cheatsheets/Logging_Cheat_Sheet.html)
  covers tamper detection for audit records. Record model publication,
  deployment and failed integrity checks so an unexpected replacement can be
  investigated.

Artifact integrity checks do not catch poisoned training data or a harmful
model that was signed by an authorized party. Validate data provenance and
evaluate model behavior before promotion as well.
