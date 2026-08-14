# Physics Question Bank: Electromagnetic Wave Propagation
> ~100 questions | Conceptual · Derivation · Numerical · Application

## A. Displacement Current and Maxwell's Equations
1. Write down the four basic laws of electricity and magnetism in differential form before Maxwell's correction.
2. Take the divergence of Faraday's law ($\nabla \times \vec{E} = -\partial\vec{B}/\partial t$). What is the result?
3. Take the divergence of Ampere's law ($\nabla \times \vec{B} = \mu_0 \vec{J}$). What is the result?
4. Explain why $\nabla \cdot (\nabla \times \vec{B}) = \mu_0 \nabla \cdot \vec{J}$ poses a problem for time-varying fields.
5. Use the continuity equation to show why the original Ampere's law fails.
6. What is the missing term that Maxwell added to Ampere's law?
7. Derive the expression for the displacement current density $\vec{J}_d = \varepsilon_0 \partial\vec{E}/\partial t$.
8. Write Ampere's law with Maxwell's correction.
9. Verify that the modified Ampere's law is consistent with the continuity equation.
10. What is displacement current? Does it represent an actual flow of charge?
11. Write the complete set of four Maxwell's equations in a vacuum (no dielectrics or magnetic materials).
12. Consider a parallel plate capacitor charging with a constant current $I$.
13. What is the electric field between the plates as a function of time $t$?
14. Calculate the displacement current density between the capacitor plates.
15. Show that the total displacement current between the plates equals the conduction current $I$ in the wires.
16. Use the modified Ampere's law to find the magnetic field at a distance $s$ from the axis between the capacitor plates.
17. What is the Amperian loop chosen for finding the magnetic field between the plates?
18. Compare the magnetic field between the plates to the magnetic field outside the wires.
19. How did Maxwell's correction unify electricity and magnetism?
20. Why was the displacement current difficult to observe experimentally before Hertz?

## B. Maxwell's Equations in Material Medium
21. What happens to the electric polarization $\vec{P}$ when it varies with time?
22. Define polarization current density $\vec{J}_p$.
23. Derive $\vec{J}_p = \partial\vec{P}/\partial t$ using the continuity equation for bound charges.
24. Write the expression for total charge density $\rho$ in a material medium.
25. Write the expression for total current density $\vec{J}$ in a material medium, including free, bound, and polarization currents.
26. Substitute the total charge density into Gauss's law for electricity.
27. Define the electric displacement vector $\vec{D}$ and write the modified Gauss's law ($\nabla \cdot \vec{D} = \rho_f$).
28. Substitute the total current density into Ampere's law with Maxwell's correction.
29. Define the magnetic field strength $\vec{H}$ in terms of $\vec{B}$ and $\vec{M}$.
30. Derive the macroscopic version of Ampere-Maxwell law: $\nabla \times \vec{H} = \vec{J}_f + \partial\vec{D}/\partial t$.
31. Write down the four Maxwell's equations in a material medium in terms of free charges and currents ($\rho_f, \vec{J}_f$).
32. Write down the constitutive relations connecting $\vec{D}$ to $\vec{E}$ and $\vec{H}$ to $\vec{B}$ in linear media.
33. Under what conditions do the macroscopic Maxwell's equations reduce to the vacuum equations?
34. What is the significance of distinguishing between free and bound charges/currents in macroscopic media?
35. How do boundary conditions for $\vec{E}, \vec{B}, \vec{D},$ and $\vec{H}$ derive from Maxwell's equations?
36. Prove that the normal component of $\vec{D}$ is discontinuous by the free surface charge density.
37. Prove that the tangential component of $\vec{E}$ is continuous across a boundary.
38. Prove that the normal component of $\vec{B}$ is continuous across a boundary.
39. Prove that the tangential component of $\vec{H}$ is discontinuous by the free surface current density.
40. Why does polarization current not result in a net accumulation of charge?

## C. Energy in EM Field (Poynting Theorem)
41. Write the expression for the energy stored per unit volume in an electric field.
42. Write the expression for the energy stored per unit volume in a magnetic field.
43. What is the total energy density $u_{em}$ in an electromagnetic field?
44. State the Lorentz force law for a system of point charges.
45. Calculate the work done by the electromagnetic field on a point charge in time $dt$.
46. Why does the magnetic force do no work in this calculation?
47. Extend the work done calculation to a continuous charge distribution with volume charge density $\rho$.
48. Express the rate of work done as an integral involving $\vec{E} \cdot \vec{J}$.
49. Use the Ampere-Maxwell law to substitute for $\vec{J}$ in the $\vec{E} \cdot \vec{J}$ integral.
50. Apply the vector identity $\nabla \cdot (\vec{E} \times \vec{B}) = \vec{B} \cdot (\nabla \times \vec{E}) - \vec{E} \cdot (\nabla \times \vec{B})$.
51. Use Faraday's law to simplify the resulting expression.
52. Group terms to isolate the time derivative of the total electromagnetic energy density $u_{em}$.
53. Define the Poynting vector $\vec{S}$. What are its formula and SI units?
54. What is the physical meaning of the Poynting vector?
55. Derive the integral form of Poynting's theorem: $\frac{dW}{dt} = -\frac{dU_{em}}{dt} - \oint \vec{S} \cdot d\vec{a}$.
56. State Poynting's theorem in words (the work-energy theorem of electrodynamics).
57. Derive the differential form of Poynting's theorem: $\frac{\partial}{\partial t}(u_{mech} + u_{em}) = -\nabla \cdot \vec{S}$.
58. Show how the differential Poynting theorem resembles the continuity equation for charge.
59. What does the term $\nabla \cdot \vec{S}$ represent physically?
60. Calculate the Poynting vector for a straight wire carrying a steady current $I$ and having resistance $R$. Does energy flow into or out of the wire?

## D. Electromagnetic Wave Equations in Vacuum
61. Write Maxwell's equations for free space where $\rho = 0$ and $\vec{J} = 0$.
62. Take the curl of Faraday's law in free space.
63. Apply the vector identity $\nabla \times (\nabla \times \vec{E}) = \nabla(\nabla \cdot \vec{E}) - \nabla^2\vec{E}$.
64. Use Gauss's law for free space to simplify the vector identity result.
65. Substitute the Ampere-Maxwell law into the right side of the curled Faraday's law.
66. Derive the electromagnetic wave equation for the electric field $\vec{E}$: $\nabla^2\vec{E} = \mu_0 \varepsilon_0 \frac{\partial^2 \vec{E}}{\partial t^2}$.
67. Write the three component equations (for $E_x, E_y, E_z$) corresponding to the vector wave equation.
68. Take the curl of the Ampere-Maxwell law in free space.
69. Apply the vector identity and Gauss's law for magnetism to simplify.
70. Substitute Faraday's law into the right side to derive the wave equation for the magnetic field $\vec{B}$.
71. Show that the wave equation for $\vec{B}$ is identical in form to the wave equation for $\vec{E}$.
72. Compare the derived EM wave equations to the standard 3D wave equation $\nabla^2 f = \frac{1}{v^2} \frac{\partial^2 f}{\partial t^2}$.
73. What is the theoretical speed $v$ of the electromagnetic waves in a vacuum?
74. Calculate the numerical value of $c = 1/\sqrt{\mu_0 \varepsilon_0}$ and state its significance.
75. Explain how this derivation led Maxwell to conclude that light is an electromagnetic wave.
76. Write the general mathematical form of a monochromatic plane wave solution for $\vec{E}(z,t)$ propagating in the z-direction.
77. If $\vec{E}$ propagates in the z-direction and is polarized in the x-direction, what direction must $\vec{B}$ point?
78. Use Faraday's law on the plane wave solution to find the relationship between the amplitudes $E_0$ and $B_0$.
79. Prove that the electric and magnetic fields in an EM plane wave are always mutually perpendicular.
80. Prove that the electric and magnetic fields in an EM plane wave are both perpendicular to the direction of propagation (transverse waves).
81. Show that the fields in a plane EM wave are in phase.
82. Calculate the time-averaged energy density of an EM plane wave.
83. Show that the electric and magnetic contributions to the total energy density of an EM wave are equal.
84. What is the time-averaged Poynting vector (intensity) of a plane EM wave?
85. Relate the intensity of an EM wave to the energy density and the speed of light.
86. What is radiation pressure, and how is it related to the Poynting vector?
87. If an EM wave travels through a linear, non-conducting medium ($\varepsilon, \mu$), what is the wave speed $v$?
88. Define the index of refraction $n$ of a material in terms of $\varepsilon, \mu$ and $\varepsilon_0, \mu_0$.
89. How do Maxwell's equations change if magnetic monopoles exist?
90. If $\nabla \cdot \vec{B} = \mu_0 \rho_m$, derive the modified Faraday's law.
91. Discuss the symmetry of Maxwell's equations with and without magnetic monopoles.
92. How does the wave equation change in a conducting medium (where $\vec{J} = \sigma \vec{E}$)?
93. What is the "skin depth" of a conducting material for an EM wave?
94. Why do EM waves not penetrate deeply into good conductors?
95. What generates electromagnetic waves in practice (e.g., in antennas)?
96. Can a static charge generate EM waves? Can a steady current?
97. Explain the concept of retarded potentials.
98. What is the spectrum of electromagnetic waves?
99. Name three applications of electromagnetic wave propagation.
100. Summarize the fundamental insight of Maxwell's synthesis of electromagnetism.
