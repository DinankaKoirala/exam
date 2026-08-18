# Unit 3 — Multiple Integrals
> MATH 104 Advanced Calculus · Kathmandu University

---

## 🎯 YouTube Search Topics

| Topic | Search Query |
|---|---|
| Double integrals intro | `double integrals intuition 3blue1brown` |
| Fubini's theorem | `fubini's theorem explained` |
| Changing order of integration | `switching order of integration` |
| Polar double integrals | `double integrals polar coordinates` |
| Triple integrals | `triple integrals cylindrical spherical` |
| Change of variables Jacobian | `Jacobian change of variables multiple integrals` |

---

## 📖 Core Concepts

### 3.1 Double Integrals

Over a rectangle $R = [a,b] \times [c,d]$:
$$\iint_R f(x,y)\, dA = \lim_{m,n \to \infty} \sum_{i=1}^m \sum_{j=1}^n f(x_{ij}^*, y_{ij}^*)\,\Delta A$$

### 3.2 Fubini's Theorem

If $f$ is continuous on $R = [a,b] \times [c,d]$:
$$\iint_R f(x,y)\, dA = \int_a^b \int_c^d f(x,y)\, dy\, dx = \int_c^d \int_a^b f(x,y)\, dx\, dy$$

For a general region $D$ of **Type I** (bounded by functions of $x$):
$$\iint_D f\, dA = \int_a^b \int_{g_1(x)}^{g_2(x)} f(x,y)\, dy\, dx$$

For **Type II** (bounded by functions of $y$):
$$\iint_D f\, dA = \int_c^d \int_{h_1(y)}^{h_2(y)} f(x,y)\, dx\, dy$$

### 3.3 Change of Order of Integration

Sketch the region first, then re-express the bounds. Critical step: always identify the actual region $D$ before rewriting limits.

### 3.4 Polar Double Integrals

$$\iint_R f(x,y)\, dA = \int_\alpha^\beta \int_{r_1(\theta)}^{r_2(\theta)} f(r\cos\theta, r\sin\theta)\, r\, dr\, d\theta$$

The extra $r$ is the **Jacobian** — don't forget it!

### 3.5 Triple Integrals

$$\iiint_D f(x,y,z)\, dV$$

**Cylindrical:** $dV = r\, dr\, d\theta\, dz$

**Spherical:** $dV = \rho^2 \sin\phi\, d\rho\, d\phi\, d\theta$

where $x = \rho\sin\phi\cos\theta$, $y = \rho\sin\phi\sin\theta$, $z = \rho\cos\phi$.

### 3.6 Substitution (Change of Variables)

For a transformation $x = g(u,v)$, $y = h(u,v)$:
$$\iint_R f(x,y)\, dA = \iint_S f(g,h)\, |J|\, du\, dv$$

where the Jacobian is:
$$J = \frac{\partial(x,y)}{\partial(u,v)} = \begin{vmatrix} x_u & x_v \\ y_u & y_v \end{vmatrix}$$

---

## 📝 Practice Set

---

### Section A — Double Integrals over Rectangles (Fubini's Theorem)

**Evaluate:**

1. $\displaystyle\int_0^1 \int_0^2 (x + 2y)\, dx\, dy$

2. $\displaystyle\int_1^e \int_0^1 \frac{x}{y}\, dx\, dy$

3. $\displaystyle\int_0^{\pi/2} \int_0^1 y\sin x\, dy\, dx$

4. $\displaystyle\int_0^1 \int_0^1 \frac{xy}{\sqrt{x^2+y^2+1}}\, dy\, dx$

5. Compute $\iint_R e^{x+y}\, dA$ where $R = [0,1] \times [0,1]$.

---

### Section B — Double Integrals over General Regions

**Sketch the region $D$ and evaluate:**

6. $\displaystyle\iint_D x^2y\, dA$, where $D$ is bounded by $y = x$, $y = 0$, $x = 1$.

7. $\displaystyle\iint_D (x + y)\, dA$, where $D$ is bounded by $y = x^2$ and $y = 2x$.

8. $\displaystyle\iint_D e^{x^2}\, dA$, where $D$ is bounded by $x = y$, $x = 1$, $y = 0$.
*(Hint: switch the order of integration.)*

9. $\displaystyle\iint_D xy\, dA$, where $D$ is the region in the first quadrant bounded by $y = x^2$ and $y = x$.

10. $\displaystyle\int_0^1 \int_x^1 \sin(y^2)\, dy\, dx$ &nbsp; *(change order of integration)*

---

### Section C — Changing Order of Integration

**Sketch the region and reverse the order of integration, then evaluate:**

11. $\displaystyle\int_0^1 \int_y^1 \frac{\sin x}{x}\, dx\, dy$

12. $\displaystyle\int_0^2 \int_{x^2}^4 x e^{y^2}\, dy\, dx$

13. $\displaystyle\int_0^1 \int_{\sqrt{x}}^1 e^{y^3}\, dy\, dx$

14. $\displaystyle\int_0^4 \int_{\sqrt{y}}^2 e^{x^3}\, dx\, dy$

---

### Section D — Polar Double Integrals

15. $\iint_D x^2 + y^2\, dA$, where $D$ is the disk $x^2 + y^2 \leq 4$.

16. $\iint_D e^{-(x^2+y^2)}\, dA$, where $D$ is the disk $x^2 + y^2 \leq 9$.

17. $\iint_D \sqrt{x^2 + y^2}\, dA$, where $D$ is the region in the first quadrant between $r = 1$ and $r = 3$.

18. Find the area of the region bounded by $r = 2 + 2\cos\theta$ using a double integral.

19. Evaluate $\displaystyle\int_{-2}^{2} \int_0^{\sqrt{4-x^2}} (x^2 + y^2)^{3/2}\, dy\, dx$ by converting to polar.

20. Find $\iint_D \dfrac{1}{(x^2+y^2)^2}\, dA$ where $D: 1 \leq x^2+y^2 \leq 4$, $y \geq 0$.

---

### Section E — Triple Integrals (Rectangular)

21. $\displaystyle\int_0^1 \int_0^2 \int_0^3 xyz\, dx\, dy\, dz$

22. $\displaystyle\iiint_E z\, dV$ where $E = \{(x,y,z) \mid 0 \leq x \leq 1,\ 0 \leq y \leq 1,\ 0 \leq z \leq x+y\}$

23. Find the volume of the tetrahedron bounded by the planes $x = 0$, $y = 0$, $z = 0$, and $x + y + z = 1$.

24. $\displaystyle\iiint_E (x^2 + y^2)\, dV$ where $E$ is bounded by $z = 0$ and $z = 4 - x^2 - y^2$.

---

### Section F — Triple Integrals (Cylindrical & Spherical)

**Set up and evaluate using cylindrical coordinates:**

25. $\iiint_E \sqrt{x^2+y^2}\, dV$ where $E$ is the region inside the cylinder $x^2+y^2=4$ between $z=0$ and $z=3$.

26. Find the volume of the solid bounded by $z = x^2 + y^2$ (paraboloid) and $z = 4$ (plane).

27. $\displaystyle\int_{-2}^{2}\int_{-\sqrt{4-x^2}}^{\sqrt{4-x^2}}\int_{\sqrt{x^2+y^2}}^{2} z\, dz\, dy\, dx$ — convert to cylindrical.

**Set up and evaluate using spherical coordinates:**

28. $\iiint_E e^{(x^2+y^2+z^2)^{3/2}}\, dV$ where $E$ is the unit ball $x^2+y^2+z^2 \leq 1$.

29. Find the volume of the solid that lies between the spheres $x^2+y^2+z^2 = 1$ and $x^2+y^2+z^2 = 4$.

30. $\iiint_E \dfrac{1}{\sqrt{x^2+y^2+z^2}}\, dV$ where $E$ is the region $1 \leq x^2+y^2+z^2 \leq 4$.

---

### Section G — Substitution and Jacobian

31. Use the substitution $u = x + y$, $v = x - y$ to evaluate $\iint_R (x-y)e^{x^2-y^2}\, dA$ where $R$ is the square with vertices $(0,0)$, $(1,1)$, $(2,0)$, $(1,-1)$.

32. Compute $\iint_R e^{(x+y)/(x-y)}\, dA$ where $R$ is the trapezoidal region with vertices $(1,0)$, $(2,0)$, $(0,-2)$, $(0,-1)$ using appropriate substitution.

33. **[Challenge]** Find the volume enclosed by the ellipsoid $\dfrac{x^2}{a^2} + \dfrac{y^2}{b^2} + \dfrac{z^2}{c^2} = 1$ using the substitution $x = a\rho\sin\phi\cos\theta$, etc. *(Answer should be $\frac{4}{3}\pi abc$.)*

---

> **Key reminder:** In polar coordinates, $dA = r\, dr\, d\theta$ — the $r$ factor comes from the Jacobian of the transformation. In cylindrical, $dV = r\, dr\, d\theta\, dz$. In spherical, $dV = \rho^2\sin\phi\, d\rho\, d\phi\, d\theta$.
