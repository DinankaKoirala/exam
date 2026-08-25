# Unit 2: AC Circuit Analysis — ENGG 112

## Topics Covered
1. AC waveform basics: peak, RMS, average, period, frequency
2. Phasor algebra; R, L, C in AC circuits
3. Impedance, reactance, admittance
4. Series & Parallel RLC circuits
5. Real, Reactive, Apparent power; Power Factor
6. Mesh & Nodal analysis in AC
7. Superposition, Thevenin, Norton in AC
8. Maximum Power Transfer in AC
9. Series & Parallel Resonance (Q-factor, bandwidth)
10. Three-Phase systems (Y and Δ): line/phase voltage, current, power

---

## Key Formulas

### Waveform Values
| Quantity | Formula |
|----------|---------|
| RMS (sinusoidal) | V_rms = V_peak / √2 ≈ 0.707 V_peak |
| Average (full-wave rectified) | V_avg = 2V_peak / π ≈ 0.637 V_peak |
| Average (half-wave) | V_avg = V_peak / π |
| Form factor | k_f = V_rms / V_avg = π/(2√2) ≈ 1.11 (sinusoid) |
| Peak factor | k_p = V_peak / V_rms = √2 ≈ 1.414 (sinusoid) |

### R, L, C Response
| Element | Impedance | Phase |
|---------|-----------|-------|
| Resistor | Z = R | V in phase with I |
| Inductor | Z = jωL = jX_L | V leads I by 90° |
| Capacitor | Z = 1/(jωC) = -jX_C | I leads V by 90° |

### Series RLC
- Z_T = R + j(X_L - X_C)
- |Z_T| = √(R² + (X_L - X_C)²)
- Phase angle: φ = arctan((X_L - X_C) / R)

### Power
| Type | Formula | Unit |
|------|---------|------|
| Real (Average) | P = V_rms · I_rms · cosφ = I²R | W |
| Reactive | Q = V_rms · I_rms · sinφ | VAR |
| Apparent | S = V_rms · I_rms = √(P² + Q²) | VA |
| Power Factor | PF = cosφ = P/S | dimensionless |

### Resonance (Series RLC)
- Resonant frequency: f₀ = 1 / (2π√LC)
- Quality factor: Q_s = ω₀L/R = 1/(ω₀CR) = (1/R)√(L/C)
- Bandwidth: BW = f₀/Q_s = R/(2πL)
- Half-power (cutoff) frequencies: f₁, f₂ where BW = f₂ - f₁
- At resonance: Z = R (purely resistive), PF = 1, I = max

### Three-Phase (Balanced)
| Config | Voltage relation | Current relation |
|--------|-----------------|-----------------|
| Y (Star) | V_L = √3 · V_Ph | I_L = I_Ph |
| Δ (Delta) | V_L = V_Ph | I_L = √3 · I_Ph |

- Total 3-phase power: P = √3 · V_L · I_L · cosφ = 3 · V_Ph · I_Ph · cosφ
- Phases are 120° apart

### AC Maximum Power Transfer
- For complex load Z_L = R_L + jX_L:
  - Z_L = Z_th* (conjugate of Thevenin impedance)
  - i.e., R_L = R_th, X_L = -X_th

---

## MCQ Bank (Past Year Questions)

### AC Waveform Basics

**[Jun 2024, Q7]** Time period of a waveform with frequency 60 Hz:
- ✅ **a) 16.67 ms** (T = 1/f)

**[Jun 2024, Q8]** RMS value if peak is 100V:
- ✅ **b) 70.7 V** (V_rms = 100/√2)

**[May 2022, Q12]** 50 Hz, 30A RMS current — correct equation:
- ✅ **a) 42.42 sin 314t** (I_peak = 30√2 ≈ 42.42; ω = 2π×50 ≈ 314)

**[May 2022, Q15]** Form and peak factor of a specific waveform (half-wave):
- ✅ **a) 1.57 and 2 respectively**

**[Mar 2025, Q3a]** Find average and RMS value of a periodic waveform (given graph). *(Long answer — see below)*

**[May 2022, Q4b]** Find average and RMS of a periodic waveform (sine wave with DC offset). *(Long answer)*

**[Sep 2024, Q3c — MCQ context]** RMS of a square wave alternating between +10V and -10V:
- Hint: V_rms = V_peak for a square wave = 10V *(check original)*

### R, L, C Behaviour

**[Jun 2024, Q3]** Time constant of RC circuit: R=5kΩ, C=10µF:
- a) 500ms  ✅ **b) 0.5s = 500ms** (τ = RC = 5000×10×10⁻⁶)  c) 50µs  d) 50ms

**[Jun 2024, Q9]** Coil: R=4Ω, X_L=3Ω. Total impedance:
- a) 17Ω  b) 6Ω  ✅ **c) 5Ω** (|Z| = √(16+9))  d) 4Ω

**[Jun 2024, Q10]** Phase angle for coil: R=4Ω, X_L=3Ω:
- a) 60.1°  b) 50°  c) 43.5°  ✅ **d) 36.8°** (arctan(3/4))

**[May 2022, Q13]** Reactance of capacitor at 50Hz = 20Ω. At 100Hz:
- ✅ **a) 2.5 Ω** (X_C = 1/ωC; doubles frequency → halves reactance)

### Phasors & Phase Relationships

**[Jan 2025, Q12]** Phase relation between V=9sin(ωt+30°) and I=7sin(ωt+80°):
- a) V leads I by 30°  b) V leads I by 80°  c) V leads I by 110°  ✅ **d) V leads I by 50°** (30°-(-20°)... wait: 30°-80°= -50° → V lags I by 50°, or I leads V by 50°. Re-check: V leads I means φ_V > φ_I → 30° < 80° so **I leads V by 50°** / V lags I by 50°)

> ⚠️ Check options carefully in exam. The relative angle = 80° - 30° = 50°, with I leading.

**[Sep 2024, Q16]** V₁=60sin(θ), V₂=40sin(θ-π/3). Instantaneous resultant:
- ✅ **c) 87.2sin(θ-26.5°) Volts** (phasor addition)

**[Sep 2024, Q17]** V1=(2+5j)V, V2=(3+6j)V in series. Total voltage:
- ✅ **c) 5+11j Volts**

### Power Factor & Power Types

**[Jan 2025, Q13]** For purely resistive AC circuit, power factor =
- ✅ **c) 1**

**[May 2022, Q11]** Load: PF=0.8 lagging, 8kW at 220V. Impedance in rectangular form:
- a) 3.2-j2.4  b) 3.2+j2.4  c) 4+j3  ✅ **d) 4-j3** (lagging → inductive → positive angle → Z = R+jX, but PF lagging means current lags → load is inductive, Z should be R+jX. Wait: S=P/PF=10kVA, I=S/V=45.45A, Z=V/I. Recheck sign convention in exam.)

**[May 2022, Q14]** Apparent power=10kVA, active power=8kW. Reactive power:
- a) 2kVAR  b) 6kVAR  ✅ **c) 8kVAR** (Q = √(S²-P²) = √(100-64)×1000 = 6kVAR)

> ⚠️ Answer is **b) 6 kVAR** — Q = √(10²-8²) = √36 = 6 kVAR

### Resonance

**[Jan 2025, Q14]** Bandwidth=400Hz, resonant frequency=4000Hz. Quality factor:
- a) 5  ✅ **b) 10** (Q = f₀/BW = 4000/400)  c) 15  d) 20

**[Jun 2024, Q11]** Resonant frequency of LC: L=2mH, C=54µF:
- a) 225.1Hz  b) 159.2Hz  ✅ **c) 114.27Hz** (f = 1/(2π√(2e-3 × 54e-6)))  d) 99.45Hz

**[Jun 2024, Q13]** Series RLC: R=10Ω, L=0.1H, C=10µF. Q at resonance:
- a) 10  b) 15.92  c) 25.29  ✅ **d) 31.62** (Q = (1/R)√(L/C))

**[Jun 2024, Q15]** In series resonance with X_L = X_C, circuit is:
- ✅ **a) Purely resistive**

**[Jun 2024, Q16]** Total impedance: R=8Ω, L=0.05H, C=20µF at 1kHz:
- a) 8Ω  b) 10Ω  ✅ **c) 128Ω** (X_L=314Ω, X_C=7.96Ω, Z=√(64+(314-7.96)²))

**[Sep 2024, Q12]** A circuit is selective if it has a ___ peak and ___ bandwidth:
- ✅ **b) Sharp, narrow**

**[Sep 2024, Q13]** At resonance, capacitive energy ___ inductive energy and electrostatic energy ___ magnetic energy:
- ✅ **a) Equal to, equal to**

**[Sep 2024, Q14]** Current in capacitor leads voltage in series RLC circuit ___ the resonant frequency:
- ✅ **a) Above** (above resonance: X_C < X_L, circuit is inductive... wait: above resonance X_L > X_C, net inductive, current lags. Below resonance X_C > X_L, net capacitive, current leads — so **b) Below**)

> ⚠️ Below resonance: capacitive behavior → capacitor current leads. Answer = **b) Below**.

### Three-Phase

**[Jan 2025, Q15]** Voltages in three windings of 3-phase alternator are ___ apart in phase:
- ✅ **a) 120°**

**[May 2022, Q16]** Same — 3-phase generator voltages are ___ degrees apart in time phase:
- ✅ **a) 120°**

**[Jan 2025, Q16]** Balanced 3-phase star connected system. Correct statement:
- a) V_L=V_Ph and I_L=I_Ph  b) V_L=√3·V_Ph  c) V_L=V_Ph and √3·I_Ph=I_L  ✅ **d) V_L=√3·V_Ph and I_L=I_Ph** (wait: for Y: V_L=√3·V_Ph, I_L=I_Ph → **b) and d) overlap** — check exact option wording)

**[Jun 2024, Q12]** Power in three-phase circuit:
- a) P=V_Ph·I_Ph·cosφ  b) both a and b  ✅ **both**: P=3·V_Ph·I_Ph·cosφ = √3·V_L·I_L·cosφ

**[Jun 2024, Q14]** In three-phase delta connection:
- ✅ **b) Line voltage equals phase voltage**

**[Sep 2024, Q18]** Sum of instantaneous power in three phases of a 3-phase system:
- ✅ **b) Remains constant** (key advantage of 3-phase)

**[Sep 2024, Q19]** Purpose of neutral conductor in star-connected 3-phase system:
- ✅ **b) Used for grounding and helps in equalizing phase voltages**

**[Sep 2024, Q20]** Angle between line current and line voltage in balanced star system with φ = phase angle:
- ✅ **d) 30°+φ lagging** (V_line leads V_phase by 30°)

**[May 2022, Q9]** Three-phase power expression:
- ✅ **c) P_T = √3 · V_L · I_L · cosφ**

### Transformer (AC context)

**[Jan 2025, Q11]** If supply frequency increases, secondary output voltage:
- ✅ **c) Remains the same** (V_s/V_p = N_s/N_p; ratio unchanged by frequency — EMF equation has f but so does E_p)

> Actually: E = 4.44·f·N·Φ_max. If f increases but Φ stays same → E increases. But usually, applied V_p is fixed, so Φ_max = V_p/(4.44·f·N_p) decreases → E_s stays ≈ same if turns ratio fixed. Answer depends on assumption — check slides.

**[May 2022, Q17]** Same question — answer: ✅ **b) Decreases** (Φ_max decreases → E_s decreases)

**[Jun 2024, Q19]** What does NOT change in a transformer:
- a) Current  b) Voltage  ✅ **c) Frequency**  d) All

**[Jun 2024, Q20]** Primary: 200 turns, 120V. Secondary: 400 turns. Secondary voltage:
- ✅ **a) 240V** (V_s = V_p × N_s/N_p = 120 × 400/200)

**[Jun 2024, Q17]** Electric current in circuit is analogous to ___ in magnetic circuit:
- ✅ **b) Flux** (I ↔ Φ, EMF ↔ MMF, R ↔ Reluctance)

---

## Long Answer Questions (Section B)

### Waveform Calculations

**[Mar 2025, Q3a]** Find average and RMS value of periodic waveform (given as graph with values +2, +1, -1, -2 over a period).

**[May 2022, Q4b]** Find average and RMS value of a waveform (sine wave from graph).

### Series/Parallel AC Circuits

**[Jun 2024, Q3a]** Plot phase relationship between i=15sin(ωt+60°) and v=10sin(ωt-20°), interpret meaning.

**[Jun 2024, Q3b]** Given i₁=-√2×20sin(ωt-60°) and i=6sin(ωt-30°), find i_s. Sketch time-domain and phasor plots.

**[Jun 2024, Q4b]** Circuit: e=6sin(314t+60°), X_L=2kΩ, X_C=1kΩ. Find current, PF, and average power.

**[Mar 2025, Q4a]** Z₁=(4-j10)Ω parallel with Z₂=(6+j8)Ω, fed from 230V 50Hz. Find:
- Current through each branch
- Total current, total impedance
- PF, active/reactive/apparent power
- Draw phasor diagram

**[Sep 2024, Q5b]** Find active power, reactive power, apparent power, and PF. Network: R=6Ω, X_L=7Ω, X_C=15Ω (details from figure), E=100V∠0°.

**[Sep 2024, Q3b (OR)]** Transformer problem: find primary current, secondary voltage, input impedance. (Iron core transformer)

### Mesh & Nodal in AC

**[Mar 2025, Q3b]** Mesh analysis: find current through R1. Network: V1=220V∠0°, V2=100V∠90°, R=1Ω, 4Ω, 15Ω, 15Ω, 10Ω.

**[Jun 2024, Q4a]** Mesh analysis: find current I₁ through 200mH inductor. Network: R₂=5kΩ (details from figure).

### Superposition, Thevenin, Norton in AC

**[Jan 2025, Q4b]** Using superposition theorem, find current I through 4Ω reactance. Network: E1=10V∠0°, E2=5V∠10°, R=3Ω, X_L=1Ω.

**[Sep 2024, Q5a]** Using Superposition Theorem, determine current through X_L.

**[Sep 2024, Q3c]** Find Thevenin's equivalent: E=50V∠0° (AC source), given network.

### Resonance

**[Jan 2025, Q1a]** Find cutoff frequencies and bandwidth expression for series RLC. Derive relationship between Q-factor, resonant frequency, and bandwidth.

**[Jun 2024, Q6a]** Series RLC resonance: f₀=5kHz, R=2Ω, X_L=X_C=10Ω. Find Q_s and bandwidth.

**[May 2022, Q5a]** Series resonant circuit: f₀=6000Hz, Q=15. Find:
- (i) Bandwidth
- (ii) Cutoff frequencies
- (iii) X_L and X_C (if R=3Ω at resonance)
- (iv) X_C
- (v) Power at half-power frequencies (I_max=0.5A)

**[Sep 2024, Q2c]** What is resonance? State conditions. Derive resonant frequency for series RLC.

**[Sep 2024, Q3b]** Series RLC: ω₀=10 rad/s, BW=0.15 rad/s, draws 16W from 120V at resonance.
- (i) Find R
- (ii) Find BW in Hz
- (iii) Find L and C

### Three-Phase

**[Jan 2025, Q4a]** Show that for Δ-connected 3-phase generator, line current = √3 × phase current, and line voltage = phase voltage. Use diagrams.

**[Jan 2025, Q5c]** Y-connected generator, phase sequence ABC. Given E_a=120V∠0°, E_b=120V∠?, E_c=120V∠?, balanced load (3Ω+j4Ω each):
- (i) Find phase angles θ₂ and θ₃
- (ii) Find magnitudes of line voltages
- (iii) Find line currents
- (iv) Verify I_N = 0 for balanced load

**[Jun 2024, Q6b]** Balanced star-delta connected system: E=150V∠0°, E_b=150V∠?. Find:
- (i) Phase angles θ₁ and θ₂
- (ii) Phase currents
- (iii) Line currents
- (iv) Average power per phase

**[May 2022, Q4a]** 3-phase Y-connected generator, phase sequence ABC: E_AB=150V∠0°. Find:
- (i) Phase angles θ₂ and θ₃
- (ii) Current in each phase of load (R=6Ω, X_L=8Ω each)
- (iii) Line current magnitudes

**[Sep 2024, Q5c]** Y-connected generator, phase sequence ABC, 120V∠0° phase voltage, balanced load (3Ω+j4Ω):
- (i) Phase angles θ₂ and θ₃
- (ii) Line voltage magnitudes
- (iii) Verify I_N = 0

**[Mar 2025, Q5b]** Δ-Y connected load system: V_an=200V∠0°, V_bn=200V∠-120°, V_cn=200V∠+120°. Find total average power, reactive power, apparent power, and PF.

---

## Practice Tips
- **Phasors**: convert all quantities to phasor form (polar or rectangular) before calculation
- **Impedance**: R stays R; X_L = jωL (positive imaginary); X_C = -j/ωC (negative imaginary)
- **Power triangle**: S² = P² + Q²; PF = cos(angle of Z)
- **Three-phase**: always draw the phasor diagram first; label each phase 120° apart
- **Resonance**: the key trick is Z is purely real at resonance (imaginary parts cancel)
- For **balanced loads**: line analysis reduces to single-phase equivalent; use Y-equivalent for Δ load
