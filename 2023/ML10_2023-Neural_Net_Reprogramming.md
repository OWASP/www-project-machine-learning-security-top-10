---

document: OWASP Machine Learning Security Top Ten 2023
year: 2023
order: 6
title: ML10:2023:Neural_Net_Reprogramming
lang: en
author:
contributors:
tags: OWASP Top Ten 2023, Top Ten, ML10:2023
exploitability: 4
prevalence:
detectability: 3
technical: 3
redirect_from:

---

![ML10-chart](/assets/images/ML10-chart.png)


It is important to note that this chart is only a sample based on
scenario below, and the actual risk assessment will depend on the
specific circumstances of each machine learning system.

**Description:**

Neural net reprogramming attacks occur when an attacker manipulates the
model\'s parameters to cause it to behave in an undesirable way.

**Example Attack Scenario:**

Consider a scenario where a bank is using a machine learning model to
identify handwritten characters on cheques to automate their clearing
process. The model has been trained on a large dataset of handwritten
characters, and it has been designed to accurately identify the
characters based on specific parameters such as size, shape, slant, and
spacing.

An attacker who wants to exploit the Neural Net Reprogramming attack may
manipulate the parameters of the model by altering the images in the
training dataset or directly modifying the parameters in the model. This
can result in the model being reprogrammed to identify characters
differently. For example, the attacker could change the parameters so
that the model identifies the character "5" as the character "2",
leading to incorrect amounts being processed.

The attacker can exploit this vulnerability by introducing forged
cheques into the clearing process, which the model will process as valid
due to the manipulated parameters. This can result in significant
financial loss to the bank.

**How to Prevent:**

Regularization: Adding regularization techniques like L1 or L2
regularization to the loss function helps to prevent overfitting and
reduce the chance of neural net reprogramming attacks.

Robust Model Design: Designing models with robust architectures and
activation functions can help reduce the chances of successful
reprogramming attacks.

Cryptographic Techniques: Cryptographic techniques can be used to secure
the parameters and weights of the model, and prevent unauthorized access
or manipulation of these parameters.

**References:**
