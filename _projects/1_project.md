---
layout: page
title: trustworthy machine learning
#description: with background image
img: assets/img/1.jpg
importance: 1
category: work
related_publications: true
---

Machine learning (ML) systems are anticipated to become embedded into various aspects of daily life, including health care, financial transactions, and transportation systems. As a result, they will present prime targets for attackers. ML systems are known to be susceptible to a range of attacks, including data and model poisoning, backdoor, privacy leakage, and adversarial inputs among others.

Real-world machine learning systems often require several guarantees to be met at the same time such as privacy and robustness. For example, a federated learning system should protect the privacy of individual client updates which can leak information about their datasets, and also protect against malicious clients who aim to poison the model with malicious updates. In our work zPROBE {% cite ghodsi2023zprobe %}, we propose a private and robust federated learning framework which utilizes zero-knowledge proofs to provide robustness guarantees without compromising client privacy.

Integrity or correctness guarantees for machine learning computations are also important in increasingly common scenarios where operations are outsourced to commercial vendors instead of performed locally due to lack of sufficient computational resources. A vendor has a financial incentive to replace the model with a simpler but less accurate one to reduce its own operational costs, or it may be compromised and return the wrong result to the client. In SafetyNets {% cite ghodsi2017safetynets%}, we proposed a framework for verifiable execution of neural networks on untrusted cloud servers which started a line of research on verifiable machine learning.

