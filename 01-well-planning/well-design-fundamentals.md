# Well Design Fundamentals

## Overview

Well design integrates geological, engineering, and operational considerations to create a safe, efficient, and cost-effective drilling program.

---

## Well Design Objectives

1. **Safety**: Maintain well control at all times
2. **Geological Success**: Reach target and evaluate formations
3. **Mechanical Integrity**: Provide long-term wellbore integrity
4. **Cost Efficiency**: Optimize cost per barrel produced
5. **Environmental Protection**: Protect aquifers and surface

---

## Well Architecture

### Casing Program Components

| Casing String | Purpose | Typical Setting |
|---------------|---------|-----------------|
| Conductor | Structural support, initial isolation | 40-100 ft |
| Surface | Protect fresh water, BOP support | 500-3,000 ft |
| Intermediate | Isolate problem zones | Variable |
| Production | Hydrocarbon containment | Target zone |
| Liner | Cost savings, targeted isolation | Below intermediate |

### Casing Selection Factors

**Depth Considerations:**
- Formation pressures (pore pressure, fracture gradient)
- Formation stability
- Regulatory requirements
- Directional requirements

**Casing Properties:**
- Weight (ppf)
- Grade (J-55, N-80, P-110, etc.)
- Connection type
- Drift diameter
- Collapse/burst/tension ratings

---

## Pressure Management

### Pressure Hierarchy

```
Fracture Gradient > Mud Weight > Pore Pressure
```

**Design Window:**
- Minimum mud weight: Pore pressure + trip margin
- Maximum mud weight: Fracture gradient - safety margin

### Pore Pressure Sources

1. Normal hydrostatic (0.433-0.465 psi/ft)
2. Abnormal (overpressured) - compaction, charging
3. Subnormal (underpressured) - depletion, leakoff

### Key Pressure Calculations

**Hydrostatic Pressure:**
```
P = 0.052 × MW × TVD

Where:
P = Pressure (psi)
MW = Mud weight (ppg)
TVD = True Vertical Depth (ft)
```

**Equivalent Circulating Density:**
```
ECD = MW + (APL / (0.052 × TVD))

Where:
APL = Annular Pressure Loss (psi)
```

---

## Casing Setting Depths

### Determination Method

1. Plot pore pressure vs. depth
2. Plot fracture gradient vs. depth
3. Apply design factors (kick tolerance, trip margin)
4. Identify casing points where window closes
5. Verify regulatory requirements
6. Optimize for operational efficiency

### Casing Point Selection Criteria

**Must Set Casing When:**
- Mud weight required exceeds fracture gradient of upper formations
- Regulatory requirement (fresh water protection)
- Well control capability required (BOP)
- Hole stability issues
- Changing hole size required

### Kick Tolerance Calculation

```
Kick Tolerance = (Frac Gradient - MW) × (TVD / BHA Depth)
```

**Minimum Kick Tolerance:**
- Surface casing: 50-100 bbls
- Intermediate casing: 25-50 bbls
- Production casing: Design specific

---

## Hole Sizes and Casing Sizes

### Standard Hole/Casing Combinations

| Hole Size | Casing OD | Min Drift | Application |
|-----------|-----------|-----------|-------------|
| 26" | 20" | 19.00" | Conductor |
| 17-1/2" | 13-3/8" | 12.415" | Surface |
| 12-1/4" | 9-5/8" | 8.681" | Intermediate |
| 8-1/2" | 7" | 6.151" | Production |
| 6-1/8" | 4-1/2" | 3.833" | Liner |

### Clearance Requirements

**Minimum Annular Clearances:**
- Casing: 0.75" radial (OD to hole)
- Cement: Design for 360° coverage
- Centralizers: Achieve > 70% standoff

---

## Directional Considerations

### Well Profile Types

| Profile | Description | Application |
|---------|-------------|-------------|
| Vertical | < 3° inclination | Simple reservoirs |
| Slant | Build to angle, hold to TD | Avoiding obstacles |
| S-curve | Build, hold, drop to vertical | Deep vertical targets |
| J-curve | Build to angle, continue at angle | Horizontal section |
| Horizontal | > 85° through target | Unconventional, thin zones |

### Dogleg Severity Limits

| Operation | Max DLS (°/100ft) |
|-----------|-------------------|
| Running casing | 3-6° |
| Running tubing | 8-12° |
| Wireline operations | 15-20° |
| Drilling | 3-6° |

### Torque and Drag Considerations

- Model T&D before spud
- Design for worst case (stuck pipe)
- Include safety factors
- Consider buckling limits

---

## Formation Evaluation Requirements

### Logging Program Selection

| Formation | Recommended Logs |
|-----------|------------------|
| Reservoir | GR, Resistivity, Porosity, NMR |
| Cap Rock | GR, Resistivity, Image |
| Problem Zones | Image, Caliper, Sonic |
| Casing Depth | GR, Resistivity (correlation) |

### Evaluation Points

```
□ Pre-drill: Offset data analysis
□ While drilling: MWD/LWD, mud logs
□ Before casing: Wireline logs, cores
□ Post-cement: CBL/VDL, temperature
□ Completion: Production logs, PLT
```

---

## Wellbore Stability

### Stability Factors

| Factor | Mitigation |
|--------|------------|
| Shale instability | Inhibited mud, high MW |
| Sand production | Adequate MW, gravel pack |
| Fractured formations | Lost circulation material |
| Salt | Saturated mud, undersaturated |
| Reactive clays | Inhibited mud systems |

### Mud Weight Window

**Minimum:**
- Pore pressure gradient + trip margin (0.2-0.5 ppg)
- Borehole stability requirement

**Maximum:**
- Fracture gradient - safety margin (0.2-0.5 ppg)
- Formation damage consideration

---

## Design Workflow

### Step-by-Step Process

1. **Data Gathering**
   - Offset well data
   - Seismic interpretation
   - Geological prognosis
   - Regulatory requirements

2. **Pressure Analysis**
   - Pore pressure prediction
   - Fracture gradient estimation
   - Uncertainty analysis

3. **Casing Design**
   - Setting depth selection
   - Size and weight selection
   - Connection selection
   - Load case analysis

4. **Directional Planning**
   - Survey program
   - BHA requirements
   - T&D modeling

5. **Drilling Program**
   - Mud program
   - Bit selection
   - Hydraulics design

6. **Contingency Planning**
   - Alternative casing points
   - Stuck pipe plan
   - Well control plan

---

## Design Checklist

### Pre-Design Review

```
□ Offset well performance analyzed
□ Geological prognosis received
□ Pressure data validated
□ Target coordinates confirmed
□ Regulatory requirements identified
□ Lease/surface constraints known
```

### Design Validation

```
□ Casing design checked by peer
□ T&D model run and validated
□ Hydraulics program acceptable
□ Cement design adequate
□ Risk assessment complete
□ Contingency plans documented
```

---

## Related Documents

- [Casing Design](../02-drilling-operations/casing-design.md)
- [Directional Planning](../04-directional-drilling/directional-planning.md)
- [Mud Programs](../02-drilling-operations/mud-programs.md)
- [Pre-Spud Checklist](./pre-spud-checklist.md)
