---

document: OWASP Machine Learning Security Top Ten 2023
year: 2023
order: 6
title: ML03:2023:Model_Inversion_Attack
lang: en
author:
contributors:
tags: OWASP Top Ten 2023, Top Ten, ML03:2023
exploitability:
prevalence:
detectability:
technical:
redirect_from:

---


Description:

Model inversion attacks occur when an attacker reverse-engineers the
model to extract information from it.

Example Attack Scenario:

For example, an attacker could use a model trained on facial recognition
data to reconstruct an image of a person\'s face from their feature
representations.

How to Prevent:

To prevent model inversion attacks, it is important to use models that
are designed to be robust against inversion and to secure the model\'s
parameters.

References:
