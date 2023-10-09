---
layout: col-sidebar
type: documentation
altfooter: true
level: 4
auto-migrated: 0
document: OWASP Machine Learning Security Top Ten 2023
year: 2023
order: 3
title: ML03:2023 Model Inversion Attack
lang: en
tags:
  [
    OWASP Machine Learning Security Top Ten 2023,
    Top Ten,
    ML03:2023,
    mltop10,
    mlsectop10,
  ]
exploitability: 4
detectability: 2
technical: 4
---

## Description

Model inversion attacks occur when an attacker reverse-engineers the model to
extract information from it.

## How to Prevent

**Access control:** Limiting access to the model or its predictions can prevent
attackers from obtaining the information needed to invert the model. This can be
done by requiring authentication, encryption, or other forms of security when
accessing the model or its predictions.

**Input validation:** Validating the inputs to the model can prevent attackers
from providing malicious data that can be used to invert the model. This can be
done by checking the format, range, and consistency of the inputs before they
are processed by the model.

**Model transparency:** Making the model and its predictions transparent can
help to detect and prevent model inversion attacks. This can be done by logging
all inputs and outputs, providing explanations for the model's predictions, or
allowing users to inspect the model's internal representations.

**Regular monitoring:** Monitoring the model's predictions for anomalies can
help to detect and prevent model inversion attacks. This can be done by tracking
the distribution of inputs and outputs, comparing the model's predictions to
ground truth data, or monitoring the model's performance over time.

**Model retraining:** Regularly retraining the model can help to prevent the
information leaked by model inversion attacks from becoming outdated. This can
be done by incorporating new data and correcting any inaccuracies in the model's
predictions.

## Risk Factors

|                                                                    Threat Agents/Attack Vectors                                                                     |                                Security Weakness                                |                              Impact                               |
| :----------------------------------------------------------------------------------------------------------------------------------------------------------------- | :----------------------------------------------------------------------------- | :--------------------------------------------------------------- |
|                                 Exploitability: 4 (Moderate) <br/><br/> _ML Application Specific: 5_ <br/> _ML Operations Specific: 3_                                 |                          Detectability: 2 (Difficult)                           |                      Technical: 4 (Moderate)                      |
| Threat Agents: Attackers who have access to the model and input data. <br/><br/> Attack Vectors: Submitting an image to the model and analyzing the model's response. | Model's output can be used to infer sensitive information about the input data. | Confidential information about the input data can be compromised. |

: {.striped .hover .bordered .responsive }

It is important to note that this chart is only a sample based on
[the scenario below](#ml03_scenario1) only. The actual risk assessment will depend on
the specific circumstances of each machine learning system.

## Example Attack Scenarios

### Scenario \#1: Stealing personal information from a face recognition model {#ml03_scenario1}

An attacker trains a deep learning model to perform face recognition. They then
use this model to perform a model inversion attack on a different face
recognition model that is used by a company or organization. The attacker inputs
images of individuals into the model and recovers the personal information of
the individuals from the model\'s predictions, such as their name, address, or
social security number.

The attacker executed this attack by training the model to perform face
recognition and then using this model to invert the predictions of another face
recognition model. This could be done by exploiting a vulnerability in the
model\'s implementation or by accessing the model through an API. The attacker
would then be able to recover the personal information of the individuals from
the model\'s predictions.

### Scenario \#2: Bypassing a bot detection model in online advertising

An advertiser wants to automate their advertising campaigns by using bots to
perform actions such as clicking on ads and visiting websites. However, online
advertising platforms use bot detection models to prevent bots from performing
these actions. To bypass these models, the advertiser trains a deep learning
model for bot detection and uses it to invert the predictions of the bot
detection model used by the online advertising platform. The advertiser inputs
their bots into the model and is able to make the bots appear as human users,
allowing them to bypass the bot detection and successfully execute their
automated advertising campaigns.

The advertiser executed this attack by training their own bot detection model
and then using it to reverse the predictions of the bot detection model used by
the online advertising platform. They were able to access this other model
through a vulnerability in its implementation or by using an API. The end result
of the attack was the advertiser successfully automating their advertising
campaigns by making their bots appear as human users.

## References
