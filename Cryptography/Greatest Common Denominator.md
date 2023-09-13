---
id: "Greatest Common Denominator"
aliases:
  - "Greatest Common Denominator"
tags: []
---
### Greatest Common Denominator
+ Finding out **the greatest integer that divides two integers** without leaving a remainder.
+ It is notated by: **$gcd(a, b)$**.

### How To Find GCD
#### 1. Greatest Common Factor
1. Find the numbers that divide both numbers without leaving a remainder.
2. Find the **common factors** that will divide the number **without leaving a remainder**.
3. The **largest common factor** is the GCD.
    + For example, **$gcd(12, 18)$**:
    + $12 = 1, 2, 3, 4,$ **$6$**, $12$
    + $18 = 1, 2, 3,$ **$6$**$, 9, 18$
    + $gcd(12, 18) =$ **$6$**

#### 2. Prime Factorization
1. Find the prime factorization of both numbers.
2. Multiply the common prime factors.
3. The product is the GCD.
    + For example, **$gcd(12, 18)$**:
        + $12 =$ **$2$** $\cdot 2 \cdot$ **$3$**
        + $18 =$ **$2$** $\cdot$ **$3$** $\cdot 3$
        + $gcd(12, 18) = 2 \cdot 3 = 6$

#### 3. Euclidean Algorithm
1. **Start with two integers, a and b, where a is greater than or equal to b.**
   + For example, let's use **$a = 48$** and **$b = 18$**.

2. **Divide $a$ by $b$ and find the remainder $(r)$.**
   + **$a = 48$**.
   + **$b = 18$**.
   + **$r = a \bmod b = 48 \bmod 18 = 12$**.

3. **If r is not equal to 0, set $a = b$, and $b = r$, then go back to step 2.**
   + In our example, since **$r = 12$** is not equal to **$0$**, we update **$a = 18$** and **$b = 12$**, and repeat step 2.

4. **Repeat steps 2 and 3 until r becomes 0.**
   + We continue the process:
     + **$a = 18, b = 12, r = a \bmod b = 18 \bmod 12 = 6$**.
     + **$a = 12, b = 6, r = a \bmod b = 12 \bmod 6 = 0$**.

5. **When r becomes 0, the GCD is the non-zero value of b.**
   + The GCD is **$6$** in the example above.

+ For example, let's use the Euclidean Algorithm to find the GCD of **$48$** and **$18$**:
    1. Start: **$a = 48, b = 18$**.
        + **$a \bmod b = 48 \bmod 18 = 12$**.
    3. Update: **$a = 18, b = 12$**.
        + **$a \bmod b = 18 \bmod 12 = 6$**.
    5. Update: **$a = 12, b = 6$**.
        + **$a \bmod b = 12 \bmod 6 = 0$**.
    7. Since **$r = 0$**, the GCD is the non-zero value of **$b$**, which is **$6$**.

+ So, **$GCD(48, 18) = 6$**.

#### Co-Prime Numbers
+ Two numbers are **co-prime** if their **GCD (greatest common denominator) is 1**.
    + For example, **$gcd(12, 25) = 1$**.
    + This means that **12 & 25 are co-prime**.

### Mini-Exercise
1. Compute the GCD of **$75$** and **$28$** using:
    1. Prime-factor decomposition.
        + **$75 = 3 \cdot 5 \cdot 5$**.
        + **$28 = 2 \cdot 2 \cdot 7$**.
        + **$gcd(75, 28) = 1$**.

    2. Euclidean algorithm.
        + **$75 \bmod 28 = 19$**.
        + **$28 \bmod 19 = 9$**.
        + **$19 \bmod 9 = 1$**.
        + **$9 \bmod 1 = 0$**.
        + **$gcd(75, 28) = 1$**.

2. Find the greatest common divisor **$g$** of **$799$** and **$987$**. Find integers **$x$** and **$y$** such that **$799x + 987y = g$**.
