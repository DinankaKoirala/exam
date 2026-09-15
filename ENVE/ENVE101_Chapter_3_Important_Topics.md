# ENVE 101 — Chapter 3: Mass Transfer
**Kathmandu University | Exam Study Priority**

> **Priority basis:** This is a study-priority guide made from the official ENVE 101 (2026) syllabus plus the amount of emphasis, formulas, worked examples, tables, and diagrams in the uploaded Kathmandu University lecture PDF. It is **not an official prediction of exam questions**.

**Priority key:**  
- **A — Highest:** explicit syllabus item + strongly developed in the lecture / numerical or major diagram  
- **B — Important:** explicit syllabus item or substantial lecture topic  
- **C — Review:** supporting material, examples, or background


## A — Highest Priority

### 1. Conservation of Mass and Importance of Mass Balance
- Mass is not created or destroyed; it is transferred/transformed.
- Environmental use: track pollutant **source, movement and fate**.
- **PDF:** pp. 2–3.

### 2. Mass-Transfer Processes by Phase
Know examples of:
- gas → liquid;
- liquid → gas;
- liquid → liquid;
- liquid → solid;
- solid → gas.
- **PDF:** p. 4.

### 3. General Mass-Balance Equation
Core relation:
- **Accumulation rate = Input rate − Output rate ± Transformation rate**

Be able to:
- define a system boundary;
- draw a black-box diagram;
- keep units consistent;
- identify influent/effluent, generation and decay.
- **PDF:** pp. 5–8, 16.

### 4. Single-Material Flow: Splitting and Combining
At steady state with no transformation:
- one inlet/one outlet: `X_0 = X_1`
- splitting: inlet = sum of outlets
- combining: sum of inlets = outlet
- **PDF:** pp. 7–12.

### 5. Conservative vs Non-Conservative Substance
**Conservative**
- no normal transformation;
- examples in lecture: salt, metals;
- transformation rate = `0`.

**Non-conservative**
- physical/chemical/biological transformation occurs;
- examples: BOD, ammonia, some organics;
- transformation rate ≠ `0`.
- **PDF:** p. 13.

### 6. Steady-State Condition
- `dM/dt = 0`
- conservative steady state: **Input rate = Output rate**
- non-conservative steady state:
  - `Input − Output ± Transformation = 0`
  - for decay: `Input = Output + Decay`
- **PDF:** pp. 18–21.

### 7. First-Order Decay
Must know:
- `dC/dt = -kC`
- `ln(C/C_0) = -kt`
- `C = C_0 e^(-kt)`
- for uniform concentration in volume `V`: **decay rate = `VkC`**
- **PDF:** pp. 22–23.

### 8. CSTR / Complete-Mix Box Model
For a completely mixed steady system:
- `Input rate = Output rate + kCV`
- concentration in the reactor/room equals concentration in the outlet under complete mixing.
- Application to both water and air pollution.
- **PDF:** pp. 24–25.

## Numerical Problems to Practice
1. **Refuse splitting to incinerators and landfill** — p. 11.
2. **Wastewater mixing in a river**:
   - `Q_1C_1 + Q_2C_2 = Q_3C_3`
   - complete mixing, steady state, conservative pollutant.
   - **PDF:** pp. 26–28.
3. **Kitchen CO / non-conservative CSTR**:
   - `G = QC + kCV`
   - `C = G/(Q + kV)`
   - **PDF:** pp. 29–31.
4. **Air-quality box model for SO₂** — pp. 32–35.
5. **Ventilation / H₂S decay problem using `C = C_0e^(-kt)`** — p. 36.

## Diagram/Method You Should Use in Every Numerical
1. Draw the system boundary.
2. Label every flow and concentration.
3. State assumptions:
   - steady or unsteady;
   - conservative or non-conservative;
   - complete mixing or not.
4. Write the general balance first.
5. Simplify only after assumptions.
6. Check units.

## B — Important
- Volume balance vs mass balance — p. 9.
- Complex process with a single material — pp. 14–15.
- Multiple-material balances — p. 17.
- Meaning of reaction/transformation rate — p. 19.

## Syllabus Coverage Alert
The official syllabus names this chapter **“Mass and Energy Transfer”**, but the uploaded Chapter 3 PDF develops **mass transfer/mass balance** and contains no substantive section titled energy transfer. Review any additional instructor notes for **energy transfer** if they exist.

## Exam Checklist
- [ ] I can write the general mass-balance equation from memory.
- [ ] I can distinguish conservative and non-conservative pollutants.
- [ ] I can state the steady-state simplification.
- [ ] I can derive/use first-order decay.
- [ ] I can solve river-mixing and CSTR problems.
- [ ] I can draw a correct black-box/box-model diagram before calculating.
