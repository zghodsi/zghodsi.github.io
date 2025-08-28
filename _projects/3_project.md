---
layout: page
title: hardware acceleration
img: assets/img/7.jpg
importance: 3
category: work
related_publications: true
---

Domain-specific hardware accelerators are computing engines that are specialized for a particular domain of applications, offering orders of magnitude improvement in performance. Accelerators are critical in enabling cutting-edge applications such as machine learning, and provide benefits based on specialized operations, parallelism, and efficient memory management. We can also design specialized hardware to accelerate expensive cryptographic protocols to provide security guarantees to various systems without compromising efficiency. 

In our prior work cuOT {% cite gan2025cuot%} we developed the first GPU-based library for accelerating Oblivious Transfer (OT), a fundamental building block in cryptographic protocols for secure multiparty computation. As an example use case, consider privacy-preserving machine learning (PPML) which is a popular application of secure computation. State-of-the-art protocols for PPML combine homomorphic encryption for linear layers and OT for non-linear layer evaluations. However, PPML computations (e.g., performing one private inference) are still orders of magnitude more expensive than their non-private counterpart, with non-linear layer evaluations taking up to 60% of runtime. cuOT accelerates the OT protocol on GPU, improving OT generation time by up to 75x.

Despite providing efficiency benefits, hardware accelerators can also be accompanied by security concerns. Accelerators are typically designed and fabricated by external third party vendors. As a result, a malicious vendor would be able to corrupt the hardware by Trojans or fault injection attacks. In SafeTPU {% cite collantes2020safetpu%}, we provide security guarantees for a machine learning accelerator regardless of how the hardware Trojan is designed or triggered. Rather than relying on heuristics  to detect or mitigate Trojans, we build on cryptographic interactive proofs which ensures that any incorrect output can be detected with high probability.  

