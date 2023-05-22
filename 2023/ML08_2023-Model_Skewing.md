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

|                                                                                                                          Threat agents/Attack vectors                                                                                                                          |                                                                                                                                            Security Weakness                                                                                                                                           |                                                                                                                                                               Impact                                                                                                                                                               |
|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
| Exploitability: 5 (Easy)<br>ML Application Specific: 4<br>the attacker has a clear understanding of the machine learning project and its vulnerabilities.<br>ML Operations Specific: 3<br>manipulation of the training data requires knowledge of the machine learning process |                                                                                                      Detectability: 2<br>the model skewing might not be easily noticeable during the testing phase                                                                                                     |                                                                                                                          Technical: 4 <br>manipulation of the training data is a technically complex task                                                                                                                          |
| The attackers in a Model Skewing attack could be individuals with malicious intent, or a third-party with a vested interest in manipulating the outcomes of a model.                                                                                                           | The security weakness in a Model Skewing attack is the inability of the model to accurately reflect the underlying distribution of the training data. This can occur due to factors such as data bias, incorrect sampling of the data, or manipulation of the data or training process by an attacker. | The impact of a Model Skewing attack can be significant and can lead to incorrect decisions being made based on the output of the model. This can result in financial loss, damage to reputation, and even harm to individuals if the model is being used for critical applications such as medical diagnosis or criminal justice. |


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
