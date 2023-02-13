---

document: OWASP Machine Learning Security Top Ten 2023
year: 2023
order: 6
title: ML05:2023:Model_Stealing
lang: en
author:
contributors:
tags: OWASP Top Ten 2023, Top Ten, ML05:2023
exploitability: 4
prevalence:
detectability: 3
technical: 4
redirect_from:

---

+----------------------+-----------------------+-----------------------+
| Threat agents/Attack | Security Weakness     | Impact                |
| vectors              |                       |                       |
+======================+=======================+=======================+
| Exploitability: 4    | Detectability: 3      | Technical: 4          |
| (Effort required to  |                       |                       |
| exploit this         | (Detection of this    | (Moderate technical   |
| weakness is          | attack is moderately  | skill required)       |
| moderate)            | challenging)          |                       |
|                      |                       |                       |
| ML Application       |                       |                       |
| Specific: 4          |                       |                       |
|                      |                       |                       |
| ML Operations        |                       |                       |
| Specific: 3          |                       |                       |
+----------------------+-----------------------+-----------------------+
| Agent/Attack Vector: | Unsecured model       | The impact of a model |
| This refers to the   | deployment: The       | theft could be both   |
| entity that carries  | unsecured deployment  | on the                |
| out the attack, in   | of the model makes it | confidentiality of    |
| this case, it is an  | easier for the        | the data used to      |
| attacker who wants   | attacker to access    | train the model and   |
| to steal the machine | and steal the model.  | the reputation of the |
| learning model.      |                       | organization that     |
|                      |                       | developed the model.\ |
|                      |                       | Confidentiality,      |
|                      |                       | Reputation            |
+----------------------+-----------------------+-----------------------+

It is important to note that this chart is only a sample based on
scenario below, and the actual risk assessment will depend on the
specific circumstances of each machine learning system.

**Description:**

Model stealing attacks occur when an attacker gains access to the
model's parameters.

**Example Attack Scenario:**

Scenario: Stealing a machine learning model from a competitor

A malicious attacker is working for a competitor of a company that has
developed a valuable machine learning model. The attacker wants to steal
this model so that their company can gain a competitive advantage and
start using it for their own purposes.

The attacker executed this attack by reverse engineering the company's
machine learning model, either by disassembling the binary code or by
accessing the model's training data and algorithm. Once the attacker
has reverse engineered the model, they can use this information to
recreate the model and start using it for their own purposes. This can
result in significant financial loss for the original company, as well
as damage to their reputation.

**How to Prevent:**

Encryption: Encrypting the model's code, training data, and other
sensitive information can prevent attackers from being able to access
and steal the model.

Access Control: Implementing strict access control measures, such as
two-factor authentication, can prevent unauthorized individuals from
accessing and stealing the model.

Regular backups: Regularly backing up the model's code, training data,
and other sensitive information can ensure that it can be recovered in
the event of a theft.

Model Obfuscation: Obfuscating the model's code and making it difficult
to reverse engineer can prevent attackers from being able to steal the
model.

Watermarking: Adding a watermark to the model's code and training data
can make it possible to trace the source of a theft and hold the
attacker accountable.

Legal protection: Securing legal protection for the model, such as
patents or trade secrets, can make it more difficult for an attacker to
steal the model and can provide a basis for legal action in the event of
a theft.

Monitoring and auditing: Regularly monitoring and auditing the model's
use can help detect and prevent theft by detecting when an attacker is
attempting to access or steal the model.

**References:**
