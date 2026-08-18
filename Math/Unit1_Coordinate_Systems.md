# Unit 1 — Coordinate Systems
> MATH 104 Advanced Calculus · Kathmandu University

---

## 🎯 YouTube Search Topics

Search these exact phrases to find good videos (3Blue1Brown, Professor Leonard, blackpenredpen, etc.):

| Topic | Search Query |
|---|---|
| Polar coordinates intro | `"polar coordinates" 3blue1brown` or `polar coordinates visual` |
| Converting polar ↔ Cartesian | `polar to rectangular coordinates` |
| Limaçons & cardioids | `graphing polar curves limaçon cardioid` |
| Rose curves & lemniscates | `rose curves polar equations` |
| Area in polar coordinates | `area polar coordinates integral` |
| Cylindrical coordinates | `cylindrical coordinates 3D` |
| Spherical coordinates | `spherical coordinates explained` |

---

## 📖 Core Concepts

### 1.1 Polar Coordinates

A point $P$ is given as $(r, \theta)$ where:
- $r$ = directed distance from origin (pole)
- $\theta$ = angle from the initial ray

**Non-uniqueness:** The same point has infinitely many representations:
$$P(r, \theta) = P(r, \theta + 2n\pi) = P(-r, \theta + \pi)$$

### 1.2 Polar ↔ Cartesian Conversion

$$x = r\cos\theta, \quad y = r\sin\theta$$
$$r^2 = x^2 + y^2, \quad \tan\theta = \frac{y}{x}$$

### 1.3 Curve Classification

| Equation | Curve Type | Condition |
|---|---|---|
| $r = a$ | Circle at origin | — |
| $r = 2a\cos\theta$ or $r = 2a\sin\theta$ | Circle on axis | — |
| $r = a \pm b\cos\theta$ | Limaçon | $a \neq b$ |
| $r = a \pm a\cos\theta$ | Cardioid | $a = b$ |
| $r = a\sin n\theta$ | Rose | $n$ petals if odd, $2n$ if even |
| $r^2 = a^2\sin 2\theta$ | Lemniscate | figure-8 shape |

**Limaçon shape depends on $a/b$ ratio:**
- $a/b < 1$ → inner loop
- $1 < a/b < 2$ → dimpled
- $a/b \geq 2$ → convex (oval)

### 1.4 Area in Polar Coordinates

$$A = \int_\alpha^\beta \frac{1}{2} r^2 \, d\theta$$

---

## 📝 Practice Set

---

### Section A — Plotting & Equivalent Coordinates

**Plot the following points on a polar grid:**

1. $(3, \pi/3)$
2. $(-2, \pi/4)$
3. $(1, -5\pi/6)$
4. $(-3, -\pi/2)$

**Find all equivalent polar coordinate pairs for each point:**

5. $(2, \pi/6)$
6. $(-3, 2\pi/3)$
7. $(4, -\pi/4)$
8. $(-1, 5\pi/6)$

---

### Section B — Coordinate Conversion

**Convert polar → rectangular:**

9. $(2, \pi/3)$
10. $(-3, \pi/6)$
11. $(5, -\pi/4)$
12. $\left(\sqrt{2},\ 3\pi/4\right)$

**Convert rectangular → polar** *(require $r > 0$, $0 \leq \theta < 2\pi$):*

13. $(0, -3)$
14. $(-1, 1)$
15. $(\sqrt{3}, -1)$
16. $(-2, -2\sqrt{3})$

---

### Section C — Equation Conversion

**Rectangular → Polar:**

17. $x^2 + y^2 = 9$
18. $y = 2x$
19. $x^2 - y^2 = 1$
20. $(x-2)^2 + y^2 = 4$

**Polar → Rectangular:**

21. $r = 5\sin\theta$
22. $r = \tan\theta \sec\theta$
23. $r = \dfrac{3}{1 - \cos\theta}$
24. $\theta = \pi/3$
25. $r = -4\cos\theta$

---

### Section D — Curve Identification & Sketching

**Identify each curve type and sketch:**

26. $r = 4$ &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; *(What shape is this?)*
27. $r = 3\cos\theta$
28. $r = -5\sin\theta$
29. $r = 1 + \sin\theta$ &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; *(Identify: cardioid, limaçon, or other?)*
30. $r = 2 + 3\cos\theta$ &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; *(Inner loop or dimpled?)*
31. $r = 3 - 2\sin\theta$
32. $r = 1 + 4\cos\theta$
33. $r = 4 + 4\sin\theta$
34. $r^2 = 9\cos 2\theta$
35. $r^2 = 16\sin 2\theta$
36. $r = 3\cos 2\theta$ &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; *(How many petals?)*
37. $r = 2\sin 3\theta$
38. $r = 4\sin 5\theta$
39. $r = 3\theta,\ \theta > 0$ &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; *(This is a spiral — what kind?)*

---

### Section E — Area in Polar Coordinates

40. Find the area enclosed by $r = 3\cos\theta$.
41. Find the area enclosed by $r = 1 + \cos\theta$.
42. Find the area enclosed by one petal of $r = 4\cos 3\theta$.
43. Find the area inside $r = 2$ and outside $r = 2 - 2\cos\theta$.
44. Find the area of the region shared by $r = 1$ and $r = 2\sin\theta$.

---

### Section F — Cylindrical & Spherical Coordinates

**Convert to cylindrical coordinates $(r, \theta, z)$:**

45. Cartesian point $(1, -1, 2)$
46. Cartesian point $(-\sqrt{3}, 1, 0)$

**Convert to spherical coordinates $(\rho, \phi, \theta)$:**

47. Cartesian point $(0, 0, 5)$
48. Cartesian point $(1, 1, \sqrt{2})$

**Describe the surface:**

49. $\rho = 4$
50. $\phi = \pi/4$
51. $r = z$ (cylindrical)
52. $\rho = 2\cos\phi$ (spherical — convert to Cartesian and identify)

---

### Section G — Challenge Problems

53. Show that the curves $r = \cos\theta$ and $r = 1 - \cos\theta$ intersect. Find all intersection points. *(Hint: deceptive coordinates — check $r = 0$ separately.)*

54. Find the area of the region inside $r = 3\sin\theta$ and outside $r = 1 + \sin\theta$.

55. A curve is given by $r = e^\theta$ for $0 \leq \theta \leq 2\pi$. Sketch the curve and find the total arc length using:
$$L = \int_\alpha^\beta \sqrt{r^2 + \left(\frac{dr}{d\theta}\right)^2}\, d\theta$$

---

> **Tip:** For problems involving intersection of polar curves, always check the pole $(r=0)$ separately — one curve may pass through it at a different angle than the other.
