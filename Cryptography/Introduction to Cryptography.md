---
id: "Introduction to Cryptography"
aliases:
  - "Historical Cryptographic Ciphers"
  - "Terminology"
tags: []
---

#### Terminology
1. **Symmetric Ciphers**: The same key is used to encrypt and decrypt the message.
2. **Asymmetric Ciphers**: Two keys are used to encrypt and decrypt the message.
3. **Hybrid Schemes**: The usage of both asymmetric ciphers and symmetric ciphers.
4. **Plaintext**: Text that still has not been encrypted.
5. **Ciphertext**: Plaintext that is now encrypted.
6. **Cryptanalysis**: The study of how to break cryptographic algorithms.
7. **Kerckhoff's Principle**: The security of a cryptographic algorithm should not depend on the secrecy of the algorithm.
8. **Brute-force Attacks**: Trying all possible keys to find the correct one (also known as Known-Plaintext Attacks).
9. **Exhaustive Key Search**: A similar word for brute-force attacks.
10. **Substitution Cipher**: A cipher that replaces each letter in the plaintext with another letter.
---
### Symmetric Cryptography

1. Encryption function: **$e_{k}()$**
1. Decryption function: **$d_{k}()$**
2. Ciphertext: **$y$**
3. Plaintext: **$x$**
4. Key: **$k$**

##### Encryption Function: **$y = e_{k}(x)$**
+ The function **$e_{k}()$** is responsible for **converting plaintext into ciphertext** using a key.
    + The plaintext **$x$** is sent into the encryption function **$e_{k}()$** and its output is saved as **$y$**. This can be formalized as **$y = e_{k}(x)$**.
    + If you swap **$y$** and **$x$** in this equation, you get the decryption function.

##### Decryption Function: **$x = d_{k}(y)$**
+ The function **$d_{k}()$** is responsible for **converting ciphertext into plaintext** using a key.
    + The ciphertext **$y$** is sent into the decryption function **$d_{k}()$** and its output is saved as **$x$**. This can be formalized as **$x = d_{k}(y)$**.

+ Another way to write the decryption function is: **$x = d_{k}(e_{k}(x))$**.
    + The above is just **$e_{k}(x)$** passed into **$d_{k}()$**.
    + This is because the **decryption function undoes the encryption function**.
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

### Substitution Cipher
+ This is a cipher that **replaces each letter with another letter** to convert plaintext into ciphertext.
    #### Attacks Against Substitution Ciphers
    1. **Exhaustive Key Search (Brute-force Attacks)**: Testing all [[Substitution Tables]] to find the correct one.
        + This attack is not practical because there are **$26!$** possible keys.
        + However, substitution ciphers are still **vulnerable to frequency analysis attacks**.

    2. **Frequency Analysis**: This is an attack that uses the fact that some letters are more common than others.
        + For example, the letter **e** is the most common letter in the English language.
        + The attacker can use this fact to **find the most common letter in the ciphertext** and assume that it is the letter **e** and use this information to decipher the other letters.
        + The following are the **top 5 frequent letters** in the English alphabet an attacker can compare to perform a frequency analysis:

            | Letter | Frequency (%)|
            |:------:|:------------:|
            | E      | 13           |
            | T      | 9            |
            | A      | 9            |
            | O      | 8            |
            | N      | 7            |
