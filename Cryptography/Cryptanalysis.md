---
id: "Cryptanalysis"
aliases:
  - "Cryptanalysis"
tags: []
---

### Cryptanalysis
+ This is the process of **breaking cryptographic functions** to test their security.
+ **Kerckhoff's Principle**: This is a principle that states that even though an attacker knows the internal workings of the algorithm, they should not be able to break it.
+ There are **three types of cryptanalysis** attacks:
    1. **Implementation Attacks**: Finding problems/mistakes in the implementation of the algorithm and exploiting it.
    2. **Social Engineering**: Tricking a user to give out the secret key.
    3. **Classical Cryptanalysis**
        + **Mathematical Attacks**: Exploiting vulnerabilities in the mathematical properties of the algorithm.
        + **Brute-force Attacks / Exhaustive Key Search**: Trying all possible keys to find the correct one.
            + Brute-force attacks require both the ciphertext **$y_{0}$** and its decoded plaintext **$x_{0}$**.
            + The attacker will try all possible keys **$k$** until **$d_{k}(y_{0}) = x_{0}$**.
