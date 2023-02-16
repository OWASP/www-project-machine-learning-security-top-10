---

document: OWASP Machine Learning Security Top Ten 2023
year: 2023
order: 6
title: ML07:2023:Transfer_Learning_Attack
lang: en
author:
contributors:
tags: OWASP Top Ten 2023, Top Ten, ML07:2023
exploitability: 4
prevalence:
detectability: 2
technical: 4
redirect_from:

---

![ML07-chart](/assets/images/ML07-chart.png)


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
