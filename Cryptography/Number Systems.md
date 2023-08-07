---
id: "Number Systems"
aliases:
  - "Decimal Number System"
  - "Decimal"
  - "Number Systems"
tags: []
---
# Number Systems
+ A system used to **represent numbers**.

#### Number System Formula:
> **$d_b(a) = (d_k\times b^k) + (d_{k-1}\times b^{k-1}) + \dots + (d_1\times b^1) + (d_0\times b^0)$**
+ **$d$** : Digit
+ **$b$** : Base
+ **$a$** : Number
+ **$k$** : The current digit's index
+ **$d_k$** : **$k^{th}$** digit of **$a$**

##### Formula Explanation
+ Assume that we have the number **$1234$** and consider it as **$a$**, then:
    + **$a$** : **$1234$**
    + **$b$** : **$10$**
    + **$d_3$** : **$1$**
    + **$d_2$** : **$2$**
    + **$d_1$** : **$3$**
    + **$d_0$** : **$4$**
    + **$d_b(a)$** : **($1\times 10^3) + (2\times 10^2) + (3\times 10^1) + (4\times 10^0)$**
        + **$d_b(a)$** : **$1000 + 200 + 30 + 4$**
            + **$d_b(a)$** : **$1234$**

---
###### Decimal to Binary
+ Assume that we have the number **$22$** and consider it as **$a$**, then:
    + **$\frac{22}{2} = 11$** with a remainder of **$0$**
    + **$\frac{11}{2} = 5$** with a remainder of **$1$**
    + **$\frac{5}{2} = 2$** with a remainder of **$1$**
    + **$\frac{2}{2} = 1$** with a remainder of **$0$**
    + **$\frac{1}{2} = 0$** with a remainder of **$1$**
    + Collect the remainders from bottom to top to get **$10110$**.

---
###### Fractional Decimal to Binary
+ Assume that we have the number **$\frac{5}{8}$** and consider it as **$a$**, then:
+ **$\frac{5}{8} \times 2 = \frac{10}{8} = 1\frac{2}{8}$** *($k_{-1}$ is $1$ as there is whole number)*
    + **$\frac{2}{8} \times 2 = \frac{4}{8} = \frac{1}{2}$** *($k_{-2}$ is $0$ as there is no whole number)*
        + **$\frac{1}{2} \times 2 = 1$** *($k_{-3}$ is $1$ as there is a whole number)*
            + **$(\frac{5}{8})_{10} = (0.101)_{2}$**

---
###### Fractional Binary to Decimal
+ Assume that we have the number **$0.1011$** and consider it as **$a$**, then:
    + **$k_{-1}$** : **$1$**
    + **$k_{-2}$** : **$0$**
    + **$k_{-3}$** : **$1$**
    + **$k_{-4}$** : **$1$**
    + As these are fractional binary numbers, $k$ will start from **$-1$**.
        + **$(d_k\times b^k) + (d_{k-1}\times b^{k-1}) + \dots + (d_1\times b^1) + (d_0\times b^0)$**
            + **$(d_{-1}\times 2^{-1}) + (d_{-2}\times 2^{-2}) + (d_{-3}\times 2^{-3}) + (d_{-4}\times 2^{-4})$**
                + **$(1 \times \frac{1}{2}) + (0 \times \frac{1}{4}) + (1 \times \frac{1}{8}) + (1 \times \frac{1}{16})$**
                    + **$\frac{1}{2} + \frac{0}{4} + \frac{1}{8} + \frac{1}{16}$**
                        + **$\frac{8}{16} + \frac{0}{16} + \frac{2}{16} + \frac{1}{16}$**
                            + **$\frac{11}{16}$**
---

###### Decimal to Ternary
+ Assume that we have the number **$22$** and consider it as **$a$**, then:
    + **$\frac{22}{3} = 7$** with a remainder of **$1$**
    + **$\frac{7}{3} = 2$** with a remainder of **$1$**
    + **$\frac{2}{3} = 0$** with a remainder of **$2$**
    + Collect the remainders from bottom to top to get **$211$**.
---

###### Decimal to Hexadecimal
+ Assume that we have the number **$50$** and consider it as **$a$**, then:
    + **$50 \div 16 = 3$** with a remainder of **$2$**
    + **$3 \div 16 = 0$** with a remainder of **$3$**
    + Collect the remainders from bottom to top to get **$32_{16}$**
---

### Mini-Exercise
1. Convert **$1010110_2$** to decimal.
    + **$1010110_2$** = **$1 \times 2^6 + 0 \times 2^5 + 1 \times 2^4 + 0 \times 2^3 + 1 \times 2^2 + 1 \times 2^1 + 0 \times 2^0$**
        + **$1 \times 64 + 0 \times 32 + 1 \times 16 + 0 \times 8 + 1 \times 4 + 1 \times 2 + 0 \times 1$**
            + **$64 + 16 + 4 + 2$**
                + **$86$**

2. Write the integer **$12$** as:
    1. Decimal:
        + **$12_{10} = 12_{10}$**
    2. Binary:
        + **$12_{10} = \frac{12}{2} = 6$** with a remainder of **$0$**
            + **$\frac{6}{2} = 3$** with a remainder of **$0$**
                + **$\frac{3}{2} = 1$** with a remainder of **$1$**
                    + **$\frac{1}{2} = 0$** with a remainder of **$1$**
                        + Collect the remainders from bottom to top to get **$1100_{2}$**.
    3. Ternary:
        + **$12_{10} = \frac{12}{3} = 4$** with a remainder of **$0$**
            + **$\frac{4}{3} = 1$** with a remainder of **$1$**
                + **$\frac{1}{3} = 0$** with a remainder of **$1$**
                    + Collect the remainders from bottom to top to get **$110_{3}$**.

3. Convert **${0.011_2}$** into decimal notation.
    + **${0.011_2} = (0 \times 2^{-1}) + (1 \times 2^{-2}) + (1 \times 2^{-3})$**
        + **${0.011_2} = 0 + \frac{1}{4} + \frac{1}{8}$**
            + **${0.011_2} = \frac{3}{8}$**

4. Write **$\frac{5}{10}$** as:
    1. Binary:
        + **$\frac{5}{10} = \frac{1}{2}$**
            + **$\frac{1}{2} \times 2 = 1$**
                + **$\frac{5}{10} = 0.1_{2}$**

    2. Ternary:
        + **$\frac{5}{10} = \frac{1}{2}$**
            + **$\frac{1}{2} \times 3 = 1\frac{1}{2}$**
                + **$\frac{1}{2} \times 3 = 1\frac{1}{2}$**
                    + This seems to be a *recurring fraction*
                        + **$\frac{5}{10}_{10} = 0.\overline{1}_{3}$**
---
