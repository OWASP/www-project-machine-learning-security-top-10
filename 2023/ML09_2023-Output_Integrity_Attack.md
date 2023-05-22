---
layout: col-sidebar
title: OWASP Machine Learning Security Top Ten
tags: mltop10
type: documentation
altfooter: true
level: 4
auto-migrated: 0
pitch:
---
---

document: OWASP Machine Learning Security Top Ten 2023
year: 2023
order: 6
title: ML09:2023:Output_Integrity_Attack
lang: en
author:
contributors:
tags: OWASP Top Ten 2023, Top Ten, ML09:2023
exploitability: 5
prevalence:
detectability: 3
technical: 3
redirect_from:

---

|                                                                                        Threat agents/Attack vectors                                                                                       |                                                                                                                                 Security Weakness                                                                                                                                |                                                                                                                                          Impact                                                                                                                                         |
|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
|                                                          Exploitability: 5 (Easy)<br>ML Application Specific: 4<br>ML Operations Specific: 4<br>                                                          |                                                                                                                               Detectability: 3<br>                                                                                                                               |                                                                                                                                    Technical: 3<br>                                                                                                                                     |
| Malicious attackers or insiders who have access to the model's inputs and outputs<br>Third-party entities who have access to the inputs and outputs and may tamper with them to achieve a certain outcome | Lack of proper authentication and authorization measures to ensure the integrity of the inputs and outputs<br>Inadequate validation and verification of inputs and outputs to prevent tampering<br>Insufficient monitoring and logging of inputs and outputs to detect tampering | Loss of confidence in the model's predictions and results<br>Financial loss or damage to reputation if the model's predictions are used to make important decisions<br>Security risks if the model is used in a critical application such as financial fraud detection or cybersecurity |


It is important to note that this chart is only a sample based on
scenario below, and the actual risk assessment will depend on the
specific circumstances of each machine learning system.

**Description:**

In an Output Integrity Attack scenario, an attacker aims to modify or
manipulate the output of a machine learning model in order to change its
behavior or cause harm to the system it is used in.

**Example Attack Scenario:**

An attacker has gained access to the output of a machine learning model
that is being used to diagnose diseases in a hospital. The attacker
modifies the output of the model, making it provide incorrect diagnoses
for patients. As a result, patients are given incorrect treatments,
leading to further harm and potentially even death.

**How to Prevent:**

Using cryptographic methods: Cryptographic methods like digital
signatures and secure hashes can be used to verify the authenticity of
the results.

Secure communication channels: Communication channels between the model
and the interface responsible for displaying the results should be
secured using secure protocols such as SSL/TLS.

Input Validation: Input validation should be performed on the results to
check for unexpected or manipulated values.

Tamper-evident logs: Maintaining tamper-evident logs of all input and
output interactions can help detect and respond to any output integrity
attacks.

Regular software updates: Regular software updates to fix
vulnerabilities and security patches can help reduce the risk of output
integrity attacks.

Monitoring and auditing: Regular monitoring and auditing of the results
and the interactions between the model and the interface can help detect
any suspicious activities and respond accordingly.

**[References]{.underline}**:
