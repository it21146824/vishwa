---
id: "Modular Arithmetic"
aliases:
  - "Modular Arithmetic"
tags: []
---

## Modular Arithmetic

### Modulo Operation
+ This is an operation that **returns the remainder of a division operation**.
+ The modulo operation is denoted by **$a \bmod m$**.
    + For example, **$27 \bmod 6 = 3$**.
    + **$27 \div 6 = 4$** with a remainder of **$3$**.
    + Therefore, **$27 \bmod 6 = 3$**.
+ Other notations for the modulo operation are:
    1. **$a \bmod m = r$**
    2. **$a \equiv r \pmod m$**
    3. **$r = \bmod(a, m)$**

#### Properties Of The Modulo Operation
1. **$a \bmod m$** is always smaller than **$m$**.
    + This is true because the **remainder of a division operation is always smaller than the divisor**.

2. If **$a$** is smaller than **$m$**, then **$a \bmod m = a$**.
    + For example, lets consider **$7 \bmod 10 = 7$**.
    + **$7$** is smaller than **$10$**.
    + We are basically asking: **"How many times does 10 fit into 7?"**
    + The answer is **$0$** times, with **$7$** remaining.
    + So, **$a \bmod m$** equals **$7$** because there's no full '**$10$**' within '**$7$**', and **$7$** is the remainder.

3. **$(a + k \cdot m) \bmod m = a \bmod m$**.
    + This means that **$(7+3 \cdot 5) \bmod 5 = 7 \bmod 5$**.
    + Also means that **$(7+20 \cdot 5) \bmod 5 = 7 \bmod 5$**.
    + What this means is that **adding multiples of the divisor to the dividend does not change the remainder**.

#### Calculating Negative Modulo Values
+ Assume that we are told to find **$-7 \bmod 5$**.
    + The closest & smallest multiple of **$5$** to **$-7$** is **$-10$**.
    + **$-10$** is **$3$** away from **$-7$**.
    + Therefore, **$-7 \bmod 5 = 3$**.

#### Associativity In Modulo Operations
+ **$k+a \bmod m = (k+a) \bmod m$**
    + For example:
        + **$5+7 \bmod 10 = (5+7) \bmod 10 = 12 \bmod 10 = 2$**
        + **$1+1 \bmod 2 = (1+1) \bmod 2 = 2 \bmod 2 = 0$**
        + **$1-1 \bmod 2 = (1-1) \bmod 2 = 0 \bmod 2 = 0$**
        + **$4 \times 7 \bmod 27 = (4 \times 7) \bmod 27 = 28 \bmod 27 = 1$**
        + **$14^{7} \bmod 13 = (14^{7}) \bmod 13 = 105413504 \bmod 13 = 1$**
    + Basically, **perform any operation on the left side of the modulo operation**, and then perform the modulo operation on the result.

#### Modular Arithmetic Tables
+ These are basically tables that show the results of a modulo operation.

+ **Addition mod 4**: **$a + b \bmod m$** where **$a$** & **$b$** are the numbers to be added, and **$m$** is the divisor.
    + |   $+$   | **$0$** | **$1$** | **$2$** | **$3$** | **$4$** |
      | ------- | ------- | ------- | ------- | ------- | ------- |
      | **$0$** |   $0$   |   $1$   |   $2$   |   $3$   |   $4$   |
      | **$1$** |   $1$   |   $2$   |   $3$   |   $4$   |   $0$   |
      | **$2$** |   $2$   |   $3$   |   $4$   |   $0$   |   $1$   |
      | **$3$** |   $3$   |   $4$   |   $0$   |   $1$   |   $2$   |
      | **$4$** |   $4$   |   $0$   |   $1$   |   $2$   |   $3$   |

+ **Multiplication mod 4**: **$a \times b \bmod m$** where **$a$** & **$b$** are the numbers to be multiplied, and **$m$** is the divisor.
    + |   $\times$   | **$0$** | **$1$** | **$2$** | **$3$** | **$4$** |
      | ------------ | ------- | ------- | ------- | ------- | ------- |
      | **$0$**      |   $0$   |   $0$   |   $0$   |   $0$   |   $0$   |
      | **$1$**      |   $0$   |   $1$   |   $2$   |   $3$   |   $4$   |
      | **$2$**      |   $0$   |   $2$   |   $4$   |   $0$   |   $2$   |
      | **$3$**      |   $0$   |   $3$   |   $0$   |   $3$   |   $0$   |
      | **$4$**      |   $0$   |   $4$   |   $2$   |   $0$   |   $4$   |

### Mini-Exercise (Modulo Operations)
1. **$17 \bmod 5$**
    + **$17 \div 5 = 3$** with a remainder of **$2$**.
    + Therefore, **$17 \bmod 5 = 2$**.
2. **$343 \bmod 2$**
    + **$343 \div 2 = 171$** with a remainder of **$1$**.
    + Therefore, **$343 \bmod 2 = 1$**.
3. **$0 \bmod 77$**
    + **$0 \div 77 = 0$** with a remainder of **$0$**.
    + Therefore, **$0 \bmod 77 = 0$**.
4. **$97 \bmod 98$**
    + **$97 \div 98 = 0$** with a remainder of **$97$**.
    + Therefore, **$97 \bmod 98 = 97$**.
5. **$98 \bmod 97$**
    + **$98 \div 97 = 1$** with a remainder of **$1$**.
    + Therefore, **$98 \bmod 97 = 1$**.
6. **$-4 \bmod 6$**
    + The closest & smallest multiple of **$6$** to **$-4$** is **$-6$**.
    + **$-6$** is **$2$** away from **$-4$**.
    + Therefore, **$-4 \bmod 6 = 2$**.

