# Unit 1: DC Circuit Analysis — ENGG 112

## Topics Covered
1. Resistors: color codes, series/parallel, power, temperature coefficient
2. Ohm's Law, KVL, KCR, VDR, CDR
3. Star–Delta (Δ–Y) conversion
4. Sources: ideal/non-ideal, dependent/independent, source conversion
5. Series-Parallel Networks, Ladder Networks
6. Methods of Analysis: Mesh (KVL) and Nodal (KCL)
7. Network Theorems: Superposition, Thevenin's, Norton's, Maximum Power Transfer

---

## Key Formulas

| Formula | Description |
|---------|-------------|
| V = IR | Ohm's Law |
| P = VI = I²R = V²/R | Power |
| R_series = R1 + R2 + ... | Series resistance |
| 1/R_parallel = 1/R1 + 1/R2 + ... | Parallel resistance |
| VDR: Vx = V × Rx/R_total | Voltage Divider Rule |
| CDR: Ix = I × R_other/R_total | Current Divider Rule (2 resistors) |
| **Star-Delta:** Rδ = Ry1·Ry2 + Ry2·Ry3 + Ry3·Ry1 divided by the opposite Ry | Δ from Y |
| **Delta-Star:** Ry = (product of adjacent Rδ) / (sum of all Rδ) | Y from Δ |
| **Source conversion:** V_s = I_s × R_s (series R becomes parallel R) | |

### Network Theorems
- **Superposition**: Zero all sources except one. Sum contributions.
  - Voltage source → short circuit (0V)
  - Current source → open circuit (0A)
- **Thevenin**: V_th = open-circuit voltage; R_th = resistance seen from terminals (all sources zeroed)
- **Norton**: I_N = short-circuit current; R_N = R_th
- **Max Power Transfer**: R_L = R_th → P_max = V_th² / (4·R_th)

---

## MCQ Bank (Past Year Questions)

### Resistors & Ohm's Law

**[Jan 2025, Q1]** What is the resistance of a 100 ft copper wire with diameter 0.020 in at 20°C?
- a) 4.54 Ω  b) 1.57 Ω  c) 8.53 Ω  ✅ **d) 2.59 Ω**

**[Jan 2025, Q2]** How long can a 205 W television run before using more than 4 kWh of energy?
- a) 19.5 h  ✅ **b) 15.7 h** (E = P×t → t = 4000/205)  c) 23.9 h  d) 11.3 h

**[Jun 2024, Q1]** Power dissipated by an 8 Ω resistor with 3 A flowing through it:
- a) 24 W  b) 48 W  ✅ **c) 72 W** (P = I²R = 9×8)  d) 92 W

**[Sep 2024, Q2]** Two copper conductors of equal length; cross-section ratio 1:4. Smaller has 40 Ω. Resistance of larger:
- a) 160 Ω  b) 80 Ω  c) 20 Ω  ✅ **d) 10 Ω** (R ∝ 1/A)

**[Sep 2024, Q1]** Temperature coefficient of resistance is expressed in:
- a) Ohms/°C  b) Mhos/Ohms°C  ✅ **c) Ohms/Ohms°C**  d) Mhos/°C

**[May 2022, Q2]** Resistor color code: Brown, Black, Black, Gold. Value?
- ✅ **a) 10 Ω, 5% tolerance**  b) 100 Ω 10%  c) 1 Ω 5%  d) 1000 Ω 5%

**[May 2022, Q3]** A good electric conductor:
- a) Has low conductance  b) Is always copper  ✅ **c) Produces minimum voltage drop**  d) Has few electrons

**[Sep 2024, Q3]** Three identical resistors connected in parallel, then that combination in series with another identical set in parallel. Result compared to individual:
- a) 9 times  b) 1/9 times  ✅ **c) 1/3 times**  d) 3 times

> *Tip: R_parallel = R/3; two in series = 2R/3. Ratio = (2R/3)/R = 2/3 — check the exact question wording from paper.*

**[Sep 2024, Q6]** In a series circuit with unequal resistances:
- ✅ **d) The highest resistance has the highest voltage drop** (V = IR, same I throughout)

**[Sep 2024, Q7]** Total resistance of an insulator with increasing temperature:
- ✅ **a) Increases** (insulators have positive temperature coefficient unlike semiconductors)

**[Jan 2025, Q3]** Which element cannot be analyzed using Ohm's law?
- ✅ **a) Capacitors** and **b) Transistors** (non-linear/frequency-dependent) — also Inductors (c) in AC. In DC steady state: capacitor = open, inductor = short.

### KVL / KCL

**[Jan 2025, Q7]** Mesh analysis is based on:
- ✅ **a) Kirchhoff's Voltage Law**

**[Jun 2024, Q2]** A junction where two or more elements intersect is called:
- ✅ **a) Node**

### Star-Delta

**[Jun 2024, Q5]** Star network: Ra=10Ω, Rb=20Ω, Rc=40Ω. Find delta equivalents Rab, Rbc, Rca:
- a) 35, 140, 70  b) 70, 60, 35  c) 35, 60, 70  ✅ **d) 70, 150(?), 35** — verify with formula: Rδ = (R1R2+R2R3+R3R1)/R_opposite

### Superposition Theorem

**[Jan 2025, Q5]** In superposition, when one voltage source is considered, all other voltage sources are:
- ✅ **a) Shorted**

**[Sep 2024, Q8]** In superposition, when one voltage source is considered, all other current sources are:
- ✅ **b) Opened**

### Thevenin's & Norton's Theorems

**[Jan 2025, Q8]** Thevenin voltage (V_th) for a bridge network with 12A source and 7Ω, 4Ω, 5Ω, 6Ω resistors:
- a) 20V  b) 32V  c) 48V  ✅ **d) 56V**

**[May 2022, Q8]** Same bridge network as above — V_th:
- a) 20V  b) 32V  c) 48V  ✅ **d) 56V**

**[Jan 2025, Q10]** Norton resistance R_N for a shaded region with 9V source:
- ✅ **a) 5 Ω**

**[Sep 2024, Q9]** Thevenin voltage is the ___ and Thevenin resistance is calculated by ___:
- ✅ **c) Open circuit voltage; shorting all voltage sources and opening all current sources**

**[Sep 2024, Q11]** A current source in parallel with a resistor can be converted to:
- ✅ **a) A voltage source in series with a resistor**

### Maximum Power Transfer

**[Jan 2025, Q9]** Max power is delivered when load resistance is ___ Thevenin resistance:
- ✅ **c) Equal to**

**[Jun 2024, Q6]** Max power delivered when source resistance is ___ load resistance:
- ✅ **c) Equal to**

**[May 2022, Q5]** Load resistance for max power from a circuit (18V source, 12Ω, 3Ω, 3Ω):
- a) 2 Ω  b) 9 Ω  ✅ **c) 6 Ω** (find R_th)  d) 18 Ω

**[Sep 2024, Q10]** Max power delivered when source resistance is ___ load resistance:
- ✅ **b) Equal to**

---

## Long Answer Questions (Section B)

### Mesh & Nodal Analysis

**[Mar 2025, Q1b]** Determine the current through R5 (source resistor) of a network using Nodal Analysis. (Network has 10Ω, 20Ω resistors and a 2A source)

**[Mar 2025, Q3b]** Using Mesh analysis determine current through R1 for a network with:
- V1 = 220V∠0°, V2 = 100V∠90°, R=1Ω, 4Ω, 15Ω, 15Ω, 10Ω

**[Jan 2025, Q2b]** Using mesh analysis, determine current through 5Ω resistor. Network: 50V, 6V, 15V sources with 4Ω, 3Ω, 5Ω, 1Ω, 10Ω, 10Ω resistors. Also find voltage Va.

**[Jun 2024, Q2b]** Use Nodal analysis to calculate current through R1 in given network with 12Ω, 6Ω, 2Ω resistors.

**[May 2022, Q1a]** Convert voltage sources to current sources and find: (i) voltage Vab, (ii) magnitude and direction of current I. Network: E1=9V, E2=8V with R1=3Ω, R2=1Ω, R3=2Ω, R4=6Ω.

**[Sep 2024, Q2a]** Find voltage across 3Ω resistor using Nodal analysis. Network: 8V, 1V sources, 2Ω, 10Ω, 4Ω, 3Ω.

**[Sep 2024, Q2b]** Find currents through each element using mesh analysis (network with 8A current source).

**[Jan 2025, Q5a]** Determine nodal voltages V1 and V2 using super-node concept. Network: 2A, 5A current sources, 20Ω resistor, floating voltage source between V1 and V2.

**[May 2022, Q5b]** Determine nodal voltages V1 and V2. Network: 12V source, 6A, 4A current sources, 10Ω, 4Ω, 2Ω resistors.

### Network Theorems — Long Answer

**[Jan 2025, Q2a]** Find Thevenin equivalent for bridge network shaded area.

**[Mar 2025, Q2b]** Determine Thevenin equivalent for network external to R_L. Network: +22V, -12V, +6V sources, 2.2kΩ, 1.2kΩ, 3.3kΩ, 5.6kΩ, 6.8kΩ resistors.

**[May 2022, Q2a]** Same circuit as above — Thevenin equivalent external to R_L.

**[Sep 2024, Q3c]** Find Thevenin equivalent for network external to elements between points a and b. Source: E=50V∠0°.

**[Sep 2024, Q4a]** Find value of R for maximum power transfer, and determine the maximum power. Network: 5A source, R1=4Ω.

**[Sep 2024, Q4c]** Find Norton equivalent for network external to resistor R. Network: 20V source, 2Ω, 12Ω, R1=25Ω, R2=16Ω, 2Ω.

**[May 2022, Q2b]** Using Superposition, find current through R1 for the networks. Has R5=1Ω, R1=1Ω, R2=6Ω, R3=30Ω, R4=12Ω, E1=11V, E2=8V, 6A source.

**[Jan 2025, Q1b]** Find current I4 and voltage V2 for a network using KVL/KCL. Network: 12V, E with I1=3A, R=4Ω, 3Ω, 6Ω, 8Ω.

**[Mar 2025, Q1a]** Find equivalent resistance for a network where all resistors are 10Ω. (Complex series-parallel arrangement)

**[Sep 2024, Q1a]** Calculate total resistance RT of a resistor cube where each edge is 10Ω.

**[May 2022, Q1b]** Calculate currents I5, I6 and voltage V2 for a large network with: 4kΩ, 8kΩ, 12kΩ, 24kΩ, 12kΩ, 12kΩ, 3kΩ, 9kΩ, 6kΩ resistors and 72V source.

---

## Conceptual / Describe Questions

**[Jan 2025, Q5b]** How does a DC motor work? Explain with a suitable diagram.

**[Sep 2024, Q1c]** Describe any three differences between star (Y) and delta (Δ) connected three-phase AC supply systems. Explain the type of supply used in Nepal for residential consumers.

---

## Practice Tips
- For **Mesh analysis**: assign loop currents, apply KVL to each loop, solve simultaneous equations.
- For **Nodal analysis**: assign node voltages, apply KCL at each node (currents leaving = 0).
- **Super-node**: when a voltage source sits between two non-reference nodes — write KCL + voltage constraint.
- **Super-mesh**: when a current source is shared between two meshes — write KVL around combined mesh + current constraint.
- Always verify **Thevenin** by: V_th = V_oc, R_th = V_oc / I_sc.
