---

document: OWASP Machine Learning Security Top Ten 2023
year: 2023
order: 6
title: ML08:2023:Model_Skewing
lang: en
author:
contributors:
tags: OWASP Top Ten 2023, Top Ten, ML08:2023
exploitability: 5
prevalence:
detectability: 2
technical: 4
redirect_from:

---

![ML08-chart](/assets/images/ML08-chart.png)


It is important to note that this chart is only a sample based on
scenario below, and the actual risk assessment will depend on the
specific circumstances of each machine learning system.

**Description:**

Model skewing attacks occur when an attacker manipulates the
distribution of the training data to cause the model to behave in an
undesirable way.

**Example Attack Scenario:**

A financial institution is using a machine learning model to predict the
creditworthiness of loan applicants, and the model's predictions are
integrated into their loan approval process. An attacker wants to
increase their chances of getting a loan approved, so they manipulate
the feedback loop in the MLOps system. The attacker provides fake
feedback data to the system, indicating that high-risk applicants have
been approved for loans in the past, and this feedback is used to update
the model's training data. As a result, the model's predictions are
skewed towards low-risk applicants, and the attacker's chances of
getting a loan approved are significantly increased.

This type of attack can compromise the accuracy and fairness of the
model, leading to unintended consequences and potential harm to the
financial institution and its customers.

**How to Prevent:**

Implement robust access controls: Ensure that only authorized personnel
have access to the MLOps system and its feedback loops, and that all
activities are logged and audited.

Verify the authenticity of feedback data: Use techniques such as digital
signatures and checksums to verify that the feedback data received by
the system is genuine, and reject any data that does not match the
expected format.

Use data validation and cleaning techniques: Clean and validate the
feedback data before using it to update the training data, to minimize
the risk of incorrect or malicious data being used.

Implement anomaly detection: Use techniques such as statistical and
machine learning-based methods to detect and alert on anomalies in the
feedback data, which could indicate an attack.

Regularly monitor the model's performance: Continuously monitor the
performance of the model, and compare its predictions with actual
outcomes to detect any deviation or skewing.

Continuously train the model: Regularly retrain the model using updated
and verified training data, to ensure that it continues to reflect the
latest information and trends.

**References:**
