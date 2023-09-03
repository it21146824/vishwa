---
id: "Boolean Algebra"
aliases:
  - "Boolean Algebra"
tags: []
---

### Boolean Algebra
+ A branch of mathematics that **deals with logical operations** and their representation using **algebraic structures**, allowing us to manipulate and **analyze logical expressions** in a formal and systematic way.

|  A   |   B   |   A AND B   |   A OR B   |   A **$\oplus$** B   |   A **$\rightarrow$** B   |   A **$\leftrightarrow$** B   |
|:----:|:-----:|:-----------:|:----------:|:--------------------:|:--------------------------:|:------------------------------:|
| **0**| **0** |    **0**    |   **0**    |        **0**         |            **1**           |              **1**             |
| **0**| **1** |    **0**    |   **1**    |        **1**         |            **1**           |              **0**             |
| **1**| **0** |    **0**    |   **1**    |        **1**         |            **0**           |              **0**             |
| **1**| **1** |    **1**    |   **1**    |        **0**         |            **1**           |              **1**             |

#### AND : $\wedge$
+ If **two inputs are true**, the output is **true**.
+ If **one or both inputs are false**, the output is **false**.

|   A   |   B   |   A AND B   |
|:-----:|:-----:|:-----------:|
| **0** | **0** |    **0**    |
| **0** | **1** |    **0**    |
| **1** | **0** |    **0**    |
| **1** | **1** |    **1**    |

#### OR : $\vee$
+ If **one or both inputs are true**, the output is **true**.

|   A   |   B   |   A OR B   |
|:-----:|:-----:|:----------:|
| **0** | **0** |   **0**    |
| **0** | **1** |   **1**    |
| **1** | **0** |   **1**    |
| **1** | **1** |   **1**    |

#### XOR **$\oplus$**
+ XOR is represented by the symbol **$\oplus$**.
+ If **one input is true** and **one input is false**, the output is **true**.
+ If **both inputs are true** or **both inputs are false**, the output is **false**.
+ Very similar to an OR gate, but **false when both inputs are true**.

|   A   |   B   |   A **$\oplus$** B   |
|:-----:|:-----:|:--------------------:|
| **0** | **0** |        **0**         |
| **0** | **1** |        **1**         |
| **1** | **0** |        **1**         |
| **1** | **1** |        **0**         |

#### If-Then **$\rightarrow$**
+ Also known as **implication**, represented by the symbol **$\rightarrow$**.
+ If **the first input is false**, the output is **true**.
+ If **the first input is true**, the output is **the second input**.

|   A   |   B   |   A **$\rightarrow$** B   |
|:-----:|:-----:|:------------------------:|
| **0** | **0** |           **1**          |
| **0** | **1** |           **1**          |
| **1** | **0** |           **0**          |
| **1** | **1** |           **1**          |

#### If And Only If **$\leftrightarrow$**
+ Also known as **equivalence**, represented by the symbol **$\leftrightarrow$**.
+ If **both inputs are true** or **both inputs are false**, the output is **true**.
+ If **one input is true** and **one input is false**, the output is **false**.

|   A   |   B   |   A **$\leftrightarrow$** B   |
|:-----:|:-----:|:------------------------------:|
| **0** | **0** |              **1**             |
| **0** | **1** |              **0**             |
| **1** | **0** |              **0**             |
| **1** | **1** |              **1**             |

### Mini-Exercise
1. **$101101 \oplus 111$** = **$101010$**
2. **$101$** OR **$1100$** = **$1101$**
