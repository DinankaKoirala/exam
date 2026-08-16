# Physics 102 — 50 High-Yield Electromagnetism Questions

## Part A: Electric Dipole — Potential and Field

1. Define an electric dipole and electric dipole moment **p**. State its magnitude, direction, and SI unit.

2. What is meant by a short dipole? State the condition required for the short-dipole approximation.

3. Derive the electric potential `V(r, θ)` at a general point due to a short electric dipole.

4. Write the dipole potential in:
   - Spherical polar form
   - Cartesian form
   - Coordinate-free vector form

5. How does the potential of a dipole vary with distance compared with the potential of a point charge? Why?

6. Find the dipole potential at:
   - Axial point (`θ = 0°`)
   - Equatorial point (`θ = 90°`)
   - At what angle is `V = 0`?

7. State the relationship between electric field and electric potential:

   `E = −∇V`

   Explain its physical meaning.

8. Derive the electric field of a short dipole in spherical coordinates and show that:

   `E = [p/(4πε₀r³)](2cosθ r̂ + sinθ θ̂)`

9. Derive the magnitude of the electric field of a short dipole:

   `E = [p/(4πε₀r³)]√(3cos²θ + 1)`

10. Show that the dipole field can be expressed in coordinate-free form as:

    `E(r) = [1/(4πε₀r³)][3(p·r̂)r̂ − p]`

11. Derive the electric field at the axial and equatorial points and show that:

    `E_axial = 2E_equatorial`

12. At what angle is the electric field of a dipole:
    - Purely radial?
    - Purely tangential?

13. A dipole has given values of `p`, `r`, and `θ`. Calculate its potential `V` and electric field `E`.


---

## Part B: Dipole in an External Electric Field

14. Why is the net force on a dipole zero in a uniform electric field while its torque can be non-zero?

15. Derive the torque on a dipole in a uniform electric field and show:

    `τ = p × E`

    and

    `τ = pE sinθ`

16. At what orientations is the torque:
    - Maximum?
    - Zero?

    What direction does the torque tend to rotate the dipole?

17. Derive the work done in rotating a dipole from `θ₁` to `θ₂`:

    `W = −pE(cosθ₂ − cosθ₁)`

18. Derive the potential energy of a dipole and show:

    `U = −p·E = −pE cosθ`

19. Determine the orientations corresponding to:
    - Minimum potential energy
    - Maximum potential energy

    Explain stable and unstable equilibrium.

20. Given `p`, `E`, and `θ`, calculate:
    - Torque
    - Potential energy
    - Work required to flip the dipole through `180°`


---

## Part C: Dielectrics and Atomic Polarization

21. What is a dielectric? Distinguish between polar and nonpolar molecules and give examples.

22. Explain how an external electric field induces a dipole moment in a nonpolar atom or molecule.

23. Define atomic polarizability `α` and explain:

    `p = αE`

    State the SI unit of `α`.

24. Using the primitive atomic model, derive:

    `p = 4πε₀a³E`

    and hence obtain:

    `α = 4πε₀a³ = 3ε₀v`

25. Why is atomic polarizability proportional to atomic volume? Why is `p = αE` restricted to sufficiently small electric fields?


---

## Part D: Polarization and Bound Charges

26. Define the polarization vector **P**. State its physical meaning and SI unit.

27. Distinguish between uniform and nonuniform polarization.

28. What are bound charges? Explain their origin using the string-of-dipoles picture.

29. Derive the surface bound-charge density:

    `σ_b = P·n̂`

30. Derive the volume bound-charge density using the divergence theorem:

    `ρ_b = −∇·P`

31. Explain why a uniformly polarized material has no volume bound charge but can have surface bound charge.

32. For a uniformly polarized sphere, determine:
    - Surface bound-charge density `σ_b`
    - Volume bound-charge density `ρ_b`

33. Given a nonuniform polarization such as:

    `P = 3x x̂ C/m²`

    calculate `ρ_b`.


---

## Part E: Electric Displacement and Gauss's Law

34. Distinguish between free charge and bound charge. Write:

    `ρ = ρ_f + ρ_b`

35. Starting from Gauss's law and:

    `ρ_b = −∇·P`

    derive:

    `D = ε₀E + P`

36. State Gauss's law for **D** in:

    **Differential form:**

    `∇·D = ρ_f`

    **Integral form:**

    `∮D·da = Q_f,enc`

37. Why is Gauss's law for **D** particularly useful for dielectric problems?

38. A long charged wire is surrounded by dielectric insulation. Use Gauss's law for **D** to determine **D** and **E** inside and outside the dielectric.

39. A charged metal sphere of radius `a` is surrounded by a dielectric shell extending to radius `b`. Find **D** and **E** in all regions.

40. For the metal sphere with dielectric shell, derive the potential at the center:

    `V = (Q/4π)[1/(ε₀b) + 1/(εa) − 1/(εb)]`


---

## Part F: Linear Dielectrics, Susceptibility, and Permittivity

41. What is a linear dielectric? Define electric susceptibility `χ_e` and write:

    `P = ε₀χ_eE`

42. Define:
    - Permittivity `ε`
    - Relative permittivity `ε_r`
    - Dielectric constant `K`

    Derive:

    `ε = ε₀(1 + χ_e)`

    and

    `K = ε_r = 1 + χ_e`

43. Show that for a linear dielectric:

    `D = εE`

44. Derive the relationship between bound and free volume-charge densities in a linear dielectric:

    `ρ_b = −[χ_e/(1 + χ_e)]ρ_f`

45. Given `ε_r` or `χ_e` and one of **D**, **E**, or **P**, calculate the remaining dielectric quantities.


---

## Part G: Spherical Cavity Field

46. Explain why bound charges appear on the surface of a spherical cavity inside a uniformly polarized dielectric.

47. Derive the electric field at the center of a spherical cavity and show:

    `E_C = P/(3ε₀)`

    Explain why transverse field components cancel by symmetry.


---

## Part H: Clausius–Mossotti Equation

48. Define:
    - Molecular/local field **E_m**
    - Molecular polarizability `α_m`

    Explain:

    `E_m = E + P/(3ε₀)`

    and

    `p_m = α_m E_m`

49. Derive the Clausius–Mossotti equation:

    `α_m = (3ε₀/N)[(K − 1)/(K + 2)]`

    State its physical significance and explain what microscopic and macroscopic quantities it connects.

50. Given `N` and `K`, calculate molecular polarizability `α_m`. Alternatively, given `N` and `α_m`, determine `K`.
