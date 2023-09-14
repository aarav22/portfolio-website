---
layout: page
title: Anonymous PAO
description: A proof of concept for a cryptographic protocol that allows users to prove ownership of an account without revealing their account identifier.
img: assets/img/anonpao-otp.png
importance: 1
category: work
related_publications: youchoose
---




### Problem
Company reviews are important for both potential employees and the company itself, but they can be risky for current employees to post as they might face retaliation from the company. Anonymous reviews can be faked, and third-party identity verification requires trust that the third party won't side with the company and disclose the employee's identity.

<div class="row">
    <div class="col-sm-6 mt- mt-md-0">
        {% include figure.html path="assets/img/anonpao-feedback" title="feedback image" class="img-fluid rounded" %}
    </div>
</div>

## Solution 
Our solution allows users to prove to a verifier that they own an account (say email account) with the company without revealing which account (i.e. the email address). An important aspect of this solution is that the prover does not require any co-operation from the company as is usually the case in anonymous credentials.


