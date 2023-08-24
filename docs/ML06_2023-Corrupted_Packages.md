---
layout: col-sidebar
type: documentation
altfooter: true
level: 4
auto-migrated: 0
document: OWASP Machine Learning Security Top Ten 2023
year: 2023
order: 6
title: ML06:2023 Corrupted Packages
lang: en
tags:
  [
    OWASP Machine Learning Security Top Ten 2023,
    Top Ten,
    ML06:2023,
    mltop10,
    mlsectop10,
  ]
exploitability: 5
detectability: 5
technical: 4
---

## Description

Corrupted packages attacks occur when an attacker modifies or replaces a machine
learning library or model that is used by a system.

## How to Prevent

**Verify Package Signatures:** Before installing any packages, verify the
digital signatures of the packages to ensure that they have not been tampered
with.

**Use Secure Package Repositories:** Use secure package repositories, such as
Anaconda, that enforce strict security measures and have a vetting process for
packages.

**Keep Packages Up-to-date:** Regularly update all packages to ensure that any
vulnerabilities are patched.

**Use Virtual Environments:** Use virtual environments to isolate packages and
libraries from the rest of the system. This makes it easier to detect any
malicious packages and remove them.

**Perform Code Reviews:** Regularly perform code reviews on all packages and
libraries used in a project to detect any malicious code.

**Use Package Verification Tools:** Use tools such as PEP 476 and Secure Package
Install to verify the authenticity and integrity of packages before
installation.

**Educate Developers:** Educate developers on the risks associated with
Corrupted Packages Attacks and the importance of verifying packages before
installation.

## Risk Factors

|                                                     Threat Agents/Attack Vectors                                                      |           Security Weakness            |                                       Impact                                       |
| :-----------------------------------------------------------------------------------------------------------------------------------: | :------------------------------------: | :--------------------------------------------------------------------------------: |
|                    Exploitability: 5 (Easy) <br><br> _ML Application Specific: 5_ <br> _ML Operations Specific: 3_                    |        Detectability: 5 (Easy)         |                              Technical: 4 (Moderate)                               |
| Threat Actor: Malicious attacker. <br><br> Attack Vector: Modifying code of open-source package used by the machine learning project. | Relying on untrusted third-party code. | Compromise of the machine learning project and potential harm to the organization. |

It is important to note that this chart is only a sample based on
[the scenario below](#scenario1) only. The actual risk assessment will depend on
the specific circumstances of each machine learning system.

## Example Attack Scenarios

### Scenario \#1: Attack on a machine learning project in an organization {#scenario1}

A malicious attacker wants to compromise a machine learning project being
developed by a large organization. The attacker knows that the project relies on
several open-source packages and libraries and wants to find a way to compromise
the project.

The attacker executed the attack by modifying the code of one of the packages
that the project relies on, such as NumPy or Scikit-learn. The attacker then
uploads this modified version of the package to a public repository, such as
PyPI, making it available for others to download and use. When the victim
organization downloads and installs the package, the attacker's malicious code
is also installed and can be used to compromise the project.

This type of attack can be particularly dangerous as it can go unnoticed for a
long time, since the victim may not realize that the package they are using has
been compromised. The attacker's malicious code could be used to steal sensitive
information, modify results, or even cause the machine learning model to fail.

## References
