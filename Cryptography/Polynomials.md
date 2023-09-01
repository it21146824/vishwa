---
id: "Polynomials"
aliases:
  - "Polynomials"
tags: []
---

### Polynomials
+ These are equations that can be represented in the following form **$ax^{m} + bx^{n} + c$**.
    + **$a$**, **$b$**, & **$c$** are **constants**
    + **$x$** is a **variable**
    + **$m$** & **$n$** are **exponents**

+ An example polynomial is: **$3x^{2} + 2x + 1$**.

### Interpolation
+ The process of **finding the equation** of a polynomial **given a set of points**.
+ Assume we have the points: **$(2, 3)$** and **$(3, 5)$**:
    + This means that:
        + **$(2, 3)$** : **$x = 2$** & **$y = 3$**
        + **$(3, 5)$** : **$x = 3$** & **$y = 5$**
    + If we substitute this to the the equation of a straight line: **$y = mx + c$**, we get:
        + **$3 = 2m + c$**
        + **$5 = 3m + c$**
    + We use **simultaneous equations** to solve for **$m$** & **$c$**:
        + **$3 = 2m + c$**
        + **$5 = 3m + c$**
        + If we **substract these two equations**, we will get:
            + **$3 - 5 = 2m + c - 3m - c$**
            + **$-2 = -m$**
            + **$m = 2$**
        + Since we have discovered that **$m$** is **$2$**, lets substitute **$m$** into our first equation to find **$c$**.
            + **$3 = 2(2) + c$**
            + **$3 = 4 + c$**
            + **$3 - 4 = 4 + c - 4$**
            + **$-1 = c$**
            + **$c = -1$**
    + Therefore, the equation of the line is: **$y = 2x - 1$**.

### Mini-Exercise
1. Given **$f(x) = 3x^{2}−4x+5$**, evaluate this polynomial at the points **$0$,$1$ & $2$**.
    + **$f(0) = 3(0)^{2}−4(0)+5 = 5$**
        + **$f(0) = 0-0+5 = 5$**
            + **$f(0) = 5$**

2. Perform interpolation using the points **$(1, 1)$** and **$(2, −3)$** in order to compute a polynomial **$g(x)$** of degree **$1$**, satisfying **$g(1) = 1$** and **$g(2) = −3$**
    + **$g(x) = mx + c$**
    + **$g(1) = 1$**
        + **$1 = m(1) + c$**
        + **$1 = m + c$**
    + **$g(2) = -3$**
        + **$-3 = m(2) + c$**
        + **$-3 = 2m + c$**
    + **$1 = m + c$**
    + **$-3 = 2m + c$**
    + **$1 - (-3) = m + c - 2m - c$**
    + **$4 = -m$**
    + **$m = -4$**
    + **$1 = -4 + c$**
    + **$1 - (-4) = -4 + c - (-4)$**
    + **$5 = c$**
    + **$c = 5$**
    + **$g(x) = -4x + 5$**
