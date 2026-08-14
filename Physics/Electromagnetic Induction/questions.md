# Physics Question Bank: Electromagnetic Induction
> ~100 questions | Conceptual · Derivation · Numerical · Application

## A. Motional EMF and Flux Rule
1. Define motional emf.
2. What causes motional emf in a conducting rod moving through a magnetic field?
3. Set up the scenario for a rectangular loop moving out of a uniform magnetic field.
4. Calculate the Lorentz force on the charges in the moving arm of the rectangular loop.
5. Why do charges in the stationary parts of the loop experience no magnetic force?
6. Derive the expression for the motional emf $\mathcal{E} = vBh$ for the rectangular loop.
7. Define magnetic flux $\Phi$ for the rectangular loop.
8. Show that the rate of change of flux is $-vBh$.
9. Combine the emf and flux expressions to state the flux rule for the rectangular loop.
10. State the flux rule mathematically.
11. Consider an arbitrary loop moving in a non-uniform magnetic field. How is the change in flux $d\Phi$ calculated?
12. What does the area vector $d\vec{a}$ sweep out when a loop segment $d\vec{l}$ moves with velocity $\vec{v}$?
13. Prove that $d\Phi/dt = -\oint (\vec{v} \times \vec{B}) \cdot d\vec{l}$ for an arbitrary moving loop.
14. Show that the right-hand side of the above equation equals the induced motional emf.
15. Conclude the general flux rule $\mathcal{E} = -d\Phi/dt$ from the arbitrary loop derivation.
16. A 1m rod moves at 5 m/s perpendicularly through a 2T field. Calculate the motional emf.
17. If the rod is part of a closed circuit with resistance $R$, what is the induced current?
18. What force is required to keep the rod moving at a constant velocity?
19. Show that the mechanical power provided equals the electrical power dissipated in the resistor.
20. Does motional emf arise from an electric field or a magnetic field?

## B. Faraday's Laws and Lenz's Law
21. State Faraday's first law of electromagnetic induction.
22. State Faraday's second law of electromagnetic induction.
23. State Faraday's third law (quantitative law).
24. What is the fundamental difference between motional emf and Faraday induced emf?
25. Express induced emf as a line integral of the electric field $\vec{E}$.
26. Equate the line integral of $\vec{E}$ to the negative rate of change of magnetic flux.
27. Use Stokes' theorem to transform the integral form of Faraday's law into a surface integral.
28. Derive the differential form of Faraday's law: $\nabla \times \vec{E} = -\partial\vec{B}/\partial t$.
29. Compare Faraday's induced electric field to an electrostatic field. What is the key difference regarding the curl?
30. Is a Faraday induced electric field conservative? Explain.
31. State Lenz's law.
32. How does Lenz's law determine the direction of the induced current?
33. Explain how Lenz's law is a consequence of the law of conservation of energy.
34. What would happen if Lenz's law were reversed (i.e., if the induced current aided the flux change)?
35. How can you find the induced electric field from the vector potential $\vec{A}$?
36. Show that $\vec{E} = -\partial\vec{A}/\partial t$ satisfies Faraday's law.
37. Derive the analog to the Biot-Savart law for calculating the induced electric field.
38. When a magnet is dropped through a conducting ring, what happens to its acceleration?
39. Why does a spark occur when a circuit containing an inductor is broken?
40. How does the presence of an induced electric field explain eddy currents?

## C. Self Induction
41. Define self-induction.
42. Why is the induced emf in self-induction sometimes called "back emf"?
43. Define the coefficient of self-induction (self-inductance) $L$ in terms of flux and current.
44. Define self-inductance $L$ in terms of induced emf and the rate of change of current.
45. What is the SI unit of inductance, and how is it related to Volts, Amperes, and seconds?
46. Set up the calculation for the self-inductance of a long solenoid.
47. What is the magnetic field inside a long solenoid?
48. What is the total magnetic flux linked with a portion of the solenoid of length $l$?
49. Derive the self-inductance $L = \mu_0 \pi n^2 R^2 l$ for a solenoid.
50. What is the self-inductance per unit length of a long solenoid?
51. How does the self-inductance of a solenoid depend on the number of turns per unit length?
52. How does the self-inductance of a solenoid depend on its cross-sectional area?
53. Set up the calculation for the self-inductance of a coaxial cable.
54. What Amperian loop is used to find the magnetic field in the region between the cylinders of a coaxial cable?
55. Derive the magnetic field $B = \mu_0 I / 2\pi r$ between the cylinders.
56. Calculate the magnetic flux through a rectangular cross-section between the inner and outer cylinders.
57. Derive the self-inductance $L = (\mu_0 l / 2\pi) \ln(b/a)$ for a coaxial cable.
58. Write the differential equation for an RL circuit connected to a DC battery.
59. Solve the differential equation to find the current $I(t)$ as a function of time.
60. What is the time constant of an RL circuit?

## D. Mutual Induction and Neumann Formula
61. Define mutual induction.
62. Set up a scenario with two coils to illustrate mutual induction.
63. Define the coefficient of mutual induction $M_{21}$ between two coils.
64. Write Faraday's law for the induced emf in coil 2 due to a changing current in coil 1.
65. What does the coefficient of mutual induction depend on?
66. Set up the calculation to find the mutual inductance between two arbitrary loops using the Biot-Savart law.
67. Express the magnetic field $\vec{B}_1$ due to loop 1 in terms of a line integral.
68. Express the vector potential $\vec{A}_1$ due to loop 1.
69. Calculate the flux $\Phi_2$ through loop 2 using the vector potential $\vec{A}_1$.
70. Derive the Neumann formula for mutual inductance: $M_{21} = \frac{\mu_0}{4\pi} \oint \oint \frac{d\vec{l}_1 \cdot d\vec{l}_2}{r}$.
71. State the reciprocity theorem for mutual inductance.
72. How does the Neumann formula prove the reciprocity theorem ($M_{12} = M_{21}$)?
73. Why is the reciprocity theorem practically useful in solving complex mutual inductance problems?
74. A short solenoid is placed inside a long solenoid. Which flux is easier to calculate directly: short-on-long or long-on-short?
75. Calculate the mutual inductance between a long solenoid and a short solenoid wrapped around it.
76. In the solenoid example, show how reciprocity simplifies the calculation.
77. Two circular loops are concentric and coplanar. If the inner radius is much smaller than the outer, find $M$.
78. What is a perfectly coupled transformer in terms of mutual inductance?
79. How is mutual inductance minimized in circuit design?
80. Can mutual inductance be negative? Explain.

## E. Energy Stored in a Magnetic Field
81. Why must work be done to establish a current in an inductor?
82. Write the expression for the rate of work done (power) against the back emf.
83. Set up the integral to find the total work done to reach a steady current $I$.
84. Derive the energy stored in an inductor: $W = \frac{1}{2} L I^2$.
85. Relate the energy $W = \frac{1}{2} L I^2$ to the magnetic flux $\Phi$.
86. Express the energy stored in terms of the vector potential $\vec{A}$ and the current element $I d\vec{l}$.
87. Generalize the energy expression to a volume integral involving $\vec{A}$ and volume current density $\vec{J}$.
88. Use Ampere's law ($\mu_0 \vec{J} = \nabla \times \vec{B}$) to substitute for $\vec{J}$ in the energy integral.
89. Apply the vector identity $\nabla \cdot (\vec{A} \times \vec{B}) = \vec{B} \cdot (\nabla \times \vec{A}) - \vec{A} \cdot (\nabla \times \vec{B})$ to the integrand.
90. Separate the integral into a volume integral of $B^2$ and a surface integral.
91. Why does the surface integral term vanish when integrated over all space?
92. Derive the final expression for the total energy stored in a magnetic field: $W = \frac{1}{2\mu_0} \int B^2 d\tau$.
93. Define magnetic energy density $u_m$.
94. Write the formula for magnetic energy density $u_m = B^2 / 2\mu_0$.
95. Calculate the magnetic energy stored in a length $l$ of a long solenoid using the $B^2$ volume integral.
96. Compare the result from the volume integral to the $\frac{1}{2} L I^2$ formula for the solenoid.
97. Calculate the magnetic energy stored in a coaxial cable using the volume integral.
98. Compare the result from the volume integral to the $\frac{1}{2} L I^2$ formula for the coaxial cable.
99. Is magnetic energy stored in the wires or in the magnetic field itself?
100. Compare the formula for magnetic energy density with that for electric energy density.
