## ML09:2023 Output Integrity Attack - Cheatsheets

These OWASP cheat sheets cover different points where an inference result can be
changed between the model and the system that acts on it:

- [Transport Layer Security](https://cheatsheetseries.owasp.org/cheatsheets/Transport_Layer_Security_Cheat_Sheet.html)
  protects results in transit between services. It does not establish that the
  model or either endpoint produced a trustworthy result.
- [Key Management](https://cheatsheetseries.owasp.org/cheatsheets/Key_Management_Cheat_Sheet.html)
  covers keys for message authentication codes and digital signatures. If
  results cross a trust boundary, authenticate them and verify them before a
  downstream service uses them.
- [Input Validation](https://cheatsheetseries.owasp.org/cheatsheets/Input_Validation_Cheat_Sheet.html)
  applies at the consumer of a model result: validate its structure, types and
  permitted values before using it in a decision or command.
- [Logging](https://cheatsheetseries.owasp.org/cheatsheets/Logging_Cheat_Sheet.html)
  covers protecting event records from alteration and monitoring suspicious
  changes. Log the model, result identifier and downstream action without
  recording sensitive inputs or outputs unnecessarily.

These controls help preserve and check the output *after* inference. They cannot
prove that the model's prediction itself is correct.
