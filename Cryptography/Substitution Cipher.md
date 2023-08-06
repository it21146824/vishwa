---
id: "Substitution Cipher"
aliases:
  - "Substitution Cipher"
tags: []
---

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
