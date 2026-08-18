# Unit 5 — Vector Functions and Their Derivatives
> MATH 104 Advanced Calculus · Kathmandu University

---

## 🎯 YouTube Search Topics

| Topic | Search Query |
|---|---|
| Vector valued functions intro | `vector valued functions calculus` |
| Derivatives of vector functions | `derivative vector function tangent vector` |
| Arc length parameterization | `arc length parameterization curve` |
| Unit tangent vector | `unit tangent vector curvature` |
| Curvature | `curvature formula explained` |
| TNB frame (Frenet-Serret) | `TNB frame frenet serret` or `binormal torsion explained` |
| Components of acceleration | `tangential normal acceleration components` |

---

## 📖 Core Concepts

### 5.1 Vector Functions

A vector function maps scalars to vectors:
$$\vec{r}(t) = f(t)\hat{i} + g(t)\hat{j} + h(t)\hat{k}$$

The **range** is a curve $C$ in space, parameterized by $t$.

### 5.2 Limits and Continuity

$$\lim_{t \to a} \vec{r}(t) = \left(\lim_{t\to a} f(t)\right)\hat{i} + \left(\lim_{t\to a} g(t)\right)\hat{j} + \left(\lim_{t\to a} h(t)\right)\hat{k}$$

Continuous if each component is continuous.

### 5.3 Derivatives and Integrals

$$\vec{r}'(t) = f'(t)\hat{i} + g'(t)\hat{j} + h'(t)\hat{k}$$

$\vec{r}'(t)$ is the **velocity** (tangent vector); $|\vec{r}'(t)|$ is the **speed**.

**Differentiation rules** (same as scalar, but order matters for cross product):
- $\frac{d}{dt}[\vec{u} \times \vec{v}] = \vec{u}' \times \vec{v} + \vec{u} \times \vec{v}'$

**Integral:**
$$\int \vec{r}(t)\, dt = \left(\int f\, dt\right)\hat{i} + \left(\int g\, dt\right)\hat{j} + \left(\int h\, dt\right)\hat{k} + \vec{C}$$

### 5.4 Arc Length

For a smooth curve from $t = a$ to $t = b$:
$$L = \int_a^b |\vec{r}'(t)|\, dt = \int_a^b \sqrt{[f'(t)]^2 + [g'(t)]^2 + [h'(t)]^2}\, dt$$

**Arc length parameter:** $s(t) = \int_a^t |\vec{r}'(\tau)|\, d\tau$, so $\frac{ds}{dt} = |\vec{r}'(t)|$.

### 5.5 Unit Tangent Vector and Curvature

$$\hat{T} = \frac{\vec{r}'}{|\vec{r}'|}$$

**Curvature:**
$$\kappa = \left|\frac{d\hat{T}}{ds}\right| = \frac{|\vec{r}' \times \vec{r}''|}{|\vec{r}'|^3} = \frac{|\hat{T}'|}{|\vec{r}'|}$$

**Principal Unit Normal:**
$$\hat{N} = \frac{\hat{T}'}{|\hat{T}'|}$$

($\hat{N}$ points toward the center of curvature — the direction the curve is turning.)

### 5.6 Binormal Vector and Torsion

$$\hat{B} = \hat{T} \times \hat{N} \qquad \text{(binormal vector)}$$

$$\tau = -\frac{d\hat{B}}{ds} \cdot \hat{N} \qquad \text{(torsion — measures how much curve twists out of its osculating plane)}$$

**Frenet-Serret formulas:**
$$\frac{d\hat{T}}{ds} = \kappa\hat{N}, \qquad \frac{d\hat{N}}{ds} = -\kappa\hat{T} + \tau\hat{B}, \qquad \frac{d\hat{B}}{ds} = -\tau\hat{N}$$

**Radius of curvature:** $\rho = 1/\kappa$

**Circle of curvature** (osculating circle): center at $\vec{r}(t_0) + \rho\hat{N}(t_0)$, radius $\rho$.

### 5.7 Tangential and Normal Components of Acceleration

$$\vec{a} = a_T\hat{T} + a_N\hat{N}$$

$$a_T = \frac{d^2s}{dt^2} = \frac{\vec{v} \cdot \vec{a}}{|\vec{v}|}, \qquad a_N = \kappa\left(\frac{ds}{dt}\right)^2 = \frac{|\vec{v} \times \vec{a}|}{|\vec{v}|}$$

Alternatively: $a_N = \sqrt{|\vec{a}|^2 - a_T^2}$.

---

## 📝 Practice Set

---

### Section A — Limits, Continuity, and Domains

1. Find the domain of $\vec{r}(t) = \dfrac{1}{t-1}\hat{i} + \ln(t+1)\hat{j} + \sqrt{t}\,\hat{k}$.

2. Evaluate $\displaystyle\lim_{t \to 0} \left[\frac{\sin t}{t}\hat{i} + e^t\hat{j} + \frac{1-\cos t}{t}\hat{k}\right]$.

3. Is $\vec{r}(t) = \cos t\,\hat{i} + \sin t\,\hat{j} + t\hat{k}$ continuous everywhere? What curve does it trace?

4. Find $\displaystyle\lim_{t \to \infty} \left[e^{-t}\hat{i} + \frac{t}{t+1}\hat{j} + t\sin(1/t)\hat{k}\right]$.

---

### Section B — Derivatives and Integrals

**Find $\vec{r}'(t)$ and $\vec{r}''(t)$:**

5. $\vec{r}(t) = t^3\hat{i} - 2t^2\hat{j} + \sin t\,\hat{k}$

6. $\vec{r}(t) = e^{2t}\hat{i} + t\ln t\,\hat{j} + \hat{k}$

7. $\vec{r}(t) = \sec t\,\hat{i} + \tan t\,\hat{j} + t\hat{k}$

**Evaluate the derivative using product/dot/cross rules:**

8. If $\vec{u}(t) = (t, t^2, t^3)$ and $\vec{v}(t) = (\cos t, \sin t, 0)$, find $\dfrac{d}{dt}[\vec{u} \cdot \vec{v}]$.

9. Find $\dfrac{d}{dt}[\vec{u} \times \vec{v}]$ for $\vec{u} = t\hat{i} + 2t^2\hat{j}$ and $\vec{v} = \hat{i} - t\hat{k}$.

10. If $|\vec{r}(t)| = c$ (constant), show that $\vec{r}(t) \perp \vec{r}'(t)$.

**Integrate:**

11. $\displaystyle\int_0^1 (t\hat{i} + e^t\hat{j} + \sin\pi t\,\hat{k})\, dt$

12. Find $\vec{r}(t)$ given $\vec{r}'(t) = 2t\hat{i} + e^t\hat{j} + \cos t\,\hat{k}$ and $\vec{r}(0) = \hat{i} - \hat{j}$.

---

### Section C — Arc Length and Speed

**Find the arc length of the curve:**

13. $\vec{r}(t) = 2t\hat{i} + (1-t)\hat{j} + (3+2t)\hat{k}$, from $t = 0$ to $t = 1$.

14. $\vec{r}(t) = \cos t\,\hat{i} + \sin t\,\hat{j} + t\hat{k}$, from $t = 0$ to $t = 2\pi$. *(This is a helix — what does the length tell you geometrically?)*

15. $\vec{r}(t) = (t^2/2)\hat{i} + (2t^{3/2}/3)\hat{j}$, from $t = 0$ to $t = 4$.

16. $\vec{r}(t) = e^t\hat{i} + e^{-t}\hat{j} + \sqrt{2}\,t\hat{k}$, from $t = 0$ to $t = 1$.

**Speed:**

17. A particle moves along $\vec{r}(t) = (t^2 - 1)\hat{i} + 2t\hat{j}$. Find its speed at $t = 2$.

18. At what $t$ is the speed of $\vec{r}(t) = t\hat{i} + t^2\hat{j} + t^3\hat{k}$ minimum?

---

### Section D — Unit Tangent Vector

**Find $\hat{T}(t)$ and evaluate at the given point:**

19. $\vec{r}(t) = \cos t\,\hat{i} + \sin t\,\hat{j} + t\hat{k}$ at $t = \pi/4$.

20. $\vec{r}(t) = e^t\hat{i} + e^{-t}\hat{j} + \sqrt{2}\,t\hat{k}$ at $t = 0$.

21. $\vec{r}(t) = (2\cos t)\hat{i} + (2\sin t)\hat{j} + (\sqrt{5}\,t)\hat{k}$ at $t = \pi/2$.

22. $\vec{r}(t) = t^2\hat{i} + (2t/3)\hat{j}$ at $t = 1$.

---

### Section E — Curvature and Normal Vector

**Find the curvature $\kappa(t)$:**

23. $\vec{r}(t) = t\hat{i} + \sin t\,\hat{j}$ at $t = \pi/2$.

24. $\vec{r}(t) = t\hat{i} + t^2\hat{j}$ — find $\kappa(t)$ and determine where curvature is maximum.

25. $\vec{r}(t) = (2\cos t)\hat{i} + (2\sin t)\hat{j} + t\hat{k}$.

26. $\vec{r}(t) = e^t\hat{i} + e^{-t}\hat{j}$ at $t = 0$.

**Find the principal unit normal $\hat{N}(t)$:**

27. $\vec{r}(t) = \cos t\,\hat{i} + \sin t\,\hat{j}$.

28. $\vec{r}(t) = t\hat{i} + \frac{t^2}{2}\hat{j}$ at $t = 1$.

**Osculating circle:**

29. Find the center and radius of the osculating circle for $y = \sin x$ at $x = 0$.

30. Find the curvature of $y = x^2$ at $(0,0)$ and at $(1,1)$.

---

### Section F — Binormal Vector and Torsion

31. For the helix $\vec{r}(t) = a\cos t\,\hat{i} + a\sin t\,\hat{j} + bt\hat{k}$:
    - (a) Find $\hat{T}$, $\hat{N}$, $\hat{B}$
    - (b) Find curvature $\kappa$
    - (c) Find torsion $\tau$
    - (d) What happens to $\kappa$ and $\tau$ as $b \to 0$? As $a \to 0$?

32. Find the binormal vector $\hat{B}$ for $\vec{r}(t) = t\hat{i} + t^2\hat{j} + \frac{2}{3}t^3\hat{k}$ at $t = 0$.

33. Show that a curve has zero torsion everywhere if and only if it lies in a plane.

---

### Section G — Components of Acceleration

**Find $a_T$ (tangential) and $a_N$ (normal) components:**

34. $\vec{r}(t) = t\hat{i} + t^2\hat{j} + t^3\hat{k}$ at $t = 1$.

35. $\vec{r}(t) = \cos t\,\hat{i} + \sin t\,\hat{j} + t\hat{k}$ — find $a_T$ and $a_N$ for all $t$.

36. $\vec{r}(t) = e^t\hat{i} + e^{-t}\hat{j}$ at $t = 0$.

37. A particle has position $\vec{r}(t) = (t^2 + 1)\hat{i} + 2t\hat{j} + t^3\hat{k}$. At $t = 1$:
    - (a) Find velocity and acceleration.
    - (b) Find $a_T$ and $a_N$.
    - (c) Find $\kappa$.

38. **[Challenge]** A particle moves so that its speed is increasing. What can you say about the sign of $a_T$? What if the particle is moving in a circle of constant radius?

---

> **Tip:** When computing curvature for a plane curve $y = f(x)$, use the formula:
> $$\kappa = \frac{|f''|}{(1 + f'^2)^{3/2}}$$
> For space curves, $\kappa = |\vec{r}' \times \vec{r}''| / |\vec{r}'|^3$ is almost always faster than computing $\hat{T}$ first.
