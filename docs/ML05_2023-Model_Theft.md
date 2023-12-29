---
layout: col-sidebar
type: documentation
altfooter: true
level: 4
auto-migrated: 0
document: OWASP Machine Learning Security Top Ten 2023
year: 2023
order: 5
title: ML05:2023 Model Theft
lang: en
tags:
  [
    OWASP Machine Learning Security Top Ten 2023,
    Top Ten,
    ML05:2023,
    mltop10,
    mlsectop10,
  ]
exploitability: 4
detectability: 3
technical: 4
---

## Description

Model theft attacks occur when an attacker gains access to the model's
parameters.

## How to Prevent

**Encryption:** Encrypting the model's code, training data, and other sensitive
information can prevent attackers from being able to access and steal the model.

**Access Control:** Implementing strict access control measures, such as
two-factor authentication, can prevent unauthorized individuals from accessing
and stealing the model.

**Regular backups:** Regularly backing up the model's code, training data, and
other sensitive information can ensure that it can be recovered in the event of
a theft.

**Model Obfuscation:** Obfuscating the model's code and making it difficult to
reverse engineer can prevent attackers from being able to steal the model.

**Watermarking:** Adding a watermark to the model's code and training data can
make it possible to trace the source of a theft and hold the attacker
accountable.

**Legal protection:** Securing legal protection for the model, such as patents
or trade secrets, can make it more difficult for an attacker to steal the model
and can provide a basis for legal action in the event of a theft.

**Monitoring and auditing:** Regularly monitoring and auditing the model's use
can help detect and prevent theft by detecting when an attacker is attempting to
access or steal the model.

## Risk Factors

|                                                            Threat Agents/Attack Vectors                                                             |                                                         Security Weakness                                                         |                                                                                Impact                                                                                 |
| :-------------------------------------------------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
|                         Exploitability: 4 (Moderate) <br><br> _ML Application Specific: 4_ <br> _ML Operations Specific: 3_                         |                                                    Detectability: 3 (Moderate)                                                    |                                                                        Technical: 4 (Moderate)                                                                        |
| Threat Agent: This refers to the entity that carries out the attack, in this case, it is an attacker who wants to steal the machine learning model. | Unsecured model deployment: The unsecured deployment of the model makes it easier for the attacker to access and steal the model. | The impact of a model theft could be both on the confidentiality of the data used to train the model and the reputation of the organization that developed the model. |

It is important to note that this chart is only a sample based on
[the scenario below](#scenario1) only. The actual risk assessment will depend on
the specific circumstances of each machine learning system.

## Example Attack Scenarios

### Scenario \#1: Stealing a machine learning model from a competitor {#scenario1}

A malicious attacker is working for a competitor of a company that has developed
a valuable machine learning model. The attacker wants to steal this model so
that their company can gain a competitive advantage and start using it for their
own purposes.

The attacker executed this attack by reverse engineering the company's machine
learning model, either by disassembling the binary code or by accessing the
model's training data and algorithm. Once the attacker has reverse engineered
the model, they can use this information to recreate the model and start using
it for their own purposes. This can result in significant financial loss for the
original company, as well as damage to their reputation.

## References
