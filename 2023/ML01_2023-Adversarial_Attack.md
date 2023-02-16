---

document: OWASP Machine Learning Security Top Ten 2023
year: 2023
order: 6
title: ML01:2023:Adversarial_Attack
lang: en
author:
contributors:
tags: OWASP Top Ten 2023, Top Ten, ML01:2023
exploitability: 5
prevalence:
detectability: 3
technical: 5
redirect_from:

---

RISK Chart for Scenario One:

![/assets/images/ML01-chart.png]

It is important to note that this chart is only a sample based on
scenario below, and the actual risk assessment will depend on the
specific circumstances of each machine learning system.

**Description**:
Adversarial attacks are a type of attack in which an attacker
deliberately alters input data to mislead the model.

**Example Attack Scenario:**

Scenario 1: Image classification

A deep learning model is trained to classify images into different
categories, such as dogs and cats. An attacker creates an adversarial
image that is very similar to a legitimate image of a cat, but with
small, carefully crafted perturbations that cause the model to
misclassify it as a dog. When the model is deployed in a real-world
setting, the attacker can use the adversarial image to bypass security
measures or cause harm to the system.

Scenario 2: Network intrusion detection

A deep learning model is trained to detect intrusions in a network. An
attacker creates adversarial network traffic by carefully crafting
packets in such a way that they will evade the model\'s intrusion
detection system. The attacker can manipulate the features of the
network traffic, such as the source IP address, destination IP address,
or payload, in such a way that they are not detected by the intrusion
detection system. For example, the attacker may hide their source IP
address behind a proxy server or encrypt the payload of their network
traffic. This type of attack can have serious consequences, as it can
lead to data theft, system compromise, or other forms of damage.

**How to Prevent:**

1. Adversarial training: One approach to defending against adversarial
    attacks is to train the model on adversarial examples. This can help
    the model become more robust to attacks and reduce its
    susceptibility to being misled.

2. Robust models: Another approach is to use models that are designed
    to be robust against adversarial attacks, such as adversarial
    training or models that incorporate defense mechanisms.

3. Input validation: Input validation is another important defense
    mechanism that can be used to detect and prevent adversarial
    attacks. This involves checking the input data for anomalies, such
    as unexpected values or patterns, and rejecting inputs that are
    likely to be malicious.

**References:**
