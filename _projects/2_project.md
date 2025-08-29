---
layout: page
title: privacy-preserving computation 
img: assets/img/2.jpg
importance: 2
category: work
related_publications: true
---

Recent advancements in big data analytics and artificial intelligence are in large part due to access to massive amounts of data and powerful computing resources. The continued development of such technologies depends on addressing increasing concerns around data usage and privacy. In many cases, the collected data can be sensitive, including details about individuals and organizations that may leak their identity, location, health, or financial information. Privacy-preserving computation techniques based on cryptographic protocols have gained further popularity in recent years to provide privacy guarantees while enabling statistical and machine learning applications.

We have explored privacy guarantees in federated learning (FL) which offers a decentralized paradigm for model training. FL enables a group of clients to train a model locally  and share their gradients with a server who aggregates all the updates and  updates a global model to be shared with the clients. However, individual model updates leak information about clients' private datasets, requiring cryptographic protocols for secure aggregation to support private FL, ensuring that the server only sees the aggregate value rather than individual contributions from each client. A related question to preserving data privacy in FL is preserving client participation anonymity. In AnoFel {% cite almashaqbeh2023anofel  %} we present the first provably secure framework for private and  anonymous user participation in FL. AnoFel utilizes a public bulletin board, various cryptographic primitives, and differential privacy to support secure aggregation of model updates and client anonymity in both static and dynamic settings.


Beyond training machine learning models, inference computations (e.g., a client querying a remote server's trained model with their input) can also lead to privacy concerns, in particular with respect to client's sensitive input and the server's proprietary model. We have developed several frameworks including CryptoNAS {% cite ghodsi2020cryptonas %}, Circa {% cite ghodsi2021circa %}, and DeepReduce {% cite jha2021deepreduce %} to enable efficient and privacy-preserving inference computations.



