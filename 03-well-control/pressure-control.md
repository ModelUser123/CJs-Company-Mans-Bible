# Pressure Control

## Overview

Effective pressure control is essential for safe drilling operations. Understanding and managing the pressure relationships in the wellbore prevents kicks, lost circulation, and other well control events.

---

## Pressure Fundamentals

### Hydrostatic Pressure

**Definition:** Pressure exerted by a column of fluid due to gravity

**Formula:**
```
HP = 0.052 × MW × TVD

Where:
HP = Hydrostatic Pressure (psi)
MW = Mud Weight (ppg)
TVD = True Vertical Depth (ft)
```

### Equivalent Mud Weights

**Concept:** Express all pressures in terms of mud weight

```
EMW = Pressure / (0.052 × TVD)
```

**Applications:**
- Compare formation pressure to mud weight
- Express fracture gradient
- Evaluate ECD

---

## Formation Pressures

### Pore Pressure

**Normal Pressure:**
- 0.433-0.465 psi/ft (fresh to salt water)
- 8.34-8.94 ppg EMW

**Abnormal (Over) Pressure:**
- Above normal gradient
- Causes: Compaction, charging, aquathermal

**Subnormal (Under) Pressure:**
- Below normal gradient
- Causes: Depletion, leakoff

### Fracture Pressure

**Definition:** Pressure at which formation breaks down

**Estimation Methods:**
- Eaton's method
- Matthews-Kelly method
- LOT/FIT data

**Typical Values:**
```
Frac Gradient = 0.7-1.0 psi/ft (varies with depth and location)
```

---

## Leak-Off Test (LOT) / Formation Integrity Test (FIT)

### Purpose

- Verify casing shoe strength
- Confirm maximum allowable mud weight
- Data for well control planning

### LOT Procedure

1. Drill out shoe (typically 10-20 ft)
2. Circulate hole clean
3. Close BOP
4. Pump at low rate (0.5-1.0 bbl/min)
5. Record pressure vs. volume
6. Identify leak-off point
7. Bleed pressure, record volume back
8. Document results

### FIT Procedure

Similar to LOT but stop at predetermined pressure (less than LOT)

### Interpretation

**LOT Plot:**
- Linear portion: Pressure building in closed system
- Deviation from linear: Formation taking fluid
- Peak: Leak-off pressure

**Recording:**
```
LOT RECORD

Well: _______________ Date: ___________
Casing Shoe: _______ ft MD / _______ ft TVD
Hole below shoe: _______ ft
Mud Weight: _______ ppg

Test Results:
Pressure: _______ psi
EMW: _______ ppg
Frac Gradient: _______ psi/ft
```

---

## Equivalent Circulating Density (ECD)

### Definition

Effective mud weight at depth accounting for circulating pressure losses

### Formula

```
ECD = MW + (APL / (0.052 × TVD))

Where:
APL = Annular Pressure Loss (psi)
```

### Factors Affecting ECD

| Factor | Effect |
|--------|--------|
| Flow rate | Higher rate = higher ECD |
| Mud rheology | Higher viscosity = higher ECD |
| Annular clearance | Smaller = higher ECD |
| Cuttings load | More cuttings = higher ECD |
| Mud weight | Base for ECD |

### ECD Management

**To Reduce ECD:**
- Reduce flow rate
- Thin mud (reduce PV, YP)
- Optimize hole cleaning
- Manage cuttings

**ECD Limits:**
```
ECD < Fracture Gradient (at all depths)
```

---

## Mud Weight Selection

### Overbalance

**Definition:** Mud weight exceeds formation pressure

**Typical Overbalance:**
- Minimum: 200-500 psi
- Express as: 0.2-0.5 ppg

### Trip Margin

**Definition:** Additional mud weight for tripping operations

**Typical Values:**
- 0.2-0.5 ppg above pore pressure EMW
- Compensates for swab effect

### Maximum Mud Weight

**Constraints:**
- Below fracture gradient
- Below ECD fracture equivalent
- Consider surge effects

### Mud Weight Window

```
Minimum MW = Pore Pressure + Trip Margin
Maximum MW = Fracture Gradient - ECD Effect - Safety Margin
```

---

## Surge and Swab

### Surge Pressure

**Definition:** Pressure increase caused by running pipe into hole

**Factors:**
- Trip speed
- Pipe/hole geometry
- Mud properties
- Open/closed end pipe

**Estimation:**
```
Surge Pressure = f(velocity, rheology, geometry)
```

### Swab Pressure

**Definition:** Pressure decrease caused by pulling pipe from hole

**Factors:**
- Same as surge
- More severe with closed-end pipe

**Risk:**
- Swab = Kick potential
- More critical than surge

### Control Measures

| Factor | Control Method |
|--------|----------------|
| Speed | Reduce trip speed |
| Mud | Adjust rheology (lower PV, YP) |
| Equipment | Use surge reducers |
| Procedure | Fill hole frequently |

---

## Pressure Monitoring

### Surface Indicators

| Indicator | Location | Purpose |
|-----------|----------|---------|
| Standpipe pressure | Rig floor | Circulating pressure |
| Casing pressure | BOP | Annular pressure |
| Choke pressure | Manifold | Kill operations |

### Downhole Monitoring

| Tool | Data |
|------|------|
| MWD | Downhole pressure, ECD |
| PWD | Annular pressure while drilling |
| Memory gauges | Pressure history |

### Real-Time Pressure Calculations

**Key Outputs:**
- ECD at bit
- ECD at casing shoe
- Swab/surge predictions
- Kick tolerance

---

## Kick Tolerance

### Definition

Volume of kick that can be shut in and circulated without exceeding fracture pressure at shoe

### Calculation

```
Kick Tolerance (bbl) = 
(Frac Gradient - MW) × 0.052 × Shoe TVD / Kick Gradient
× Annular Capacity
```

**Simplified:**
```
KT = (MAASP / Gas Gradient) × Annular Capacity
```

### Factors Affecting Kick Tolerance

| Factor | Effect on KT |
|--------|--------------|
| Higher MW | Lower KT |
| Higher frac gradient | Higher KT |
| Deeper shoe | Higher KT |
| Larger annulus | Higher KT |

---

## Managed Pressure Drilling (MPD)

### Concept

Precisely control wellbore pressure using closed-loop system

### Techniques

| Technique | Description |
|-----------|-------------|
| Constant BHP | Maintain constant bottom hole pressure |
| Pressurized Mud Cap | Use heavy fluid cap |
| Dual Gradient | Vary pressure gradient with depth |
| Return Flow Control | Control annular back pressure |

### Equipment

- Rotating control device (RCD)
- Automated choke
- Flow meter
- Back pressure pump
- Control system

### Applications

- Narrow mud weight window
- Depleted reservoirs
- HPHT wells
- Lost circulation zones

---

## Pressure-Related Problems

### Differential Sticking

**Cause:** Pipe pressed against permeable zone by differential pressure

**Prevention:**
- Minimize overbalance
- Keep pipe moving
- Appropriate mud properties

### Lost Circulation

**Cause:** Wellbore pressure exceeds formation strength

**Prevention:**
- Control ECD
- Manage surge
- Appropriate mud weight

### Well Control Events

**Cause:** Formation pressure exceeds wellbore pressure

**Prevention:**
- Adequate mud weight
- Kick detection
- Proper procedures

---

## Related Documents

- [Well Control Procedures](./well-control-procedures.md)
- [Mud Programs](../02-drilling-operations/mud-programs.md)
- [Kill Sheet Calculations](../10-calculation-sheets/kill-sheet-calculations.md)
- [Drilling Calculations](../10-calculation-sheets/drilling-calculations.md)
