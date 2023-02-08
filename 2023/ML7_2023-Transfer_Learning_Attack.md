---

document: OWASP Machine Learning Security Top Ten 2023
year: 2023
order: 6
title: ML7:2023:Transfer_Learning_Attack
lang: en
author:
contributors:
tags: OWASP Top Ten 2023, Top Ten, ML7:2023
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

Transfer learning attacks occur when an attacker trains a model on one
task and then fine-tunes it on another task to cause it to behave in an
undesirable way.

Example Attack Scenario:

For instance, an attacker could train a model on a benign task and then
fine-tune it on a malicious task to cause it to produce incorrect
predictions.

How to Prevent:

To prevent transfer learning attacks, it is important to monitor the
model\'s behavior during fine-tuning and to validate its predictions.

References:
