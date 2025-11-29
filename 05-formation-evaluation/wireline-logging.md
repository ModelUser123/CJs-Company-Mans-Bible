# Wireline Logging

## Overview

Wireline logging provides high-resolution formation evaluation data after drilling. Logs are the primary source of petrophysical data for reservoir characterization, completion design, and reserve estimation.

---

## Open Hole Logging Suites

### Triple Combo (Basic Suite)

| Tool | Measurement | Primary Use |
|------|-------------|-------------|
| **Gamma Ray (GR)** | Natural radioactivity | Shale volume, correlation |
| **Resistivity** | Formation resistivity | Fluid saturation |
| **Density** | Bulk density | Porosity, lithology |
| **Neutron** | Hydrogen index | Porosity, gas detection |
| **Caliper** | Hole diameter | Hole condition |

### Quad Combo (Triple + Sonic)

| Additional Tool | Measurement | Primary Use |
|-----------------|-------------|-------------|
| **Sonic** | Acoustic travel time | Porosity, geomechanics |

### Advanced Logging Suite

| Tool | Measurement | Primary Use |
|------|-------------|-------------|
| **Imaging (FMI/UBI)** | Borehole images | Fractures, dip, faults |
| **NMR** | Nuclear magnetic resonance | Porosity, permeability, fluid typing |
| **Spectral GR** | K, U, Th content | Clay typing, source rock |
| **Elemental capture** | Elemental composition | Mineralogy |

---

## Common Logging Tools

### Gamma Ray (GR)

**Principle**: Measures natural radioactivity (K, U, Th)

| Formation | Typical GR (API) |
|-----------|------------------|
| Clean sand | 10-30 |
| Shaly sand | 30-75 |
| Shale | 75-150 |
| Hot shale | 150-300+ |
| Coal | 10-30 |
| Evaporite | 10-30 |

**Uses**:
- Shale volume calculation
- Correlation between wells
- Depth matching
- Net pay determination

### Resistivity

**Types**:

| Tool Type | Depth of Investigation | Use |
|-----------|----------------------|-----|
| **Micro-resistivity** | 1-3 inches | Rxo (flushed zone) |
| **Shallow** | 10-20 inches | Ri (invaded zone) |
| **Medium** | 20-40 inches | Invasion profile |
| **Deep** | 60-90 inches | Rt (true resistivity) |

**Resistivity Interpretation**:

| Resistivity | Fluid |
|-------------|-------|
| < 1 ohm-m | Salt water |
| 1-10 ohm-m | Fresh water or shaly |
| 10-100 ohm-m | Oil or gas |
| > 100 ohm-m | Low porosity or HC |

### Density Log

**Principle**: Gamma ray scattering (Compton scattering)

| Lithology | Matrix Density (g/cc) |
|-----------|----------------------|
| Sandstone | 2.65 |
| Limestone | 2.71 |
| Dolomite | 2.87 |
| Anhydrite | 2.98 |
| Salt | 2.03 |

**Porosity Calculation**:
```
φ = (ρma - ρb) / (ρma - ρf)

Where:
ρma = Matrix density
ρb = Bulk density (from log)
ρf = Fluid density (typically 1.0-1.1 g/cc)
```

### Neutron Log

**Principle**: Hydrogen concentration (primarily measures water/HC in pores)

**Porosity Scale**: Calibrated in limestone porosity units

**Gas Effect**:
- Neutron reads low in gas zones (low hydrogen)
- Density-Neutron crossover indicates gas

### Sonic Log

**Principle**: Acoustic travel time

| Lithology | Matrix DT (µs/ft) |
|-----------|-------------------|
| Sandstone | 55.5 |
| Limestone | 47.5 |
| Dolomite | 43.5 |
| Shale | 60-170 |
| Salt | 67 |

**Porosity Calculation (Wyllie)**:
```
φ = (DT - DTma) / (DTf - DTma)

Where:
DT = Log reading (µs/ft)
DTma = Matrix travel time
DTf = Fluid travel time (189 µs/ft for water)
```

---

## Cased Hole Logging

### Common Cased Hole Tools

| Tool | Purpose |
|------|---------|
| **GR/CCL** | Depth correlation, collar location |
| **Cement Bond Log (CBL)** | Cement quality evaluation |
| **Variable Density Log (VDL)** | Cement/formation bonding |
| **Ultrasonic Imaging** | Casing condition, cement map |
| **Production Log (PLT)** | Flow profile, fluid entry |
| **Casing Inspection** | Casing corrosion, wear |
| **Pulsed Neutron** | Saturation behind casing |

### Cement Bond Log Interpretation

| CBL Amplitude (mV) | Cement Quality |
|-------------------|----------------|
| < 5 | Excellent bond |
| 5-15 | Good bond |
| 15-30 | Fair bond |
| > 30 | Poor/no bond |

**VDL Interpretation**:
- Strong casing arrivals = Poor cement
- Strong formation arrivals = Good cement-formation bond
- Chevron patterns = Good cement

---

## Log Quality Control

### Depth Control

| Issue | Cause | Prevention/Correction |
|-------|-------|----------------------|
| **Depth stretch** | Cable stretch | Tension corrections |
| **Depth slip** | Wheel slippage | Magnetic marks, CCL |
| **Sticking** | Tool stuck | Speed control, tension |

### Environmental Corrections

| Factor | Correction Needed |
|--------|-------------------|
| **Hole size** | Density, neutron, resistivity |
| **Mud weight** | Density, neutron |
| **Mud type** | Resistivity |
| **Temperature** | Resistivity, sonic |
| **Pressure** | Various tools |
| **Invasion** | Resistivity |

### Repeat Section Requirements

| Requirement | Standard |
|-------------|----------|
| **Length** | Minimum 200 ft |
| **Location** | Through zone of interest |
| **Overlay** | Curves should match within specifications |
| **Depth** | Should match within ±1 ft |

---

## Logging Operations

### Pre-Logging Preparation

**Hole Conditioning**:
1. Circulate bottoms-up
2. Short trip to verify hole condition
3. Condition mud (weight, rheology, LGS)
4. Verify open hole to TD

**Company Man Responsibilities**:
- [ ] Approve logging program
- [ ] Verify hole condition
- [ ] Witness surface checks
- [ ] Monitor operations
- [ ] Review preliminary logs
- [ ] Sign logging tickets

### Logging Sequence (Typical)

| Run | Tools | Notes |
|-----|-------|-------|
| **Run 1** | Triple Combo | Main logging run |
| **Run 2** | Sonic/Imaging | If required |
| **Run 3** | Formation Tester | Pressure points, samples |
| **Run 4** | Sidewall Cores | If required |

### Stuck Tool Prevention

| Prevention Measure | Application |
|--------------------|-------------|
| **Circulate clean** | Before logging |
| **Condition hole** | Short trip before logging |
| **Log up** | Log on way out of hole |
| **Speed control** | Appropriate logging speed |
| **Jar placement** | Position jar strategically |
| **Stuck indicators** | Monitor tension, depth |

### If Tool Gets Stuck

1. Do NOT pull more than 2000 lb overpull
2. Work tool gently up and down
3. Try pumping if safe
4. Consider jarring if equipped
5. Discuss with logging company and company
6. Document all attempts and overpull
7. Consider cut and thread operation

---

## Log Interpretation Basics

### Quick-Look Interpretation

| Indicator | What to Look For |
|-----------|------------------|
| **Pay zone** | Low GR, high resistivity, porosity crossover |
| **Gas zone** | Density-Neutron crossover (neutron low) |
| **Oil zone** | High resistivity, matching D-N porosity |
| **Water zone** | Low resistivity, matching D-N porosity |
| **Shale** | High GR, low resistivity, high neutron |
| **Tight** | Low porosity all tools, high resistivity possible |

### Crossplot Analysis

**Density-Neutron Crossplot**:
- Points on limestone line = limestone
- Points shifted NE = gas effect
- Points shifted SW = shale effect

**M-N Crossplot**:
- Lithology identification
- Secondary porosity detection
- Gas effects

### Water Saturation

**Archie Equation**:
```
Sw = ((a × Rw) / (φ^m × Rt))^(1/n)

Where:
a = Tortuosity factor (typically 1.0)
Rw = Formation water resistivity
φ = Porosity
m = Cementation exponent (typically 2.0)
Rt = True resistivity
n = Saturation exponent (typically 2.0)
Sw = Water saturation
```

**Pay Criteria (Example)**:
- Sw < 50% = Pay
- 50% < Sw < 70% = Transition
- Sw > 70% = Water

---

## Logging Program Considerations

### When to Log

| Scenario | Logging Recommendation |
|----------|----------------------|
| **Exploration well** | Full suite, formation testing |
| **Development well** | Triple combo + cement |
| **Horizontal well** | LWD primary, wireline if rathole |
| **Deep well** | Temperature-rated tools |
| **H2S well** | H2S-rated tools |

### Log Data Delivery

| Format | Use |
|--------|-----|
| **LAS** | Industry standard, analysis software |
| **DLIS** | Full waveform data, archives |
| **PDF** | Quick viewing, reports |
| **Paper** | Field reference |

### Logging Checklist

- [ ] Confirm logging program with operations
- [ ] Verify tool ratings for hole conditions
- [ ] Condition hole before logging
- [ ] Witness calibrations and before/after surveys
- [ ] Monitor all logging operations
- [ ] Review logs before releasing logging unit
- [ ] Verify depth accuracy (repeat sections)
- [ ] Obtain preliminary prints and digital data
- [ ] Sign service tickets
