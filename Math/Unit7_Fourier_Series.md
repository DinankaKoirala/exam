# Unit 7 — Fourier Series
> MATH 104 Advanced Calculus · Kathmandu University

---

## 🎯 YouTube Search Topics

| Topic | Search Query |
|---|---|
| Fourier series visual | `fourier series 3blue1brown` — **must watch** |
| Fourier series derivation | `fourier series euler formula derivation` |
| Odd and even functions Fourier | `odd even function fourier series` |
| Half-range expansions | `fourier half range sine cosine expansion` |
| Fourier convergence theorem | `dirichlet convergence fourier series` |
| Fourier as circles (visual) | `fourier transform circles animation` |

> **3Blue1Brown note:** *"But what is a Fourier series?"* is one of the best math videos ever made — search it by name directly.

---

## 📖 Core Concepts

### 7.1 Periodic Functions

$f(x)$ is periodic with period $T$ if $f(x + T) = f(x)$ for all $x$.

**Primitive period**: the smallest positive period.

**Key facts:**
- $\sin nx$ and $\cos nx$ have period $2\pi/n$
- If $f$ and $g$ have period $T$, so does $af + bg$
- Constants and $f(x) = 0$ are periodic with every $T$ (no primitive period)

### 7.2 Trigonometric Series & Fourier Series

The Fourier series of a function $f(x)$ with period $2\pi$:
$$f(x) = \frac{a_0}{2} + \sum_{n=1}^\infty (a_n \cos nx + b_n \sin nx)$$

**Euler's Formulae** (Fourier coefficients):
$$a_0 = \frac{1}{\pi}\int_{-\pi}^{\pi} f(x)\, dx$$
$$a_n = \frac{1}{\pi}\int_{-\pi}^{\pi} f(x)\cos nx\, dx \qquad (n = 1, 2, 3, \ldots)$$
$$b_n = \frac{1}{\pi}\int_{-\pi}^{\pi} f(x)\sin nx\, dx \qquad (n = 1, 2, 3, \ldots)$$

**Useful orthogonality integrals:**
$$\int_{-\pi}^\pi \sin nx\, dx = 0, \quad \int_{-\pi}^\pi \cos nx\, dx = 0$$
$$\int_{-\pi}^\pi \sin mx\cos nx\, dx = 0 \text{ (always)}$$
$$\int_{-\pi}^\pi \sin mx\sin nx\, dx = \begin{cases} \pi & m = n \\ 0 & m \neq n \end{cases}$$
$$\int_{-\pi}^\pi \cos mx\cos nx\, dx = \begin{cases} \pi & m = n \\ 0 & m \neq n \end{cases}$$

### 7.3 Convergence Theorem (Dirichlet)

If $f$ is piecewise smooth on $[-\pi, \pi]$, then its Fourier series converges:
- To $f(x)$ at every point where $f$ is continuous
- To $\dfrac{f(x^+) + f(x^-)}{2}$ at jump discontinuities

### 7.1 Odd and Even Functions

| Property | Even $f(-x) = f(x)$ | Odd $f(-x) = -f(x)$ |
|---|---|---|
| $b_n$ | $= 0$ (no sine terms) | — |
| $a_0, a_n$ | — | $= 0$ (no cosine terms) |
| $\int_{-L}^L f\, dx$ | $= 2\int_0^L f\, dx$ | $= 0$ |

Product rules: even × even = even, odd × odd = even, even × odd = **odd**.

### 7.4 Arbitrary Period $2L$

For $f$ with period $2L$:
$$f(x) = \frac{a_0}{2} + \sum_{n=1}^\infty \left(a_n \cos\frac{n\pi x}{L} + b_n \sin\frac{n\pi x}{L}\right)$$

$$a_n = \frac{1}{L}\int_{-L}^{L} f(x)\cos\frac{n\pi x}{L}\, dx, \qquad b_n = \frac{1}{L}\int_{-L}^{L} f(x)\sin\frac{n\pi x}{L}\, dx$$

### 7.5 Half-Range Expansions

For a function defined on $[0, L]$, extend it as:

**Cosine series** (even extension to $[-L, L]$, then periodic): only $a_n$ terms.
$$a_n = \frac{2}{L}\int_0^L f(x)\cos\frac{n\pi x}{L}\, dx$$

**Sine series** (odd extension to $[-L, L]$, then periodic): only $b_n$ terms.
$$b_n = \frac{2}{L}\int_0^L f(x)\sin\frac{n\pi x}{L}\, dx$$

---

## 📝 Practice Set

---

### Section A — Periodic Functions

**Find the primitive period:**

1. $f(x) = \cos 3x$
2. $f(x) = \sin(2x + 5)$
3. $f(x) = \cos 2x + \sin 3x$ &nbsp; *(period of a sum — use LCM of individual periods)*
4. $f(x) = |\sin x|$
5. $f(x) = \tan 2x$

**Determine if the function is odd, even, or neither:**

6. $f(x) = x^3 + x$
7. $f(x) = x^2\cos x$
8. $f(x) = x\sin^2 x$
9. $f(x) = e^x$
10. $f(x) = x^2 + 2x$

---

### Section B — Fourier Series (Period $2\pi$)

**Find the Fourier series of:**

11. $f(x) = x$, $-\pi < x < \pi$; $f(x + 2\pi) = f(x)$.

12. $f(x) = |x|$, $-\pi < x < \pi$; $f(x + 2\pi) = f(x)$.
*(Hint: even function — so only $a_n$ terms.)*

13. $f(x) = x^2$, $-\pi < x < \pi$; $f(x + 2\pi) = f(x)$.

14. $f(x) = \begin{cases} 0, & -\pi < x < 0 \\ 1, & 0 < x < \pi \end{cases}$; extended periodically.

15. $f(x) = \begin{cases} -1, & -\pi < x < 0 \\ 1, & 0 < x < \pi \end{cases}$; (square wave); extended periodically.

16. $f(x) = \begin{cases} 0, & -\pi < x < 0 \\ x, & 0 < x < \pi \end{cases}$; extended periodically.

17. $f(x) = e^x$, $-\pi < x < \pi$; extended periodically.

18. $f(x) = |\cos x|$, $-\pi < x < \pi$; extended periodically.

---

### Section C — Using Fourier Results to Sum Series

*(After finding the Fourier series, substitute special values of $x$ to derive famous series identities.)*

19. From the series for $f(x) = x$ on $(-\pi, \pi)$, derive:
$$1 - \frac{1}{3} + \frac{1}{5} - \frac{1}{7} + \cdots = \frac{\pi}{4}$$

20. From the series for $f(x) = x^2$ on $(-\pi, \pi)$, derive:
$$\frac{1}{1^2} + \frac{1}{2^2} + \frac{1}{3^2} + \cdots = \frac{\pi^2}{6}$$

21. From the series for $f(x) = |x|$ on $(-\pi, \pi)$, derive:
$$\frac{1}{1^2} + \frac{1}{3^2} + \frac{1}{5^2} + \cdots = \frac{\pi^2}{8}$$

22. Using Parseval's theorem (not required to prove):
$$\frac{1}{\pi}\int_{-\pi}^\pi [f(x)]^2\, dx = \frac{a_0^2}{2} + \sum_{n=1}^\infty (a_n^2 + b_n^2)$$
Apply this to $f(x) = x$ to derive $\displaystyle\sum_{n=1}^\infty \frac{1}{n^2} = \frac{\pi^2}{6}$.

---

### Section D — Fourier Series with Arbitrary Period $2L$

**Find the Fourier series of $f$ with the given period:**

23. $f(x) = x$, period $2L = 4$ (so $L = 2$), $-2 < x < 2$.

24. $f(x) = 1 - |x|/L$, period $2L$, $-L < x < L$.

25. $f(x) = \begin{cases} 0, & -2 < x < 0 \\ 1, & 0 < x < 2 \end{cases}$, period $4$.

26. $f(x) = x^2$, $0 < x < 2$, period $2$.

27. $f(x) = \sin\frac{\pi x}{L}$, $-L < x < L$, period $2L$. *(What do you expect before computing?)*

---

### Section E — Half-Range Expansions

**Find both the half-range sine and cosine series for $f$ on $[0, L]$:**

28. $f(x) = 1$, $0 < x < \pi$.
    - (a) Sine series
    - (b) Cosine series

29. $f(x) = x$, $0 < x < L$.
    - (a) Sine series
    - (b) Cosine series

30. $f(x) = x(\pi - x)$, $0 < x < \pi$.
    - (a) Sine series
    - (b) Cosine series

31. $f(x) = \cos x$, $0 < x < \pi$. Find the half-range sine series.

32. $f(x) = \begin{cases} x, & 0 < x < L/2 \\ L - x, & L/2 < x < L \end{cases}$. Find the full Fourier, half-range sine, and half-range cosine series.

---

### Section F — Convergence

**For each Fourier series found above:**

33. Sketch $f(x)$ and the function to which the Fourier series converges at discontinuities.

34. For the square wave (problem 15): at $x = 0$ and $x = \pi$, what does the Fourier series converge to?

35. For the series of $f(x) = x$ on $(-\pi, \pi)$: what does the series converge to at $x = \pi$?

36. **[Challenge]** Show by direct substitution that if $f(x) = x$ has the Fourier series
$$x = 2\left(\sin x - \frac{\sin 2x}{2} + \frac{\sin 3x}{3} - \cdots\right),$$
then at $x = \pi/2$ you get $\pi/4 = 1 - 1/3 + 1/5 - \cdots$.

---

### Section G — Mixed and Applied Problems

37. A function $f$ with period $6$ is defined by $f(x) = x^2 - 3$, $-3 < x < 3$. Find its Fourier series.

38. Find the Fourier series of $f(x) = e^{ax}$, $-\pi < x < \pi$, periodic with period $2\pi$. Then use it to find a closed form for $\displaystyle\sum_{n=1}^\infty \frac{1}{a^2 + n^2}$.

39. **[Challenge]** The sawtooth wave is $f(x) = x$ on $(-\pi, \pi)$, extended periodically. If you truncate the Fourier series after $N$ terms and plot it, you observe the "Gibbs phenomenon" — an overshoot of about $9\%$ near the jump. Use the formula for partial sums to explain qualitatively why this happens.

40. Find the half-range sine series for $f(x) = x(L-x)$ on $[0, L]$ and use it to evaluate:
$$\sum_{n=1, 3, 5, \ldots}^\infty \frac{1}{n^3}$$

---

> **Key Insight:** A Fourier series decomposes any periodic function into pure frequencies (harmonics). This is the mathematical foundation of signal processing, audio compression (MP3), image compression (JPEG), and solving PDEs in engineering — your future courses will build heavily on this.
