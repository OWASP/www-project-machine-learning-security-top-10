---
layout: col-sidebar
type: documentation
altfooter: true
level: 4
auto-migrated: 0
document: OWASP Machine Learning Security Top Ten 2023
year: 2023
order: 9
title: ML09:2023 Output Integrity Attack
lang: en
tags:
  [
    OWASP Machine Learning Security Top Ten 2023,
    Top Ten,
    ML09:2023,
    mltop10,
    mlsectop10,
  ]
exploitability: 5
detectability: 3
technical: 3
---

## Description

In an Output Integrity Attack scenario, an attacker aims to modify or manipulate
the output of a machine learning model in order to change its behavior or cause
harm to the system it is used in.

## How to Prevent

**Using cryptographic methods:** Cryptographic methods like digital signatures
and secure hashes can be used to verify the authenticity of the results.

**Secure communication channels:** Communication channels between the model and
the interface responsible for displaying the results should be secured using
secure protocols such as SSL/TLS.

**Input Validation:** Input validation should be performed on the results to
check for unexpected or manipulated values.

**Tamper-evident logs:** Maintaining tamper-evident logs of all input and output
interactions can help detect and respond to any output integrity attacks.

**Regular software updates:** Regular software updates to fix vulnerabilities
and security patches can help reduce the risk of output integrity attacks.

**Monitoring and auditing:** Regular monitoring and auditing of the results and
the interactions between the model and the interface can help detect any
suspicious activities and respond accordingly.

## Risk Factors

|                                                                                                 Threat Agents/Attack Vectors                                                                                                 |                                                                                                                                        Security Weakness                                                                                                                                        |                                                                                                                                                 Impact                                                                                                                                                 |
| :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
|                                                               Exploitability: 5 (Easy) <br><br> _ML Application Specific: 4_ <br> _ML Operations Specific: 4_                                                                |                                                                                                                                   Detectability: 3 (Moderate)                                                                                                                                   |                                                                                                                                        Technical: 3 (Moderate)                                                                                                                                         |
| Threat Actors: Malicious attackers or insiders who have access to the model's inputs and outputs. <br> Third-party entities who have access to the inputs and outputs and may tamper with them to achieve a certain outcome. | Lack of proper authentication and authorization measures to ensure the integrity of the inputs and outputs. <br><br> Inadequate validation and verification of inputs and outputs to prevent tampering. <br><br> Insufficient monitoring and logging of inputs and outputs to detect tampering. | Loss of confidence in the model's predictions and results. <br><br> Financial loss or damage to reputation if the model's predictions are used to make important decisions. <br><br> Security risks if the model is used in a critical application such as financial fraud detection or cybersecurity. |

It is important to note that this chart is only a sample based on
[the scenario below](#scenario1) only. The actual risk assessment will depend on
the specific circumstances of each machine learning system.

## Example Attack Scenarios

### Scenario \#1: Modification of patient health records {#scenario1}

An attacker has gained access to the output of a machine learning model that is
being used to diagnose diseases in a hospital. The attacker modifies the output
of the model, making it provide incorrect diagnoses for patients. As a result,
patients are given incorrect treatments, leading to further harm and potentially
even death.

## References
