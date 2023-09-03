
### Symmetric Cryptography

1. Encryption function: **$e_{k}()$**
1. Decryption function: **$d_{k}()$**
2. Ciphertext: **$y$**
3. Plaintext: **$x$**
4. Key: **$k$**
---
##### Encryption Equation: **$y = e_{k}(x)$**
+ The function **$e_{k}()$** is responsible for **converting plaintext into ciphertext** using a key.
    + The plaintext **$x$** is sent into the encryption function **$e_{k}()$** and its output is saved as **$y$**. This can be formalized as **$y = e_{k}(x)$**.
    + If you swap **$y$** and **$x$** in this equation, you get the decryption function.
---
##### Decryption Equation: **$x = d_{k}(y)$**
+ The function **$d_{k}()$** is responsible for **converting ciphertext into plaintext** using a key.
    + The ciphertext **$y$** is sent into the decryption function **$d_{k}()$** and its output is saved as **$x$**. This can be formalized as **$x = d_{k}(y)$**.

+ Another way to write the decryption function is: **$x = d_{k}(e_{k}(x))$**.
    + The above is just **$e_{k}(x)$** passed into **$d_{k}()$**.
    + This is because the **decryption function undoes the encryption function**.
