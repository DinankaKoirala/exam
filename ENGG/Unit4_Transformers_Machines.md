# Unit 4: Transformers & Electrical Machines — ENGG 112

## Topics Covered
1. Single-phase transformer: construction, ideal operation
2. Voltage and current relationships (turns ratio)
3. EMF equation of transformer
4. Practical transformers (types)
5. DC generators and motors: working principles
6. AC generators and motors: working principles

---

## Key Formulas

### Ideal Transformer
- Turns ratio: a = N₁/N₂
- Voltage ratio: V₁/V₂ = N₁/N₂ (= a)
- Current ratio: I₁/I₂ = N₂/N₁ (= 1/a)  ← reciprocal of turns ratio
- Power: V₁I₁ = V₂I₂ (no losses in ideal transformer)
- Impedance seen at primary: Z_in = a² × Z_L

### EMF Equation
- E = 4.44 · f · N · Φ_max
  - f = frequency (Hz)
  - N = number of turns
  - Φ_max = maximum flux (Wb)
- If supply frequency increases and V_p fixed: Φ_max decreases → secondary EMF decreases

### Transformer Ratings
- Rated in **kVA** (apparent power), not kW (doesn't specify PF of load)

---

## MCQ Bank (Past Year Questions)

**[Jan 2025, Q11]** If supply frequency increases, secondary output voltage:
- ✅ **b) Decreases** (Φ_max = V/(4.44·f·N) decreases → E_s decreases)

> Note: Some sources say "remains same" — but if applied V_p is constant and f increases, then Φ_max = V_p/(4.44·f·N₁) decreases, and E_s = 4.44·f·N₂·Φ_max = N₂/N₁ · V_p (turns ratio unchanged). So **E_s remains constant** if V_p is constant! Check your lecture slides for the intended interpretation.

**[May 2022, Q17]** Same question: ✅ **b) Decreases** (per slide answer key)

**[Jun 2024, Q19]** Which does NOT change in a transformer:
- a) Current  b) Voltage  ✅ **c) Frequency**

**[Jun 2024, Q20]** N₁=200, N₂=400, V₁=120V AC. Find V₂:
- ✅ **a) 240V** (V₂ = V₁ × N₂/N₁ = 120 × 2)

**[Jan 2025, Q17]** Transformer ratings are given in:
- ✅ **a) kVA**

**[Jan 2025, Q18]** Induction generators deliver power at ___ power factor:
- ✅ **b) Leading** (they supply reactive power to the grid)

**[May 2022, Q20]** Induction generators deliver power at:
- ✅ **b) Leading** power factor

---

## Long Answer Questions (Section B)

### Transformer EMF Equation

**[Jan 2025, Q3a]** For iron-core transformer (k=1):
- (i) Find induced voltage E₁ (given E=25V, f=60Hz, some turns ratio)
- (ii) Find maximum flux Φ_max
- (iii) If Φ_max=12.5mWb, find frequency of input voltage

**[Mar 2025, Q5a]** Same setup as Jan 2025, Q3a. Given iron-core transformer with k=1:
- (i) Find E₁
- (ii) Find Φ_max
- (iii) If Φ_max=12.5mWb, find f of input voltage
> *This exact question appeared in multiple papers — very likely to come again.*

**[Jun 2024, Q5b]** Derive expression for EMF in transformer (from first principles using Faraday's law).

**[Sep 2024, Q3a]** Derive EMF equation of transformer AND prove that current transformation ratio is reciprocal of turns ratio.

**[Sep 2024, Q2b — OR section]** For iron-core transformer, find:
- (i) Magnitude of current in primary and voltage across secondary
- (ii) Input impedance of the transformer
> (Given: 2kΩ load on secondary, some turns ratio)

### DC Machines

**[Jan 2025, Q5b]** How does a DC motor work? Explain with suitable diagram.
> Key points: Fleming's left-hand rule, Lorentz force on current-carrying conductor, commutator action to maintain rotation, back-EMF.

**[Mar 2025, Q4b]** Explain construction and working principle of a DC generator.
> Key points: Faraday's law (rotating coil in magnetic field), slip rings vs commutator, EMF generation, types (separately excited, shunt, series, compound).

### AC Machines (Conceptual)

From the syllabus — expect definition/description questions:
- AC generator (alternator): rotating field, stationary armature, slip rings
- Induction motor: rotating magnetic field, slip, asynchronous operation
- Synchronous motor: no slip, speed locked to supply frequency

---

## Summary: DC Motor vs DC Generator

| | DC Generator | DC Motor |
|--|--|--|
| **Input** | Mechanical (rotation) | Electrical |
| **Output** | Electrical (DC voltage) | Mechanical (rotation) |
| **Key law** | Faraday's law (e = -dΦ/dt) | Lorentz force (F = BIL) |
| **Component** | Commutator + brushes (rectifies AC → DC) | Same (inverts DC → rotating motion) |
| **Back-EMF** | — | Generated (opposes supply, limits current) |

---

## Practice Tips
- The **EMF equation** E = 4.44·f·N·Φ_max derivation appeared 3 times across papers — know it cold.
- The **transformer current ratio** derivation (from power conservation) appeared twice.
- For motor/generator description questions: a labeled diagram is worth marks — always include one.
- Remember: **kVA rating** because transformer doesn't know the load's PF.
- Coupled circuits: use M = k√(L₁L₂) and dot convention to write mesh equations.
