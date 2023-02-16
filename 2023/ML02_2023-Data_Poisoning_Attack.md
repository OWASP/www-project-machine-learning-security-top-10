---

document: OWASP Machine Learning Security Top Ten 2023
year: 2023
order: 6
title: ML02:2023:Data_Poisoning_Attack
lang: en
author:
contributors:
tags: OWASP Top Ten 2023, Top Ten, ML02:2023
exploitability: 3
prevalence:
detectability: 2
technical: 4
redirect_from:

---

![ML02-chart](/assets/images/ML02-chart.png)

It is important to note that this chart is only a sample based on
scenario below, and the actual risk assessment will depend on the
specific circumstances of each machine learning system.

**Description:**

Data poisoning attacks occur when an attacker manipulates the training
data to cause the model to behave in an undesirable way.

**Example Attack Scenario:**

Scenario 1: Training a spam classifier

An attacker poisons the training data for a deep learning model that
classifies emails as spam or not spam. The attacker executed this attack
by injecting the maliciously labeled spam emails into the training data
set. This could be done by compromising the data storage system, for
example by hacking into the network or exploiting a vulnerability in the
data storage software. The attacker could also manipulate the data
labeling process, such as by falsifying the labeling of the emails or by
bribing the data labelers to provide incorrect labels.

Scenario 2: Training a network traffic classification system

An attacker poisons the training data for a deep learning model that is
used to classify network traffic into different categories, such as
email, web browsing, and video streaming. They introduce a large number
of examples of network traffic that are incorrectly labeled as a
different type of traffic, causing the model to be trained to classify
this traffic as the incorrect category. As a result, the model may be
trained to make incorrect traffic classifications when the model is
deployed, potentially leading to misallocation of network resources or
degradation of network performance.

**How to Prevent:**

Data validation and verification: Ensure that the training data is
thoroughly validated and verified before it is used to train the model.
This can be done by implementing data validation checks and employing
multiple data labelers to validate the accuracy of the data labeling.

Secure data storage: Store the training data in a secure manner, such as
using encryption, secure data transfer protocols, and firewalls.

Data separation: Separate the training data from the production data to
reduce the risk of compromising the training data.

Access control: Implement access controls to limit who can access the
training data and when they can access it.

Monitoring and auditing: Regularly monitor the training data for any
anomalies and conduct audits to detect any data tampering.

Model validation: Validate the model using a separate validation set
that has not been used during training. This can help to detect any data
poisoning attacks that may have affected the training data.

Model ensembles: Train multiple models using different subsets of the
training data and use an ensemble of these models to make predictions.
This can reduce the impact of data poisoning attacks as the attacker
would need to compromise multiple models to achieve their goals.

Anomaly detection: Use anomaly detection techniques to detect any
abnormal behavior in the training data, such as sudden changes in the
data distribution or data labeling. These techniques can be used to
detect data poisoning attacks early on.

**References:**
