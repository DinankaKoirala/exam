# Unit 2 — Partial Derivatives
> MATH 104 Advanced Calculus · Kathmandu University

---

## 🎯 YouTube Search Topics

| Topic | Search Query |
|---|---|
| Functions of several variables | `multivariable functions domain range 3blue1brown` |
| Partial derivatives visual | `partial derivatives visualization` |
| Gradient vectors | `gradient vector field explained` |
| Directional derivatives | `directional derivative intuition` |
| Chain rule multivariable | `multivariable chain rule` |
| Tangent planes | `tangent plane to surface calculus` |
| Saddle points & extrema | `saddle point multivariable calculus` |
| Lagrange multipliers | `lagrange multipliers 3blue1brown` or `lagrange multipliers intuition` |

---

## 📖 Core Concepts

### 2.1 Functions of Several Variables

$f: D \subseteq \mathbb{R}^n \to \mathbb{R}$. Key vocabulary:

- **Interior point**: every neighborhood lies in $D$
- **Boundary point**: every neighborhood contains points inside and outside $D$
- **Open set**: contains only interior points
- **Closed set**: contains all its boundary points

**Level curves** of $f(x,y)$: the curves $f(x,y) = c$ in the $xy$-plane.

### 2.3 Partial Derivatives

$$f_x = \frac{\partial f}{\partial x} = \lim_{h \to 0} \frac{f(x+h, y) - f(x,y)}{h}$$

**Mixed Derivative Theorem (Clairaut's):** If $f_{xy}$ and $f_{yx}$ are both continuous, then $f_{xy} = f_{yx}$.

### 2.4 Chain Rule

For $w = f(x,y)$, $x = x(t)$, $y = y(t)$:
$$\frac{dw}{dt} = \frac{\partial w}{\partial x}\frac{dx}{dt} + \frac{\partial w}{\partial y}\frac{dy}{dt}$$

For $w = f(x,y)$, $x = x(s,t)$, $y = y(s,t)$:
$$\frac{\partial w}{\partial s} = \frac{\partial w}{\partial x}\frac{\partial x}{\partial s} + \frac{\partial w}{\partial y}\frac{\partial y}{\partial s}$$

### 2.5 Directional Derivative & Gradient

$$D_{\hat{u}} f = \nabla f \cdot \hat{u}$$

$$\nabla f = \frac{\partial f}{\partial x}\hat{i} + \frac{\partial f}{\partial y}\hat{j} + \frac{\partial f}{\partial z}\hat{k}$$

The gradient points in the direction of **steepest ascent**. $D_{\hat{u}}f$ is maximum when $\hat{u}$ is parallel to $\nabla f$.

### 2.6 Tangent Plane & Linearization

Tangent plane to $z = f(x,y)$ at $(x_0, y_0, z_0)$:
$$z - z_0 = f_x(x_0,y_0)(x - x_0) + f_y(x_0,y_0)(y - y_0)$$

Linearization (local linear approximation):
$$L(x,y) = f(x_0,y_0) + f_x(x_0,y_0)(x-x_0) + f_y(x_0,y_0)(y-y_0)$$

### 2.7 Extreme Values — Second Derivative Test

At a critical point where $f_x = f_y = 0$, compute the discriminant:
$$D = f_{xx}f_{yy} - f_{xy}^2$$

| Condition | Conclusion |
|---|---|
| $D > 0$, $f_{xx} > 0$ | Local minimum |
| $D > 0$, $f_{xx} < 0$ | Local maximum |
| $D < 0$ | Saddle point |
| $D = 0$ | Test inconclusive |

### 2.8 Lagrange Multipliers

To optimize $f(x,y)$ subject to $g(x,y) = 0$:
$$\nabla f = \lambda \nabla g$$

This gives the system: $f_x = \lambda g_x$, $f_y = \lambda g_y$, $g(x,y) = 0$.

---

## 📝 Practice Set

---

### Section A — Domains, Ranges, and Level Curves

**For each function, find: (a) domain, (b) range, (c) describe the level curves.**

1. $f(x,y) = \sqrt{4 - x^2 - y^2}$

2. $f(x,y) = \ln(x + y - 1)$

3. $f(x,y) = \dfrac{1}{x^2 + y^2}$

4. $f(x,y) = e^{x^2+y^2}$

5. $f(x,y,z) = x^2 + y^2 - z$ &nbsp; *(describe the level surfaces)*

---

### Section B — Limits and Continuity

**Find each limit or show it does not exist:**

6. $\displaystyle\lim_{(x,y) \to (0,0)} \frac{xy}{x^2 + y^2}$

7. $\displaystyle\lim_{(x,y) \to (0,0)} \frac{x^2 y}{x^4 + y^2}$

8. $\displaystyle\lim_{(x,y) \to (1,2)} \frac{x^2 + y^2 - 5}{x - 1}$

9. $\displaystyle\lim_{(x,y) \to (0,0)} \frac{x^2 - y^2}{\sqrt{x^2+y^2}}$ &nbsp; *(Does it exist?)*

10. $\displaystyle\lim_{(x,y,z) \to (0,0,0)} \frac{xy + yz}{x^2 + y^2 + z^2}$

---

### Section C — Partial Derivatives

**Find $f_x$, $f_y$ (and $f_z$ if applicable):**

11. $f(x,y) = x^3y^2 - 3xy + 7$

12. $f(x,y) = e^{x\sin y}$

13. $f(x,y) = \ln(x^2 + y^2)$

14. $f(x,y) = \dfrac{x - y}{x + y}$

15. $f(x,y,z) = x^2 e^{yz} + \cos(xz)$

**Find all second-order partial derivatives:**

16. $f(x,y) = x^2y + xy^3$

17. $f(x,y) = \sin(xy)$

**Verify Clairaut's theorem** ($f_{xy} = f_{yx}$) for:

18. $f(x,y) = x^2\ln y + y^2\cos x$

---

### Section D — Chain Rule

19. Let $w = x^2 + y^2$, $x = \cos t$, $y = \sin t$. Find $dw/dt$ using the chain rule. Verify by substituting directly.

20. Let $w = xy + yz$, $x = e^t$, $y = e^{-t}$, $z = e^{2t}$. Find $dw/dt$.

21. Let $w = xy^2$, $x = s + t$, $y = s - t$. Find $\partial w/\partial s$ and $\partial w/\partial t$.

22. Let $z = x^2 + 3xy - y^2$, $x = r\cos\theta$, $y = r\sin\theta$. Find $\partial z/\partial r$ and $\partial z/\partial\theta$.

23. If $F(x,y,z) = 0$ defines $z$ implicitly as a function of $x$ and $y$, use the chain rule to derive:
$$\frac{\partial z}{\partial x} = -\frac{F_x}{F_z}$$

Then apply it to $x^3 + z^3 - 6xyz = 0$.

---

### Section E — Directional Derivatives & Gradient

24. Find the directional derivative of $f(x,y) = x^2y^3 - 4y$ at $(2, -1)$ in the direction of $\vec{v} = 2\hat{i} + 5\hat{j}$.

25. Find the gradient of $f(x,y,z) = x^2yz - 2xz^3$ at $(1, -1, 2)$.

26. In what direction does $f(x,y) = x^2 - xy + y^2$ increase most rapidly at $(1, 1)$? What is the maximum rate of increase?

27. Find the directions in which $g(x,y) = \ln(x^2 + y^2)$ has zero directional derivative at $(1, 2)$.

28. At what point on the ellipse $4x^2 + y^2 = 4$ is the tangent line parallel to the line $x + 2y = 1$? *(Use the gradient.)*

---

### Section F — Tangent Planes and Linearization

29. Find the equation of the tangent plane to $z = x^2 + y^2$ at $(1, 2, 5)$.

30. Find the equation of the tangent plane to $z = e^x\cos y$ at $(0, 0, 1)$.

31. Find the linearization $L(x,y)$ of $f(x,y) = \sqrt{x^2 + y^2}$ near $(3, 4)$.

32. Use linearization to approximate $f(1.02, 2.01)$ where $f(x,y) = x^3y^2$.

33. Find the tangent plane to the level surface $xyz = 6$ at $(1, 2, 3)$.

---

### Section G — Extreme Values and Saddle Points

**Find all critical points and classify each:**

34. $f(x,y) = x^2 + xy + y^2 - 6x$

35. $f(x,y) = x^3 - 3x - y^2 + 4y$

36. $f(x,y) = x^4 + y^4 - 4xy$

37. $f(x,y) = e^{-(x^2+y^2)}$ &nbsp; *(Use the second derivative test carefully.)*

**Find the absolute extrema on the given region:**

38. $f(x,y) = 2 + 2x + 2y - x^2 - y^2$ on the closed triangular region with vertices $(0,0)$, $(2,0)$, $(0,2)$.

39. $f(x,y) = x^2 - 2xy + 2y^2 - 2y$ on the closed rectangle $0 \leq x \leq 3$, $-1 \leq y \leq 2$.

---

### Section H — Lagrange Multipliers

40. Find the extreme values of $f(x,y) = xy$ subject to the constraint $x^2 + y^2 = 8$.

41. Find the point on the plane $x + 2y + 3z = 14$ closest to the origin.

42. Find the maximum and minimum values of $f(x,y,z) = x + 2y + 3z$ on the sphere $x^2 + y^2 + z^2 = 1$.

43. Find the dimensions of the rectangular box with largest volume if the total surface area is $64\ \text{cm}^2$.

44. **[Challenge]** Minimize $f(x,y,z) = x^2 + y^2 + z^2$ subject to both $x + 2y + z = 4$ and $x - y + z = 1$.

---

> **Key Warning:** When applying the second derivative test, $D = 0$ is inconclusive — you may need to examine the function behavior directly (e.g., by comparing values along different paths through the critical point).
