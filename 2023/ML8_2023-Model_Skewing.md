---

document: OWASP Machine Learning Security Top Ten 2023
year: 2023
order: 6
title: ML8:2023:Model_Skewing
lang: en
author:
contributors:
tags: OWASP Top Ten 2023, Top Ten, ML8:2023
exploitability:
prevalence:
detectability:
technical:
redirect_from:

---


+----------------------+-----------------------+-----------------------+
| Threat agents/Attack | Security Weakness     | Impact                |
| vectors              |                       |                       |
+======================+=======================+=======================+
| ML Exploitability:   | Prevalence: XX,       | Technical: XX         |
| XX                   | Detectability: XX     |                       |
|                      |                       |                       |
| Application /        |                       |                       |
| Operations           |                       |                       |
+----------------------+-----------------------+-----------------------+
|                      |                       |                       |
+----------------------+-----------------------+-----------------------+

Description:

Model skewing attacks occur when an attacker manipulates the
distribution of the training data to cause the model to behave in an
undesirable way.

Example Attack Scenario:

For example, an attacker could oversample certain classes in the
training data to cause the model to be biased towards them.

How to Prevent:

To prevent model skewing attacks, it is important to use diverse and
balanced training data, and to monitor the model\'s behavior during
training.

References:
