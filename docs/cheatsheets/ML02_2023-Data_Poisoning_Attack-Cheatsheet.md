## ML02:2023 Data Poisoning Attack - Cheatsheets

Data poisoning changes the examples or labels that a training pipeline trusts.
The following OWASP guidance applies at different points before those inputs
reach the model:

- [Secure AI Model Ops](https://cheatsheetseries.owasp.org/cheatsheets/Secure_AI_Model_Ops_Cheat_Sheet.html)
  covers dataset validation, versioned and auditable training pipelines, and
  monitoring for unexpected changes in model behavior. Keep a record of which
  dataset version produced each model so a suspect run can be traced and rolled
  back.
- [Input Validation](https://cheatsheetseries.owasp.org/cheatsheets/Input_Validation_Cheat_Sheet.html)
  describes validation of structured inputs. Apply schema, range, and type
  checks at data ingestion; a well-formed record may still have a maliciously
  wrong label, so validation alone cannot establish its trustworthiness.
- [Software Supply Chain Security](https://cheatsheetseries.owasp.org/cheatsheets/Software_Supply_Chain_Security_Cheat_Sheet.html)
  covers provenance and integrity checks for artifacts. Preserve the source
  and integrity of externally supplied datasets and preprocessing code before
  admitting them into a training run.
- [Logging](https://cheatsheetseries.owasp.org/cheatsheets/Logging_Cheat_Sheet.html)
  covers audit events and protected log records. Log dataset imports, label
  changes, validation failures, and training runs with identifiers that link
  an output model back to its inputs.

These controls help establish where training data came from and what changed.
They do not prove that a trusted source supplied correct labels; independently
review high-impact samples and evaluate the resulting model against a separate
trusted validation set.
