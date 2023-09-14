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

The National Institute of Standards and Technology (NIST) has taken a pivotal role in this effort by conducting a competition to standardize PQC algorithms. In this competition, Crystals-Kyber has been identified as the Key Encapsulation Mechanism (KEM) and public-key encryption scheme, while Crystals-Dilithium, Falcon, and Sphincs$^+$ have been designated as signature schemes for standardization.

While our classical public-key encryption methods remain unbroken at present, it is imperative to initiate the transition to PQC, primarily due to the potential *store now, decrypt later* attacks. This proactive approach ensures the long-term security of sensitive information in an era where the capabilities of quantum computers are continually evolving.

### Project 1: Post-Quantum Key Management Software

**Aim:** The objective of this project is to create a key management software capable of securely storing and managing post-quantum keys. Several key design requirements are essential for this software:

1. **Key Generation and Sharing:** The software should enable an administrator (KDC) to generate key material securely. Subsequently, this key material should be shareable with clients, either through physical means (HSM) or digital channels (TLS), employing Post-Quantum Cryptography (PQC) primitives.

2. **Authentication and Revocation:** It is important that the software allows clients to authenticate communications from the KDC. Additionally, clients should have the capability to revoke any received key material from further use, if needed.

3. **Platform Independence:** To ensure auditability, the software should be independent of external dependencies. Furthermore, it should have the ability to run seamlessly on various platforms, enhancing its adaptability.

**Implementation:** To meet these requirements, we've designed a Python-based key management software solution. A key aspect of the software (no pun intended) is the use of post-quantum X.509 certificates for authentication, and data transportation via extensions. These certificates are custom-built yet maintain verifiability through OQS's [OpenSSL](https://github.com/open-quantum-safe/openssl) fork. 


### Project 2: dilithium-signed workshop certificates

**Aim:** This project aims to generate digital participation certificates that are authenticated using the Dilithium signature scheme. These certificates should be easily verifiable through the signer's public key.

**Implementation:** These certificates were created and distributed to all participants during the [PQC Workshop](https://pqcworkshop-cs-ashoka.streamlit.app/) at Ashoka University. 

