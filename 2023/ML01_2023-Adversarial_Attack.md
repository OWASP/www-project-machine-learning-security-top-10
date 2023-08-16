---
layout: col-sidebar
type: documentation
altfooter: true
level: 4
auto-migrated: 0
document: OWASP Machine Learning Security Top Ten 2023
year: 2023
order: 1
title: ML01:2023 Adversarial Attack
lang: en
tags:
  [
    OWASP Machine Learning Security Top Ten 2023,
    Top Ten,
    ML01:2023,
    mltop10,
    mlsectop10,
  ]
exploitability: 5
detectability: 3
technical: 5
---

## Description

Adversarial attacks are a type of attack in which an attacker deliberately
alters input data to mislead the model.

## How to Prevent

**Adversarial training:** One approach to defending against adversarial attacks
is to train the model on adversarial examples. This can help the model become
more robust to attacks and reduce its susceptibility to being misled.

**Robust models:** Another approach is to use models that are designed to be
robust against adversarial attacks, such as adversarial training or models that
incorporate defense mechanisms.

**Input validation:** Input validation is another important defense mechanism
that can be used to detect and prevent adversarial attacks. This involves
checking the input data for anomalies, such as unexpected values or patterns,
and rejecting inputs that are likely to be malicious.

## Risk Factors

| Threat Agents/Attack Vectors                                                                                                                                                                  |                                                               Security Weakness                                                                |                                                            Impact                                                             |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------------------------------------: |
| Exploitability: 5 (Easy) <br><br> _ML Application Specific: 4_ <br> _ML Operations Specific: 3_                                                                                               | Detectability: 3 (Moderate) <br><br> _The adversarial image may not be noticeable to the naked eye, making it difficult to detect the attack._ | Technical: 5 (Difficult) <br><br> _The attack requires technical knowledge of deep learning and image processing techniques._ |
| Threat Agent: Attacker with knowledge of deep learning and image processing techniques. <br><br> Attack Vector: Deliberately crafted adversarial image that is similar to a legitimate image. |                               Vulnerability in the deep learning model's ability to classify images accurately.                                |                       Misclassification of the image, leading to security bypass or harm to the system.                       |

It is important to note that this chart is only a sample based on
[the scenario below](#scenario1) only. The actual risk assessment will depend on
the specific circumstances of each machine learning system.

## Example Attack Scenarios

### Scenario \#1: Image classification {#scenario1}

A deep learning model is trained to classify images into different categories,
such as dogs and cats. An attacker creates an adversarial image that is very
similar to a legitimate image of a cat, but with small, carefully crafted
perturbations that cause the model to misclassify it as a dog. When the model is
deployed in a real-world setting, the attacker can use the adversarial image to
bypass security measures or cause harm to the system.

### Scenario \#2: Network intrusion detection

A deep learning model is trained to detect intrusions in a network. An attacker
creates adversarial network traffic by carefully crafting packets in such a way
that they will evade the model\'s intrusion detection system. The attacker can
manipulate the features of the network traffic, such as the source IP address,
destination IP address, or payload, in such a way that they are not detected by
the intrusion detection system. For example, the attacker may hide their source
IP address behind a proxy server or encrypt the payload of their network
traffic. This type of attack can have serious consequences, as it can lead to
data theft, system compromise, or other forms of damage.

## References
