---
layout: col-sidebar
type: documentation
altfooter: true
level: 4
auto-migrated: 0
document: OWASP Machine Learning Security Top Ten 2023
year: 2023
order: 6
title: ML06:2023 AI Supply Chain Attacks
lang: en
tags:
  [
    OWASP Machine Learning Security Top Ten 2023,
    Top Ten,
    ML06:2023,
    mltop10,
    mlsectop10,
  ]
exploitability: 6
detectability: 5
technical: 4
---

## Description

In AI Supply Chain Attacks threat actors target the supply chain of ML/AI models. This category is broad and important, as software supply chain in Machine Learning and AI includes even more elements than in the case of classic software. It consists of specific elements such as MLOps platforms, data management platforms, model management software, model hubs and other specialized types of software that enable ML engineers to effectively test and deploy software.

## How to Prevent

**Verify packages integrity:** Before using any packages in your infrastructure or application dependencies, verify the authenticity of the package by checking the digital signature of the package.

**Keep packages versions up-to-date:** Constantly monitor the latest versions of the packages in your software supply chain and update your dependencies if you are using outdated software. Use tools such as OWASP Dependency Check. Refer to [https://owasp.org/Top10/A06_2021-Vulnerable_and_Outdated_Components/](OWASP Top10 A06:2021 – Vulnerable and Outdated Components) for more details

**Install packages from secure sources:** Use secure third-party software repositiories, such as
Anaconda or pip, that enforce strict security measures and have a vetting process for
packages.

**Deploy ML infrastructure securely:** Follow the vendor's deployment recommendations for MLOps platforms in your stack, limit the access to the web UIs from the Internet, monitor the traffic in the infrastructure for the anomalies and possible attacks. If the infrastructure is deployed in the cloud, ensure to leverage the cloud provider's security features such as Virtual Private Clouds (VPCs), security groups, and identity and access management (IAM) roles to restrict and control access. Implement strict access control measures. Ensure that only authorized personnel have access to the MLOps platforms.

## Risk Factors

|                                                     Threat Agents/Attack Vectors                                                      |           Security Weakness            |                                       Impact                                       |
| :-----------------------------------------------------------------------------------------------------------------------------------: | :------------------------------------: | :--------------------------------------------------------------------------------: |
|                    Exploitability: 4 (Easy) <br><br> _ML Application Specific: 5_ <br> _ML Operations Specific: 3_                    |        Detectability: 5 (Easy)         |                              Technical: 5 (Moderate)                               |
| Threat Actor: Cybercrime groups; malicious business competitors. <br><br> Attack Vector: Modifying code of open-source package used by the machine learning project. Exploiting the vulnrability in the MLOps stack. | Relying on untrusted or insecure third-party code or software. | Compromise of the machine learning infrastructure and potential harm to the organization. |

It is important to note that this chart is only a sample based on
[the scenarios below](#scenario1) only. The actual risk assessment will depend on
the specific circumstances of each machine learning system.

## Example Attack Scenarios

### Scenario \#1: Attack on a Machine Learning project dependency {#scenario1}

The attacker, that wants to compromise a Machine Learning project, knows that the project relies on several open-source packages and libraries.

During the attack, they modify the code of one of the packages that the project relies on, such as NumPy or Scikit-learn. The modified version of the package is then uploaded to a public repository, such as PyPI, making it available for others to download and use. When the victim organization downloads and installs the package, the malicious code is also installed and can be used to compromise the project.

This type of attack can be particularly dangerous as it can go unnoticed for a long time, since the victim may not realize that the package they are using has been compromised. The attacker's malicious code can be used to steal sensitive information, modify results, or lead the machine learning model to return erroneous predictions.

The attacker targets a Machine Learning project that relies on several open-source packages and libraries.


### Scenario \#2: Attack on a MLOps software used in the organization {#scenario2}

Organization builds a MLOps pipeline that uses multiple instances of the software supporting the deployment. One of the applications, which is an inference platform, is exposed publicly to the Internet.

An attacker finds a web interface of the plaftorm available without authentication and gets access to the models, which weren't meant to be exposed publicly.

### Scenario \#3: Attack on a ML model hub used by the organization {#scenario3}

An organization decides to use a model from the public model hub. An attacker finds a way to impersonate the organization account in the model hub and then deploys malicious model to the model hub. The organization employees then download the malicious model and the malicious code is ran in the organization's environment.

## References

[https://owasp.org/Top10/A06_2021-Vulnerable_and_Outdated_Components/](OWASP Top10 A06:2021 – Vulnerable and Outdated Components)
[https://5stars217.github.io/2023-08-08-red-teaming-with-ml-models/](Model Confusion - Weaponizing ML models for red teams and bounty hunters)
