# Unit 3: Magnetic Circuits — ENGG 112

## Topics Covered
1. Magnetic field, flux, flux density (B)
2. MMF, magnetizing force (H), permeability
3. Reluctance and permeance
4. Series and parallel magnetic circuits (with air gap)
5. B-H curve and its significance
6. Comparison: magnetic vs electric circuit
7. Faraday's law, self-inductance, mutual inductance
8. Dot convention

---

## Key Formulas & Analogies

### Magnetic ↔ Electric Circuit Analogy

| Magnetic | Electric |
|---------|---------|
| MMF (ℱ = N·I) | EMF (V) |
| Flux (Φ) | Current (I) |
| Reluctance (ℛ = l/μA) | Resistance (R = ρl/A) |
| Flux density B = Φ/A | Current density J = I/A |
| Magnetizing force H = ℱ/l = NI/l | Electric field E = V/l |
| Permeability μ = μ₀·μᵣ | Conductivity σ |

### Core Formulas
- **Flux**: Φ = B × A (Wb)
- **Flux density**: B = μ₀ · μᵣ · H = μH (T)
- **Reluctance**: ℛ = l / (μ · A) (AT/Wb)
- **MMF**: ℱ = N · I = H · l = Φ · ℛ (Ampere-turns)
- **Permeability of free space**: μ₀ = 4π × 10⁻⁷ H/m
- **Relative permeability**: μᵣ (dimensionless; for air ≈ 1, for steel >> 1)

### Series Magnetic Circuit
- ℱ_total = ℱ_core + ℱ_gap = H_core · l_core + H_gap · l_gap
- ℛ_total = ℛ_core + ℛ_gap (series reluctances add)

### Air Gap
- H_gap = B / μ₀ (since μᵣ = 1 for air)
- Air gap has large reluctance → requires more MMF

### Faraday's Law & Inductance
- Induced EMF: e = -N · dΦ/dt
- Self-inductance: L = N·Φ/I = N²/ℛ (Henries)
- Mutual inductance: M = k · √(L₁·L₂), where k = coupling coefficient

---

## MCQ Bank (Past Year Questions)

**[Jun 2024, Q17]** Electric current in electric circuit is analogous to ___ in magnetic circuit:
- a) MMF  ✅ **b) Flux**  c) Flux density  d) Tesla

**[Jun 2024, Q18]** A 100-turn coil has 5A and flux linkage 0.02Wb. Inductance:
- a) 4H  b) 2H  ✅ **c) 0.4H** (L = NΦ/I = 100×0.02/5)  d) 0.2H

**[Sep 2024, Q15]** A coil wound around a steel core with current → steel core acts as:
- ✅ **a) Electromagnet**

**[May 2022, Q18]** Air gap is usually inserted in magnetic circuits to:
- a) Increase MMF  b) Increase flux  ✅ **c) Prevent saturation**  d) Increase conductivity

**[May 2022, Q19]** Series resonant circuit: R=12Ω, C=40pF, L=8mH. Resonant frequency:
- a) 25.1Hz  ✅ **b) 281Hz** (f=1/(2π√(8e-3 × 40e-12)) ≈ 281kHz — check units)  c) 2810Hz  d) 300Hz

> *(This question is technically about resonance but appeared in the magnetic/AC section of the paper.)*

---

## Long Answer Questions (Section B)

**[Jun 2024, Q5a]** Compare magnetic circuit and electric circuit terminologies. Also find number of turns N₁ to establish Φ=1.2×10⁻⁴ Wb in a magnetic circuit. Given: I=2A, Area=0.0012m², mean length l=0.2m (use B-H data or μᵣ given).

**[May 2022, Q3b]** Find current I required to establish Φ=0.75×10⁻⁴ Wb in a series magnetic circuit with air gap. Given: H_cast-steel=280 AT/m, Area=1.5×10⁻⁴ m², l_cdefab=100×10⁻³ m, air gap=2×10⁻³ m.
> Steps: Find B = Φ/A → H_steel from given → MMF_steel = H·l → MMF_gap = B·l_gap/μ₀ → total MMF = N·I → solve for I.

**[Sep 2024, Q4b]** Find the current I₂ in the network (mutual inductance circuit). Given: M₁₂=2Ω, N_e=8Ω. (Involves dot convention for coupled inductors)

---

## Conceptual Questions

1. **Compare magnetic and electric circuits** — draw a table with at least 5 analogous quantities.

2. **Significance of B-H curve**:
   - Shows how flux density B varies with magnetizing force H for a material
   - Slope = permeability μ = B/H
   - Saturation region: beyond a point, increasing H gives little increase in B
   - Used in transformer and motor core design to avoid saturation
   - Hysteresis loop shows energy lost per cycle → core losses

3. **Why air gap?** — Increases effective reluctance, keeps operating point on linear region of B-H curve, prevents magnetic saturation.

4. **Faraday's Law** — Changing flux induces EMF. The induced EMF opposes the change (Lenz's law). This is the basis of transformers and generators.

5. **Dot convention** — Determines polarity of mutually induced voltages in coupled inductors. Currents entering dotted terminals produce aiding fluxes.

---

## Practice Tips
- Draw the magnetic circuit as an equivalent electrical circuit (sources = MMF, resistors = reluctances)
- For series circuits: add reluctances, use MMF = Φ × ℛ_total
- For air gap: use μ₀ (not μ₀μᵣ) since μᵣ_air = 1
- Remember: B-H curve slope = μ; at saturation, curve flattens
- Self-inductance L = N²/ℛ — larger N or smaller ℛ → larger L
