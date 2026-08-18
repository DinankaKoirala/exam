# Unit 4 — Beta and Gamma Functions
> MATH 104 Advanced Calculus · Kathmandu University

---

## 🎯 YouTube Search Topics

| Topic | Search Query |
|---|---|
| Gamma function explained | `gamma function explained intuition` |
| Gamma function and factorials | `gamma function extends factorial` |
| Beta function | `beta function properties calculus` |
| Relation between Beta and Gamma | `beta gamma function relation proof` |
| Gaussian integral | `gaussian integral trick pi` *(relates to $\Gamma(1/2) = \sqrt{\pi}$)* |

---

## 📖 Core Concepts

### 4.1 Definitions

**Beta Function** (First Eulerian Integral):
$$B(m,n) = \int_0^1 x^{m-1}(1-x)^{n-1}\, dx \qquad (m > 0,\ n > 0)$$

**Gamma Function** (Second Eulerian Integral):
$$\Gamma(p) = \int_0^\infty e^{-x} x^{p-1}\, dx \qquad (p > 0)$$

### 4.1 Properties of the Gamma Function

| Property | Formula |
|---|---|
| Reduction formula | $\Gamma(p+1) = p\,\Gamma(p)$ |
| Factorial connection | $\Gamma(n+1) = n!$ for $n \in \mathbb{N}$ |
| Special value | $\Gamma(1) = 1$ |
| Special value | $\Gamma(1/2) = \sqrt{\pi}$ |

**Derived values:**
- $\Gamma(3/2) = \frac{1}{2}\Gamma(1/2) = \frac{\sqrt{\pi}}{2}$
- $\Gamma(5/2) = \frac{3}{4}\sqrt{\pi}$

### 4.1 Properties of the Beta Function

1. **Symmetry:** $B(m,n) = B(n,m)$

2. **Alternate form:**
$$B(m,n) = \int_0^\infty \frac{x^{m-1}}{(1+x)^{m+n}}\, dx$$

3. **Trigonometric form:**
$$B(m,n) = 2\int_0^{\pi/2} \sin^{2m-1}\theta\,\cos^{2n-1}\theta\, d\theta$$

### 4.3 Relation Between Beta and Gamma

$$B(m,n) = \frac{\Gamma(m)\,\Gamma(n)}{\Gamma(m+n)}$$

This is the most powerful identity — it lets you evaluate complicated integrals by converting to Beta/Gamma form.

### 4.2 Transformations of Gamma Functions

$$\Gamma(p) = 2\int_0^\infty e^{-x^2} x^{2p-1}\, dx$$

Setting $p = 1/2$: $\displaystyle\int_0^\infty e^{-x^2}\, dx = \frac{\sqrt{\pi}}{2}$ *(the famous Gaussian integral!)*

---

## 📝 Practice Set

---

### Section A — Evaluating Gamma Functions

**Evaluate:**

1. $\Gamma(6)$

2. $\Gamma(7/2)$

3. $\Gamma(9/2)$

4. $\Gamma(1/2)\cdot\Gamma(3/2)$

5. $\dfrac{\Gamma(n+3)}{\Gamma(n)}$ &nbsp; *(simplify in terms of $n$)*

6. $\displaystyle\int_0^\infty e^{-x} x^4\, dx$

7. $\displaystyle\int_0^\infty e^{-2x} x^3\, dx$ &nbsp; *(Hint: substitute $t = 2x$)*

8. $\displaystyle\int_0^\infty e^{-x^2} x^4\, dx$

9. $\displaystyle\int_0^\infty e^{-x^3} x^2\, dx$

10. $\displaystyle\int_0^\infty x^{1/2} e^{-x}\, dx$

---

### Section B — Evaluating Beta Functions

**Evaluate using the definition directly:**

11. $B(3, 4)$

12. $B(1/2, 1/2)$

13. $B(2, 5)$

14. $B(3/2, 5/2)$

**Evaluate using the relation $B(m,n) = \dfrac{\Gamma(m)\Gamma(n)}{\Gamma(m+n)}$:**

15. $B(4, 3)$

16. $B(1/3, 2/3)$

17. $B(5/2, 3/2)$

18. $B(n, 1)$ &nbsp; *(simplify — what well-known fraction do you get?)*

---

### Section C — Integrals via Beta/Gamma

**Convert to Beta or Gamma form and evaluate:**

19. $\displaystyle\int_0^1 x^3(1-x)^4\, dx$

20. $\displaystyle\int_0^1 x^{1/2}(1-x)^{3/2}\, dx$

21. $\displaystyle\int_0^1 \sqrt[3]{x}(1-x)^{2/3}\, dx$

22. $\displaystyle\int_0^1 x^{m-1}(1-x^n)\, dx$ &nbsp; *(express in terms of $m$, $n$)*

**Using the trigonometric form of Beta:**

23. $\displaystyle\int_0^{\pi/2} \sin^4\theta\cos^6\theta\, d\theta$

24. $\displaystyle\int_0^{\pi/2} \sin^5\theta\, d\theta$

25. $\displaystyle\int_0^{\pi/2} \cos^7\theta\, d\theta$

26. $\displaystyle\int_0^{\pi/2} \sqrt{\tan\theta}\, d\theta$ &nbsp; *(Hint: write $\tan^{1/2}\theta = \sin^{1/2}\theta\cos^{-1/2}\theta$)*

27. $\displaystyle\int_0^{\pi/2} \sqrt{\sin\theta}\, d\theta$

28. $\displaystyle\int_0^{\pi/2} \dfrac{d\theta}{\sqrt{\sin\theta}}$

---

### Section D — Alternate Forms and Substitutions

**Use the substitution $x = t^2$ or $x = t^n$ to convert to Gamma form:**

29. $\displaystyle\int_0^\infty e^{-x^2} x^5\, dx$

30. $\displaystyle\int_0^\infty x^{1/3} e^{-x^{2/3}}\, dx$

31. $\displaystyle\int_0^1 \left(\ln\frac{1}{x}\right)^3\, dx$ &nbsp; *(Hint: let $x = e^{-t}$)*

32. $\displaystyle\int_0^1 x^4\left(\ln\frac{1}{x}\right)^2\, dx$

33. $\displaystyle\int_0^\infty \frac{x^{m-1}}{1+x}\, dx = \frac{\pi}{\sin(m\pi)}$ — verify this for $m = 1/2$ using the Beta function alternate form.

---

### Section E — Mixed and Challenge Problems

34. Show that $\Gamma(1/2) = \sqrt{\pi}$ using the substitution $x = t^2$ and the Gaussian integral.

35. Prove the duplication formula:
$$\Gamma(m)\,\Gamma\!\left(m + \tfrac{1}{2}\right) = \frac{\sqrt{\pi}}{2^{2m-1}}\,\Gamma(2m)$$
for $m = 1$ as a numerical verification.

36. Evaluate $\displaystyle\int_0^1 \frac{x^7 - 1}{\ln x}\, dx$.
*(Hint: write $x^7 - 1 = \int_0^7 x^t \ln x\, dt$ and interchange the order.)*

37. Find the value of $n$ if $\displaystyle\int_0^1 x^n (1-x)^3\, dx = \dfrac{1}{280}$.

38. **[Challenge]** Show that:
$$\int_0^{\pi/2} \sin^n\theta\, d\theta = \begin{cases} \dfrac{(n-1)!!}{n!!}\cdot\dfrac{\pi}{2} & \text{if } n \text{ even} \\[8pt] \dfrac{(n-1)!!}{n!!} & \text{if } n \text{ odd} \end{cases}$$
using the Beta function, where $n!! = n(n-2)(n-4)\cdots$.

---

> **Strategy tip:** When you see $\int x^a (1-x)^b\, dx$ on $[0,1]$, think Beta. When you see $\int x^a e^{-bx}\, dx$ on $[0,\infty)$, think Gamma. Trig integrals on $[0, \pi/2]$ with powers of $\sin$ and $\cos$ — use the trig form of Beta.
