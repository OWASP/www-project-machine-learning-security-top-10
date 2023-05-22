---
layout: col-sidebar
title: OWASP Machine Learning Security Top Ten
type: documentation
altfooter: true
level: 4
auto-migrated: 0
pitch:
document: OWASP Machine Learning Security Top Ten 2023
year: 2023
order: 6
title: ML07:2023:Transfer_Learning_Attack
lang: en
author:
contributors:
tags: OWASP Top Ten 2023, Top Ten, ML07:2023, mltop10
exploitability: 4
prevalence:
detectability: 2
technical: 4
redirect_from:
---

|                                                                                                                                                   Threat agents/Attack vectors                                                                                                                                                   |                                                                                                            Security Weakness                                                                                                             |                                                                                                            Impact                                                                                                            |
| :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
| Exploitability: 4 (Easy)<br>ML Application Specific: 4<br>The attack specifically targets the machine learning application and can cause significant harm to the model and the organization <br>ML Operations Specific: 3<br>The attack requires knowledge of machine learning operations but can be executed with relative ease |                                   Detectability: 2<br>The attack may be difficult to detect as the results produced by the compromised model may appear to be correct and consistent with expectations                                   |                Technical: 4 <br>The attack requires a high level of technical expertise in machine learning and a willingness to compromise the integrity of the training dataset or pre-trained models.<br>                 |
|                                                                                                               Attacker with knowledge of machine learning and access to the training dataset or pre-trained models                                                                                                               | Lack of proper data protection measures for the training dataset and pre-trained models<br>Insecure storage and sharing of pre-trained models<br>Lack of proper data protection measures for the pre-trained models and training dataset | Misleading or incorrect results from the machine learning model<br>Confidentiality breach of sensitive information in the training dataset<br>Reputational harm to the organization<br>Legal or regulatory compliance issues |

It is important to note that this chart is only a sample based on
scenario below, and the actual risk assessment will depend on the
specific circumstances of each machine learning system.

**Description:**

Transfer learning attacks occur when an attacker trains a model on one
task and then fine-tunes it on another task to cause it to behave in an
undesirable way.

**Example Attack Scenario:**

An attacker trains a machine learning model on a malicious dataset that
contains manipulated images of faces. The attacker wants to target a
face recognition system used by a security firm for identity
verification.

The attacker then transfers the model's knowledge to the target face
recognition system. The target system starts using the attacker's
manipulated model for identity verification.

As a result, the face recognition system starts making incorrect
predictions, allowing the attacker to bypass the security and gain
access to sensitive information. For example, the attacker could use a
manipulated image of themselves and the system would identify them as a
legitimate user.

**[How to Prevent:]{.underline}**

Regularly monitor and update the training datasets: Regularly monitoring
and updating the training datasets can help prevent the transfer of
malicious knowledge from the attacker\'s model to the target model.

Use secure and trusted training datasets: Using secure and trusted
training datasets can help prevent the transfer of malicious knowledge
from the attacker\'s model to the target model.

Implement model isolation: Implementing model isolation can help prevent
the transfer of malicious knowledge from one model to another. For
example, separating the training and deployment environments can prevent
attackers from transferring knowledge from the training environment to
the deployment environment.

Use differential privacy: Using differential privacy can help protect
the privacy of individual records in the training dataset and prevent
the transfer of malicious knowledge from the attacker's model to the
target model.

Perform regular security audits: Regular security audits can help
identify and prevent transfer learning attacks by identifying and
addressing vulnerabilities in the system.

**References:**
