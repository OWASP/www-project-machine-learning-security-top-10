---
layout: col-sidebar
type: documentation
altfooter: true
level: 4
auto-migrated: 0
document: OWASP Machine Learning Security Top Ten 2023
year: 2023
order: 7
title: ML07:2023 Transfer Learning Attack
lang: en
tags:
  [
    OWASP Machine Learning Security Top Ten 2023,
    Top Ten,
    ML07:2023,
    mltop10,
    mlsectop10,
  ]
exploitability: 5
detectability: 1
technical: 5
---

## Description

Transfer learning attacks occur when an attacker trains a model on one task and
then fine-tunes it on another task to cause it to behave in an undesirable way.

## How to Prevent

**Regularly monitor and update the training datasets:** Regularly monitoring and
updating the training datasets can help prevent the transfer of malicious
knowledge from the attacker\'s model to the target model.

**Use secure and trusted training datasets:** Using secure and trusted training
datasets can help prevent the transfer of malicious knowledge from the
attacker's model to the target model.

**Implement model isolation:** Implementing model isolation can help prevent the
transfer of malicious knowledge from one model to another. For example,
separating the training and deployment environments can prevent attackers from
transferring knowledge from the training environment to the deployment
environment.

**Use differential privacy:** Using differential privacy can help protect the
privacy of individual records in the training dataset and prevent the transfer
of malicious knowledge from the attacker's model to the target model.

**Perform regular security audits:** Regular security audits can help identify
and prevent transfer learning attacks by identifying and addressing
vulnerabilities in the system.

## Risk Factors

|                                                                                                                                                             Threat Agents/Attack Vectors                                                                                                                                                             |                                                                                                                    Security Weakness                                                                                                                    |                                                                                                                       Impact                                                                                                                       |
| :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
| Exploitability: 5 (Easy) <br><br> _ML Application Specific: 4_ <br>The attack specifically targets the machine learning application and can cause significant harm to the model and the organization. <br><br> _ML Operations Specific: 3_ <br> The attack requires knowledge of machine learning operations but can be executed with relative ease. |                                Detectability: 1 (Difficult) <br><br> _The attack may be difficult to detect as the results produced by the compromised model may appear to be correct and consistent with expectations._                                |                    Technical: 5 (Difficult) <br><br> _The attack requires a high level of technical expertise in machine learning and a willingness to compromise the integrity of the training dataset or pre-trained models._                    |
|                                                                                             Threat Actor: Malicious actor. <br><br> Attack Vector: Attacker with knowledge of machine learning and access to the training dataset or pre-trained models.                                                                                             | Lack of proper data protection measures for the training dataset and pre-trained models. <br><br> Insecure storage and sharing of pre-trained models. <br><br> Lack of proper data protection measures for the pre-trained models and training dataset. | Misleading or incorrect results from the machine learning model. <br><br> Confidentiality breach of sensitive information in the training dataset. <br><br> Reputational harm to the organization. <br><br> Legal or regulatory compliance issues. |

It is important to note that this chart is only a sample based on
[the scenario below](#scenario1) only. The actual risk assessment will depend on
the specific circumstances of each machine learning system.

## Example Attack Scenarios

### Scenario \#1: Training a model on a malicious dataset {#scenario1}

An attacker trains a machine learning model on a malicious dataset that contains
manipulated images of faces. The attacker wants to target a face recognition
system used by a security firm for identity verification.

The attacker then transfers the model's knowledge to the target face recognition
system. The target system starts using the attacker's manipulated model for
identity verification.

As a result, the face recognition system starts making incorrect predictions,
allowing the attacker to bypass the security and gain access to sensitive
information. For example, the attacker could use a manipulated image of
themselves and the system would identify them as a legitimate user.

## References
