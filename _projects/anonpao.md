---
layout: page
title: Anonymous PAO
description: A proof of concept for a cryptographic protocol that allows users to prove ownership of an account without revealing their account identifier.
img: assets/img/anonpao-otp.png
importance: 1
category: work
related_publications: youchoose
---

Anonymous PAO lets a prover prove to a verifier that it owns a valid account at a server without being tracked by the server or the verifier. This happens without requiring any changes at the server's end and without even revealing to the server that any anonymous PAO is taking place. 

### problem
Company reviews are important for both potential employees and the company itself, but they can be risky for current employees to post because it might harm them. Anonymous reviews can be faked, and third-party identity verification requires trust that the third party won't side with the company and disclose the employee's identity.

Our solution allows users to prove to a verifier that they own an account (say email account) with the company without revealing which account (i.e. the email address).

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/anonpao-feedback" title="feedback image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

