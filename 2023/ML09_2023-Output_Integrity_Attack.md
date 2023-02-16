---

document: OWASP Machine Learning Security Top Ten 2023
year: 2023
order: 6
title: ML09:2023:Output_Integrity_Attack
lang: en
author:
contributors:
tags: OWASP Top Ten 2023, Top Ten, ML09:2023
exploitability: 5
prevalence:
detectability: 3
technical: 3
redirect_from:

---

![ML09-chart](/assets/images/ML09-chart.png)


It is important to note that this chart is only a sample based on
scenario below, and the actual risk assessment will depend on the
specific circumstances of each machine learning system.

**Description:**

In an Output Integrity Attack scenario, an attacker aims to modify or
manipulate the output of a machine learning model in order to change its
behavior or cause harm to the system it is used in.

**Example Attack Scenario:**

An attacker has gained access to the output of a machine learning model
that is being used to diagnose diseases in a hospital. The attacker
modifies the output of the model, making it provide incorrect diagnoses
for patients. As a result, patients are given incorrect treatments,
leading to further harm and potentially even death.

**How to Prevent:**

Using cryptographic methods: Cryptographic methods like digital
signatures and secure hashes can be used to verify the authenticity of
the results.

Secure communication channels: Communication channels between the model
and the interface responsible for displaying the results should be
secured using secure protocols such as SSL/TLS.

Input Validation: Input validation should be performed on the results to
check for unexpected or manipulated values.

Tamper-evident logs: Maintaining tamper-evident logs of all input and
output interactions can help detect and respond to any output integrity
attacks.

Regular software updates: Regular software updates to fix
vulnerabilities and security patches can help reduce the risk of output
integrity attacks.

Monitoring and auditing: Regular monitoring and auditing of the results
and the interactions between the model and the interface can help detect
any suspicious activities and respond accordingly.

**[References]{.underline}**:
