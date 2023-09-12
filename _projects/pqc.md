---
layout: page
title: Post-quantum Crypto
description: Summary of my projects in post-quantum cryptography.
img: assets/img/pqc-app.png
importance: 2
category: work
giscus_comments: false
body: false
---

### Background
The rapid advancement of quantum computing has exposed vulnerabilities in traditional cryptography, particularly in public-key cryptography. Experts predict that within the next decade, our existing public-key encryption methods may become compromised. To address this impending threat, the field of Post-Quantum Cryptography (PQC) has emerged, focusing on cryptographic techniques that remain secure even in the face of quantum computers.

The National Institute of Standards and Technology (NIST) has taken a pivotal role in this effort by conducting a competition to standardize PQC algorithms. In this competition, Crystals-Kyber has been identified as the Key Encapsulation Mechanism (KEM) and public-key encryption scheme, while Crystals-Dilithium, Falcon, and Sphincs^+ have been designated as signature schemes for standardization.

While our classical public-key encryption methods remain unbroken at present, it is imperative to initiate the transition to PQC, primarily due to the potential vulnerability of ciphertext storage to attacks. This proactive approach ensures the long-term security of sensitive information in an era where the capabilities of quantum computers are continually evolving.

### Project 1: Post-Quantum Key Management Software

**Requirement:** The objective of this project is to create a robust key management software capable of securely storing and managing post-quantum keys. Several key design requirements are essential for this software:

1. **Key Generation and Sharing:** The software should enable an administrator to generate key material securely. Subsequently, this key material should be shareable with clients, either through physical means or digital channels, employing Post-Quantum Cryptography (PQC) primitives. This ensures that keys are generated and distributed using quantum-resistant methods.

2. **Authentication and Revocation:** It is crucial that the software allows clients to authenticate communications from the administrator. Additionally, clients should have the capability to revoke any received key material if needed, ensuring that the security of the keys can be maintained over time.

3. **Platform Independence:** To maximize usability and flexibility, the software should be designed to be independent of external dependencies. It should have the versatility to run seamlessly on various platforms, enhancing its adaptability for diverse user environments.

**Solution:** To address these requirements, we have developed a key management software solution in Python. One notable feature of our solution is its minimal reliance on external dependencies. We have integrated the source code from Crystals for Kyber and Dilithium into our software for key generation and encryption purposes, minimizing external dependencies and enhancing the software's self-contained nature.

Our software not only meets the stipulated requirements but also ensures the long-term security and management of post-quantum keys, aligning with the evolving landscape of quantum computing and cryptography.


### Project 2: post-quantum participation certificates



