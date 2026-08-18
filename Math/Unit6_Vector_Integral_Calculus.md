# Unit 6 — Vector Integral Calculus
> MATH 104 Advanced Calculus · Kathmandu University

---

## 🎯 YouTube Search Topics

| Topic | Search Query |
|---|---|
| Line integrals intuition | `line integrals intuition 3blue1brown` |
| Conservative vector fields | `conservative vector field potential function` |
| Green's theorem visual | `green's theorem intuition` |
| Divergence theorem | `divergence theorem explained` |
| Stokes' theorem | `stokes theorem intuition visual` |
| Surface integrals | `surface integrals flux calculus` |
| Curl of a vector field | `curl vector field explanation` |

> **3Blue1Brown note:** His *"Divergence and Curl"* video is exceptionally good for building intuition. Search `3blue1brown divergence curl`.

---

## 📖 Core Concepts

### 6.1 Line Integrals of Scalar Functions

For a curve $C$ parametrized by $\vec{r}(t)$, $a \leq t \leq b$:
$$\int_C f\, ds = \int_a^b f(\vec{r}(t))\, |\vec{r}'(t)|\, dt$$

### 6.2 Line Integrals of Vector Fields

$$\int_C \vec{F} \cdot d\vec{r} = \int_a^b \vec{F}(\vec{r}(t)) \cdot \vec{r}'(t)\, dt$$

This equals the **work** done by $\vec{F}$ along $C$.

**Flux** (in 2D, with $\vec{F} = M\hat{i} + N\hat{j}$):
$$\text{Flux} = \oint_C M\, dy - N\, dx$$

**Circulation:**
$$\text{Circulation} = \oint_C \vec{F} \cdot d\vec{r} = \oint_C M\, dx + N\, dy$$

### 6.3 Path Independence and Conservative Fields

$\vec{F}$ is **conservative** on $D$ iff $\vec{F} = \nabla f$ for some scalar $f$ (potential function).

**Test for conservativeness** (in 2D, simply connected domain):
$$\vec{F} = M\hat{i} + N\hat{j} \text{ is conservative} \iff \frac{\partial M}{\partial y} = \frac{\partial N}{\partial x}$$

In 3D:
$$\vec{F} \text{ is conservative} \iff \nabla \times \vec{F} = \vec{0}$$

**Fundamental Theorem for Line Integrals:**
$$\int_C \nabla f \cdot d\vec{r} = f(B) - f(A)$$

### 6.4 Divergence and Curl

$$\text{div}\,\vec{F} = \nabla \cdot \vec{F} = \frac{\partial M}{\partial x} + \frac{\partial N}{\partial y} + \frac{\partial P}{\partial z}$$

$$\text{curl}\,\vec{F} = \nabla \times \vec{F} = \begin{vmatrix} \hat{i} & \hat{j} & \hat{k} \\ \partial_x & \partial_y & \partial_z \\ M & N & P \end{vmatrix}$$

**Circulation density** (in 2D): $\dfrac{\partial N}{\partial x} - \dfrac{\partial M}{\partial y}$

### 6.5 Green's Theorem

For a simple closed curve $C$ (positively oriented) bounding region $D$:
$$\oint_C M\, dx + N\, dy = \iint_D \left(\frac{\partial N}{\partial x} - \frac{\partial M}{\partial y}\right) dA$$

**Area via Green's theorem:**
$$\text{Area}(D) = \frac{1}{2}\oint_C x\, dy - y\, dx$$

### 6.6 Surface Integrals

For surface $S$ parametrized by $\vec{r}(u,v)$:
$$\iint_S f\, dS = \iint_D f(\vec{r}(u,v))\, |\vec{r}_u \times \vec{r}_v|\, dA$$

**Flux through $S$:**
$$\iint_S \vec{F} \cdot d\vec{S} = \iint_D \vec{F} \cdot (\vec{r}_u \times \vec{r}_v)\, dA$$

### 6.7 Divergence Theorem (Gauss's Theorem)

For closed surface $S$ bounding volume $V$:
$$\oiint_S \vec{F} \cdot d\vec{S} = \iiint_V (\nabla \cdot \vec{F})\, dV$$

### 6.8 Stokes' Theorem

For surface $S$ bounded by curve $C$ (right-hand rule for orientation):
$$\oint_C \vec{F} \cdot d\vec{r} = \iint_S (\nabla \times \vec{F}) \cdot d\vec{S}$$

---

## 📝 Practice Set

---

### Section A — Parametrizing Curves

**Parametrize the following paths:**

1. Line segment from $(0,0,0)$ to $(1,2,3)$.
2. Circle $x^2 + y^2 = 4$ traversed counterclockwise.
3. The parabola $y = x^2$ from $(0,0)$ to $(2,4)$.
4. The quarter-circle from $(1,0)$ to $(0,1)$ counterclockwise.
5. The curve of intersection of $z = x^2 + y^2$ and $x + y = 1$ — parametrize using $x = t$.

---

### Section B — Line Integrals (Scalar)

6. Evaluate $\displaystyle\int_C (x^2 + y^2)\, ds$ where $C$ is the line segment from $(0,0)$ to $(1,1)$.

7. $\displaystyle\int_C xy\, ds$ where $C$ is the arc of the circle $x^2 + y^2 = 4$ in the first quadrant.

8. $\displaystyle\int_C \sqrt{x^2+y^2+z^2}\, ds$ where $C: \vec{r}(t) = \cos t\,\hat{i} + \sin t\,\hat{j} + t\hat{k}$, $0 \leq t \leq 2\pi$.

9. Find the mass of a wire in the shape of $x^2 + y^2 = 1$, $z = 2$ if its density is $\delta(x,y,z) = 2 + x + y$.

---

### Section C — Line Integrals (Vector Fields)

**Evaluate $\displaystyle\int_C \vec{F} \cdot d\vec{r}$:**

10. $\vec{F} = xy\hat{i} + y^2\hat{j}$, along the parabola $y = x^2$ from $(0,0)$ to $(1,1)$.

11. $\vec{F} = y\hat{i} - x\hat{j}$, around the circle $x^2 + y^2 = 1$ counterclockwise.

12. $\vec{F} = x^2\hat{i} + xy\hat{j} + z\hat{k}$, along $\vec{r}(t) = t\hat{i} + t^2\hat{j} + t^3\hat{k}$, $0 \leq t \leq 1$.

13. $\vec{F} = (y^2)\hat{i} + (x^2)\hat{j}$, along the path from $(0,0)$ to $(1,1)$: (a) straight line, (b) $y = x^2$. Are the answers the same?

14. Find the work done by $\vec{F} = 2x\hat{i} + y\hat{j}$ along the path $C$: straight line from $(0,0)$ to $(2,3)$.

---

### Section D — Conservative Fields and Potential Functions

**Determine if conservative; if so, find the potential function:**

15. $\vec{F} = (2x + y)\hat{i} + (x + 3y)\hat{j}$

16. $\vec{F} = y\hat{i} + x\hat{j}$

17. $\vec{F} = (y^2)\hat{i} + (2xy)\hat{j}$

18. $\vec{F} = (e^x\cos y)\hat{i} - (e^x\sin y)\hat{j}$

19. $\vec{F} = (yz)\hat{i} + (xz)\hat{j} + (xy)\hat{k}$

20. $\vec{F} = (2x - 3)\hat{i} - z\hat{j} + (\cos z)\hat{k}$ &nbsp; *(from slides — is it conservative?)*

**Use the potential function to evaluate the line integral:**

21. $\displaystyle\int_C 2x\, dx + 2y\, dy + 2z\, dz$ from $(0,0,0)$ to $(1,2,3)$ along any path.

22. $\displaystyle\int_C y\, dx + x\, dy$ from $(0,0)$ to $(2,4)$ along any path.

23. Evaluate $\displaystyle\oint_C 2xy\, dx + (x^2 + 1)\, dy$ around any simple closed curve.

---

### Section E — Green's Theorem

**Use Green's theorem to evaluate:**

24. $\displaystyle\oint_C (y - x)\, dx + (2x - y)\, dy$ where $C$ is the triangle with vertices $(0,0)$, $(1,0)$, $(0,1)$, counterclockwise.

25. $\displaystyle\oint_C xy\, dx + x^2\, dy$ where $C$ is the boundary of the region between $y = x^2$ and $y = x$, counterclockwise.

26. $\displaystyle\oint_C y^2\, dx - x^2\, dy$ around the circle $x^2 + y^2 = 4$.

27. $\displaystyle\oint_C (x^2 - y)\, dx + (y^2 + x)\, dy$ around the ellipse $\frac{x^2}{4} + y^2 = 1$.

28. Use Green's theorem to find the area enclosed by the ellipse $\frac{x^2}{a^2} + \frac{y^2}{b^2} = 1$.

29. **Verification:** For $\vec{F} = -y\hat{i} + x\hat{j}$ and $C$: unit circle, verify Green's theorem directly by computing both sides.

---

### Section F — Surface Integrals

30. Evaluate $\displaystyle\iint_S (x + y + z)\, dS$ where $S$ is the part of the plane $z = 1 - x - y$ in the first octant.

31. Evaluate $\displaystyle\iint_S z\, dS$ where $S$ is the hemisphere $x^2 + y^2 + z^2 = 4$, $z \geq 0$.

32. Find the surface area of the part of the paraboloid $z = 1 - x^2 - y^2$ above the $xy$-plane.

**Flux integrals:**

33. Find the flux of $\vec{F} = z\hat{i} + y\hat{j} + x\hat{k}$ through the sphere $x^2 + y^2 + z^2 = 4$ (outward normal).

34. Find the flux of $\vec{F} = x\hat{i} + y\hat{j} + z\hat{k}$ through the cube $[0,1]^3$ (outward normals on all six faces).

---

### Section G — Divergence Theorem

**Use the Divergence Theorem to compute the flux:**

35. $\vec{F} = x^2\hat{i} + y^2\hat{j} + z^2\hat{k}$ through the surface of the unit cube $[0,1]^3$.

36. $\vec{F} = xy\hat{i} + yz\hat{j} + zx\hat{k}$ through the sphere $x^2 + y^2 + z^2 = 1$.

37. $\vec{F} = z\hat{i} + y\hat{j} + x\hat{k}$ through the closed cylinder $x^2 + y^2 \leq 1$, $0 \leq z \leq 2$.

38. $\vec{F} = (x^3 + y^3)\hat{i} + (y^3 + z^3)\hat{j} + (z^3 + x^3)\hat{k}$ through the sphere $x^2 + y^2 + z^2 = 4$.

---

### Section H — Stokes' Theorem

**Use Stokes' theorem to evaluate $\oint_C \vec{F} \cdot d\vec{r}$:**

39. $\vec{F} = y^2\hat{i} + x\hat{j} + z^2\hat{k}$, $C$ is the boundary of the triangle with vertices $(1,0,0)$, $(0,1,0)$, $(0,0,1)$, oriented counterclockwise from above.

40. $\vec{F} = -y^2\hat{i} + x\hat{j} + z^2\hat{k}$, $C$ is the circle $x^2 + y^2 = 1$ in the plane $z = 3$, counterclockwise when viewed from above.

41. $\vec{F} = (y-z)\hat{i} + (z-x)\hat{j} + (x-y)\hat{k}$, $C$ is the boundary of the part of the plane $2x + y + z = 2$ in the first octant.

42. **Verification:** Take $\vec{F} = z\hat{i} + x\hat{j} + y\hat{k}$ and $S$: the portion of the paraboloid $z = 1 - x^2 - y^2$ above the $xy$-plane with $C$ being the circle $x^2+y^2 = 1$, $z = 0$. Verify Stokes' theorem by computing both sides.

---

### Section I — Challenge

43. Show that $\iint_S \nabla f \times \nabla g \cdot d\vec{S} = \oint_C f\, \nabla g \cdot d\vec{r}$ using Stokes' theorem.

44. A fluid has velocity field $\vec{v} = (x^2 + y^2)\hat{k}$. Find the flux of $\vec{v}$ upward through the paraboloid $z = 4 - x^2 - y^2$ above the $xy$-plane using (a) direct surface integral and (b) Divergence Theorem.

45. Use Green's theorem to show that if $f$ is harmonic ($\nabla^2 f = 0$) in a region $D$, then $\oint_C \frac{\partial f}{\partial n}\, ds = 0$ for any simple closed curve $C$ in $D$.

---

> **The Big Picture:** All three major theorems (Green's, Stokes', Divergence) are versions of the same idea — integrating a "derivative" over a region equals integrating the original over its boundary. Green's is 2D Stokes'. Both are special cases of the generalized Stokes' theorem.
