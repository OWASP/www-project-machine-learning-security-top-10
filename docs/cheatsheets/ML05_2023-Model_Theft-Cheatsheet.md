## ML05:2023 Model Theft - Cheatsheets

Model theft has two different access paths: copying a model artifact, and
learning its behavior through repeated predictions. These OWASP guides address
different parts of those paths:

- [Secure AI Model Ops](https://cheatsheetseries.owasp.org/cheatsheets/Secure_AI_Model_Ops_Cheat_Sheet.html)
  covers access-controlled model registries, protection of model artifacts,
  inference API security and usage monitoring.
- [Authorization](https://cheatsheetseries.owasp.org/cheatsheets/Authorization_Cheat_Sheet.html)
  explains how to restrict access to sensitive resources. Apply those checks
  to model download, registry and export operations for every caller and model.
- [REST Security](https://cheatsheetseries.owasp.org/cheatsheets/REST_Security_Cheat_Sheet.html)
  covers authentication and request limits for prediction APIs. API keys and
  rate limits can slow bulk querying, but keys alone are not sufficient access
  control for a high-value model.
- [Logging](https://cheatsheetseries.owasp.org/cheatsheets/Logging_Cheat_Sheet.html)
  covers recording access failures and excessive use. Monitor model artifact
  downloads and unusual prediction volume without storing sensitive prompts or
  outputs unnecessarily.

An authorized client can still observe a model's responses. These controls
reduce exposure and make abuse visible; they do not guarantee that behavioral
extraction is impossible.
