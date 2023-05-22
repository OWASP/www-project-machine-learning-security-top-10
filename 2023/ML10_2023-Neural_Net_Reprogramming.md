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
title: ML10:2023:Neural_Net_Reprogramming
lang: en
author:
contributors:
tags: OWASP Top Ten 2023, Top Ten, ML10:2023
exploitability: 4
prevalence:
detectability: 3
technical: 3
redirect_from:

---

|                                                                               Threat agents/Attack vectors                                                                               |                                                                          Security Weakness                                                                         |                                                                                                                                     Impact                                                                                                                                    |
|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
|                                                 Exploitability: 4 (Easy)<br>ML Application Specific: 4<br>ML Operations Specific: 4<br>                                                  |                                                                        Detectability: 3<br>                                                                        |                                                                                                                               Technical: 3<br>                                                                                                                                |
| Malicious individuals or organizations with knowledge and resources to manipulate deep learning models.<br>Malicious insiders within the organization developing the deep learning model | Insufficient access controls to the model's code and parameters<br>Lack of proper secure coding practices<br>Inadequate monitoring and logging of model's activity | Model's predictions can be manipulated to achieve desired results.<br>Confidential information within the model can be extracted.<br>Decisions based on the model's predictions can be impacted negatively.<br>Reputation and credibility of the organization can be affected |


It is important to note that this chart is only a sample based on
scenario below, and the actual risk assessment will depend on the
specific circumstances of each machine learning system.

**Description:**

Neural net reprogramming attacks occur when an attacker manipulates the
model\'s parameters to cause it to behave in an undesirable way.

**Example Attack Scenario:**

Consider a scenario where a bank is using a machine learning model to
identify handwritten characters on cheques to automate their clearing
process. The model has been trained on a large dataset of handwritten
characters, and it has been designed to accurately identify the
characters based on specific parameters such as size, shape, slant, and
spacing.

An attacker who wants to exploit the Neural Net Reprogramming attack may
manipulate the parameters of the model by altering the images in the
training dataset or directly modifying the parameters in the model. This
can result in the model being reprogrammed to identify characters
differently. For example, the attacker could change the parameters so
that the model identifies the character "5" as the character "2",
leading to incorrect amounts being processed.

The attacker can exploit this vulnerability by introducing forged
cheques into the clearing process, which the model will process as valid
due to the manipulated parameters. This can result in significant
financial loss to the bank.

**How to Prevent:**

Regularization: Adding regularization techniques like L1 or L2
regularization to the loss function helps to prevent overfitting and
reduce the chance of neural net reprogramming attacks.

Robust Model Design: Designing models with robust architectures and
activation functions can help reduce the chances of successful
reprogramming attacks.

Cryptographic Techniques: Cryptographic techniques can be used to secure
the parameters and weights of the model, and prevent unauthorized access
or manipulation of these parameters.

**References:**
