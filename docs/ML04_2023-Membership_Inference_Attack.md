---
layout: col-sidebar
type: documentation
altfooter: true
level: 4
auto-migrated: 0
document: OWASP Machine Learning Security Top Ten 2023
year: 2023
order: 4
title: ML04:2023 Membership Inference Attack
lang: en
tags:
  [
    OWASP Machine Learning Security Top Ten 2023,
    Top Ten,
    ML04:2023,
    mltop10,
    mlsectop10,
  ]
exploitability: 4
detectability: 3
technical: 4
---

## Description

In a membership inference attack, an adversary uses a trained model's behavior
to estimate whether a particular record was in its training set. The adversary
may query a model's predictions for a candidate record and compare the result
with the behavior expected for members and non-members. They do not need to
modify the target model's training data. Learning that a record was used for
training can itself reveal sensitive information, even without recovering the
record's contents.

Attackers can build reference or *shadow* models using data whose membership
they know, then use those models to distinguish members from non-members in the
target model. The attack's reliability depends on the model, the available
outputs and auxiliary information; overfitting can increase leakage, but is not
the only cause. See [Shokri et al. (2017)](https://arxiv.org/abs/1610.05820)
and [Carlini et al. (2022)](https://arxiv.org/abs/2112.03570).

## How to Prevent

**Assess membership leakage:** Evaluate the released model with representative
member and non-member records, including records that may be unusually easy to
identify. Measure attack success at a low false-positive rate rather than
assuming that a well-generalized model is private.

**Limit unnecessary prediction detail:** Consider whether the application needs
to expose confidence scores or only a predicted label. Restricting outputs can
reduce information available to some attacks, but it does not eliminate
membership inference.

**Control overfitting:** Use appropriate regularization and validate performance
on held-out data. These steps may reduce leakage, but generalization alone does
not guarantee membership privacy.

**Use a privacy-preserving training method when required:** Differentially
private training can bound the influence of any one training record. Select and
report an appropriate privacy budget, and account for the effect on model
utility; simply shuffling or reducing the training set does not provide such a
guarantee.

**Review access to the model:** Apply appropriate authentication and rate limits
to prediction APIs, and monitor unusual query patterns. These controls can
raise the cost of repeated queries, but should not be treated as a substitute
for measuring or reducing leakage.

## Risk Factors

|                                                                                                                           Threat Agents/Attack Vectors                                                                                                                            |                                                                                                Security Weakness                                                                                                |                                                                                            Impact                                                                                             |
| :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
|                                                                                        Exploitability: 4 (Moderate) <br><br> _ML Application Specific: 5_ <br> _ML Operations Specific: 3_                                                                                        |                                                                                           Detectability: 3 (Moderate)                                                                                           |                                                                                    Technical: 4 (Moderate)                                                                                    |
| Threat Actors: Anyone able to query the trained model and obtain candidate records; insiders may also have additional model or data access. <br><br> Attack Vectors: Comparing target-model behavior on a candidate record with expected member and non-member behavior. | Model behavior reveals enough information to distinguish training members from non-members. Detailed prediction outputs and overfitting can increase leakage, but neither is required in every attack. | Disclosure that a person or record was included in a sensitive training set. This may reveal participation in a service or other private information, with possible compliance and reputational consequences. |

It is important to note that this chart is only a sample based on
[the scenario below](#scenario1) only. The actual risk assessment will depend on
the specific circumstances of each machine learning system.

## Example Attack Scenarios

### Scenario \#1: Inferencing financial data from a machine learning model {#scenario1}

An organization trains a model on records from customers who received a
particular financial service and exposes a prediction API. An attacker already
has a candidate customer's record but does not know whether that customer used
the service. By querying the **organization's model** with that record and
comparing its response with member and non-member behavior learned from
reference models, the attacker estimates whether the customer was in the
training set. A successful inference reveals participation in the service; it
does not, by itself, recover the customer's full financial history.

**References:**

- Shokri et al., [Membership Inference Attacks Against Machine Learning Models](https://arxiv.org/abs/1610.05820), IEEE Symposium on Security and Privacy, 2017.
- Carlini et al., [Membership Inference Attacks From First Principles](https://arxiv.org/abs/2112.03570), IEEE Symposium on Security and Privacy, 2022.
