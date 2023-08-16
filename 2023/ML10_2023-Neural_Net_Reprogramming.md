---
layout: col-sidebar
type: documentation
altfooter: true
level: 4
auto-migrated: 0
document: OWASP Machine Learning Security Top Ten 2023
year: 2023
order: 10
title: ML10:2023 Neural Net Reprogramming
lang: en
tags: OWASP Machine Learning Security Top Ten 2023, Top Ten, ML10:2023, mltop10, mlsectop10
exploitability: 5
detectability: 3
technical: 3
---

## Description

Neural net reprogramming attacks occur when an attacker manipulates the model\'s
parameters to cause it to behave in an undesirable way.

## How to Prevent

**Regularisation:** Adding regularisation techniques like L1 or L2
regularization to the loss function helps to prevent overfitting and reduce the
chance of neural net reprogramming attacks.

**Robust Model Design:** Designing models with robust architectures and
activation functions can help reduce the chances of successful reprogramming
attacks.

**Cryptographic Techniques:** Cryptographic techniques can be used to secure the
parameters and weights of the model, and prevent unauthorized access or
manipulation of these parameters.

## Risk Factors

|                                                                                       Threat Agents/Attack Vectors                                                                                        |                                                                                 Security Weakness                                                                                 |                                                                                                                                             Impact                                                                                                                                              |
| :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
|                                                      Exploitability: 5 (Easy) <br><br> _ML Application Specific: 4_ <br> _ML Operations Specific: 4_                                                      |                                                                            Detectability: 3 (Moderate)                                                                            |                                                                                                                                     Technical: 3 (Moderate)                                                                                                                                     |
| Threat Actor: Malicious individuals or organizations with knowledge and resources to manipulate deep learning models. <br> Malicious insiders within the organization developing the deep learning model. | Insufficient access controls to the model's code and parameters. <br><br> Lack of proper secure coding practices. <br><br> Inadequate monitoring and logging of model's activity. | Model's predictions can be manipulated to achieve desired results. <br><br>Confidential information within the model can be extracted. <br><br> Decisions based on the model's predictions can be impacted negatively. <br><br> Reputation and credibility of the organization can be affected. |

It is important to note that this chart is only a sample based on
[the scenario below](#scenario1) only. The actual risk assessment will depend on
the specific circumstances of each machine learning system.

## Example Attack Scenarios

### Scenario \#1: Financial gain through neural net reprogramming {#scenario1}

Consider a scenario where a bank is using a machine learning model to identify
handwritten characters on cheques to automate their clearing process. The model
has been trained on a large dataset of handwritten characters, and it has been
designed to accurately identify the characters based on specific parameters such
as size, shape, slant, and spacing.

An attacker who wants to exploit the Neural Net Reprogramming attack may
manipulate the parameters of the model by altering the images in the training
dataset or directly modifying the parameters in the model. This can result in
the model being reprogrammed to identify characters differently. For example,
the attacker could change the parameters so that the model identifies the
character "5" as the character "2", leading to incorrect amounts being
processed.

The attacker can exploit this vulnerability by introducing forged cheques into
the clearing process, which the model will process as valid due to the
manipulated parameters. This can result in significant financial loss to the
bank.

## References
