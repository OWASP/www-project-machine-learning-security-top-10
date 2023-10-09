---
layout: col-sidebar
type: documentation
altfooter: true
level: 4
auto-migrated: 0
document: OWASP Machine Learning Security Top Ten 2023
year: 2023
order: 4
title: ML04:2023 Membership Inference Attack
lang: en
tags:
  [
    OWASP Machine Learning Security Top Ten 2023,
    Top Ten,
    ML04:2023,
    mltop10,
    mlsectop10,
  ]
exploitability: 4
detectability: 3
technical: 4
---

## Description

Membership inference attacks occur when an attacker manipulates the model's
training data in order to cause it to behave in a way that exposes sensitive
information.

## How to Prevent

**Model training on randomized or shuffled data:** Training machine learning
models on randomized or shuffled data can make it more difficult for an attacker
to determine whether a particular example was included in the training dataset.

**Model Obfuscation:** Obfuscating the model's predictions by adding random
noise or using differential privacy techniques can help prevent membership
inference attacks by making it harder for an attacker to determine the model's
training data.

**Regularisation:** Regularisation techniques such as L1 or L2 regularization
can help prevent overfitting of the model to the training data, which can reduce
the model's ability to accurately determine whether a particular example was
included in the training dataset.

**Reducing the training data:** Reducing the size of the training dataset or
removing redundant or highly correlated features can help reduce the information
an attacker can gain from a membership inference attack.

**Testing and monitoring:** Regularly testing and monitoring the model's
behavior for anomalies can help detect and prevent membership inference attacks
by detecting when an attacker is attempting to gain access to sensitive
information.

## Risk Factors

|                                                                                                                           Threat Agents/Attack Vectors                                                                                                                            |                                                                                                Security Weakness                                                                                                |                                                                                            Impact                                                                                             |
| :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
|                                                                                        Exploitability: 4 (Moderate) <br/><br/> _ML Application Specific: 5_ <br/> _ML Operations Specific: 3_                                                                                        |                                                                                           Detectability: 3 (Moderate)                                                                                           |                                                                                    Technical: 4 (Moderate)                                                                                    |
| Threat Actors: Hackers or malicious actors who have access to the data and the model. <br/> Insiders who have malicious intent or are bribed to interfere with the data. <br/><br/> Attact Vectors: Unsecured data transmission channels that allow unauthorized access to the data. | Lack of proper data access controls. <br/><br/> Lack of proper data validation and sanitization techniques. <br/><br/> Lack of proper data encryption. <br/><br/> Lack of proper data backup and recovery techniques. | Unreliable or incorrect model predictions. <br/><br/> Loss of confidentiality and privacy of sensitive data. <br/><br/> Legal and regulatory compliance violations. <br/><br/> Reputational damage. |

: {.striped .hover .bordered .responsive }

It is important to note that this chart is only a sample based on
[the scenario below](#ml04_scenario1) only. The actual risk assessment will depend on
the specific circumstances of each machine learning system.

## Example Attack Scenarios

### Scenario \#1: Inferencing financial data from a machine learning model {#ml04_scenario1}

A malicious attacker wants to gain access to sensitive financial information of
individuals. They do this by training a machine learning model on a dataset of
financial records and using it to query whether or not a particular individual's
record was included in the training data. The attacker can then use this
information to infer the financial history and sensitive information of
individuals.

The attacker executed this attack by training a machine learning model on a
dataset of financial records obtained from a financial organization. They then
used this model to query whether or not a particular individual\'s record was
included in the training data, allowing them to infer sensitive financial
information.

## References:
