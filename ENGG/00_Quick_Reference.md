# ENGG 112 — Quick Reference & Exam Strategy

## Exam Structure
| Section | Format | Marks |
|---------|--------|-------|
| Section A | 20 MCQs × 0.5 = **10 marks** | 30 mins |
| Section B | Attempt **any 4** (or 5 in some years) × 8–10 = **40 marks** | 2 hrs 30 mins |
| **Total** | | **50 marks** |

---

## High-Frequency Topics (appeared in 3+ papers)

| Topic | Papers |
|-------|--------|
| Thevenin's theorem (long answer) | Jan25, Mar25, May22, Sep24, Jun24 |
| Transformer EMF equation | Jan25, Mar25, Jun24, Sep24 |
| Mesh analysis | Jan25, Mar25, Jun24, Sep24 |
| Nodal analysis | Jan25, Mar25, Jun24, May22, Sep24 |
| Three-phase Y/Δ circuits | Jan25, Mar25, May22, Jun24, Sep24 |
| Series RLC resonance | Jan25, Jun24, May22, Sep24 |
| Superposition theorem | Jan25, May22, Sep24 |
| Max power transfer (proof/derivation) | Jun24, May22, Sep24 |
| DC motor/generator (describe) | Jan25, Mar25 |
| Average & RMS value of waveform | Mar25, May22 |

---

## Unit-wise MCQ Pattern (Section A)

| Unit | Typical MCQ count |
|------|-----------------|
| Unit 1 (DC) | 7–9 |
| Unit 2 (AC) | 7–9 |
| Unit 3 (Magnetic) | 1–2 |
| Unit 4 (Machines) | 2–3 |

---

## Most Repeated MCQ Answers to Remember

| Question type | Answer |
|--------------|--------|
| Mesh analysis is based on | KVL |
| In superposition: zero other voltage sources by | Shorting |
| In superposition: zero other current sources by | Opening |
| Max power transfer condition | R_L = R_th |
| 3-phase voltages are apart by | 120° |
| For Y-connection | V_L = √3·V_Ph, I_L = I_Ph |
| For Δ-connection | V_L = V_Ph, I_L = √3·I_Ph |
| Transformer rated in | kVA |
| What doesn't change in transformer | Frequency |
| PF of purely resistive AC circuit | 1 (unity) |
| At series resonance | Circuit is purely resistive |
| Air gap purpose in magnetic circuit | Prevent saturation |
| Electric current analogous to (in magnetic) | Flux |

---

## Formula Sheet: Must Memorise

```
RESISTOR COLOR CODE: B B ROY of Great Britain has Very Good Wife
Black=0, Brown=1, Red=2, Orange=3, Yellow=4, Green=5, Blue=6, Violet=7, Grey=8, White=9
Tolerance: Gold=5%, Silver=10%

STAR-DELTA:
  Δ→Y: R_y = (product of two adjacent Δ resistors) / (sum of all Δ)
  Y→Δ: R_δ = (sum of all pairwise YY products) / (opposite Y resistor)
  If all equal: R_Δ = 3·R_Y

THEVENIN: V_th = V_oc (open circuit voltage)
           R_th = V_oc / I_sc = resistance seen with sources zeroed

NORTON:   I_N = I_sc (short circuit current)
           R_N = R_th

MAX POWER: R_L = R_th → P_max = V_th² / (4·R_th)
           AC: Z_L = Z_th* (conjugate)

RMS: V_rms = V_peak/√2 (sinusoid)  |  V_rms = V_peak (square wave)
AVG: V_avg = 2V_peak/π (sinusoid)

AC POWER: P = V_rms·I_rms·cosφ (Watts)
           Q = V_rms·I_rms·sinφ (VAR)
           S = V_rms·I_rms (VA)
           PF = cosφ = P/S

RESONANCE: f₀ = 1/(2π√LC)
            Q = (1/R)√(L/C) = f₀/BW
            BW = f₂ - f₁ = R/(2πL) = f₀/Q

3-PHASE POWER: P = 3·V_Ph·I_Ph·cosφ = √3·V_L·I_L·cosφ

TRANSFORMER: V₁/V₂ = N₁/N₂ = I₂/I₁
              E = 4.44·f·N·Φ_max
              kVA rating = V₁·I₁ / 1000

MAGNETIC: Φ = B·A  |  B = μ₀μᵣH  |  ℛ = l/(μA)  |  ℱ = NI = Φ·ℛ
```

---

## Section B Strategy

Given **4 questions to attempt from 5** (or 5 from 6 in Jun 2024):

**Recommended choices:**
1. **Q1**: DC network + one more topic (safe, usually KVL/KCL and mesh/nodal)
2. **Q2 or Q3**: Thevenin/Norton/Superposition (very predictable)
3. **Q3 or Q4**: AC circuits + power or resonance
4. **Q5**: Three-phase system (Y/Δ) — high marks if formula applied correctly

**Skip if unsure:** Transformer derivations (can be tricky) or magnetic circuits (need μᵣ data).

---

## Per-Unit File Index

| File | Contents |
|------|---------|
| `Unit1_DC_Circuit_Analysis.md` | Resistors, KVL/KCL, Mesh, Nodal, Thevenin, Norton, Superposition, Max Power |
| `Unit2_AC_Circuit_Analysis.md` | Phasors, RLC, Power, Resonance, Three-Phase |
| `Unit3_Magnetic_Circuits.md` | Flux, MMF, Reluctance, B-H curve, Inductance |
| `Unit4_Transformers_Machines.md` | EMF equation, turns ratio, DC/AC machines |
| `00_Quick_Reference.md` | This file — formulas, patterns, strategy |
