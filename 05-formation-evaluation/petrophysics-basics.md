# Petrophysics Basics

## Overview

Petrophysics is the study of rock properties and their interaction with fluids. For the Company Man, understanding petrophysical concepts enables informed decisions about logging programs, completion intervals, and well potential.

---

## Fundamental Properties

### Porosity (φ)

**Definition**: Fraction of rock volume that is void space

```
φ = Pore Volume / Bulk Volume

Expressed as decimal (0.20) or percentage (20%)
```

**Porosity Types**:

| Type | Description | Wireline Response |
|------|-------------|-------------------|
| **Total porosity** | All void space | Density, neutron |
| **Effective porosity** | Connected pore space | NMR, core |
| **Primary porosity** | Original depositional | Intergranular |
| **Secondary porosity** | Post-depositional | Fractures, vugs |

**Typical Porosity Ranges**:

| Rock Type | Porosity Range |
|-----------|----------------|
| Sandstone | 5-30% |
| Limestone | 2-25% |
| Dolomite | 5-20% |
| Shale | 3-10% (ineffective) |
| Granite | <2% |

### Permeability (k)

**Definition**: Measure of rock's ability to transmit fluids

**Units**: Millidarcies (md)

**Darcy's Law**:
```
Q = (k × A × ΔP) / (μ × L)

Where:
Q = Flow rate
k = Permeability
A = Cross-sectional area
ΔP = Pressure differential
μ = Fluid viscosity
L = Length
```

**Permeability Classification**:

| Classification | Permeability (md) |
|----------------|-------------------|
| Very tight | < 0.01 |
| Tight | 0.01 - 1 |
| Low | 1 - 10 |
| Moderate | 10 - 100 |
| Good | 100 - 1000 |
| Excellent | > 1000 |

### Saturation (S)

**Definition**: Fraction of pore space occupied by a fluid

```
Sw + So + Sg = 1.0 (100%)

Where:
Sw = Water saturation
So = Oil saturation
Sg = Gas saturation
```

**Saturation Types**:

| Term | Definition |
|------|------------|
| **Sw (Water saturation)** | Fraction of pores with water |
| **Swi (Irreducible water)** | Water that won't flow |
| **Sor (Residual oil)** | Oil that won't flow after water flood |
| **Hydrocarbon saturation** | Sh = 1 - Sw = So + Sg |

---

## Log-Derived Calculations

### Porosity from Density Log

```
φD = (ρma - ρb) / (ρma - ρf)

Where:
ρma = Matrix density (g/cc)
ρb = Bulk density from log (g/cc)
ρf = Fluid density (g/cc)

Matrix Densities:
- Sandstone: 2.65 g/cc
- Limestone: 2.71 g/cc
- Dolomite: 2.87 g/cc

Fluid Density:
- Fresh mud: 1.0 g/cc
- Salt mud: 1.1 g/cc
```

**Example**:
```
Given: Sandstone, ρb = 2.35 g/cc, ρf = 1.0 g/cc
φD = (2.65 - 2.35) / (2.65 - 1.0)
φD = 0.30 / 1.65 = 0.182 = 18.2%
```

### Porosity from Sonic Log

**Wyllie Time-Average**:
```
φS = (Δt - Δtma) / (Δtf - Δtma)

Where:
Δt = Log reading (μs/ft)
Δtma = Matrix travel time (μs/ft)
Δtf = Fluid travel time (189 μs/ft for water)

Matrix Travel Times:
- Sandstone: 55.5 μs/ft
- Limestone: 47.5 μs/ft
- Dolomite: 43.5 μs/ft
```

### Porosity from Neutron-Density

**Crossplot Porosity**:
```
φN-D = (φN + φD) / 2

Note: In gas zones, use:
φN-D = √((φN² + φD²) / 2)
```

---

## Water Saturation Calculations

### Archie Equation

**The fundamental equation for water saturation**:

```
Sw = ((a × Rw) / (φ^m × Rt))^(1/n)

Where:
Sw = Water saturation (fraction)
a = Tortuosity factor
Rw = Formation water resistivity (ohm-m)
φ = Porosity (fraction)
m = Cementation exponent
Rt = True formation resistivity (ohm-m)
n = Saturation exponent

Common Parameters:
        a    m    n
Sandstone:   0.81  2.0  2.0
Carbonates:  1.0   2.0  2.0
Humble eq:   0.62  2.15 2.0
```

**Example Calculation**:
```
Given:
φ = 0.20, Rt = 25 ohm-m, Rw = 0.05 ohm-m
a = 0.81, m = 2, n = 2

Sw = ((0.81 × 0.05) / (0.20² × 25))^(1/2)
Sw = (0.0405 / 1.0)^0.5
Sw = 0.201 = 20.1%

Hydrocarbon saturation = 1 - 0.201 = 79.9%
```

### Simandoux Equation (Shaly Sands)

For formations with significant shale content:

```
Sw = ((a × Rw) / (2 × φ^m)) × [-Vsh/Rsh + √((Vsh/Rsh)² + (4 × φ^m) / (a × Rw × Rt))]

Where:
Vsh = Shale volume (fraction)
Rsh = Shale resistivity (ohm-m)
```

---

## Shale Volume (Vsh)

### From Gamma Ray

```
IGR = (GRlog - GRmin) / (GRmax - GRmin)

Where:
IGR = Gamma ray index
GRlog = Log reading
GRmin = Clean sand GR
GRmax = Shale GR
```

**Linear Method**:
```
Vsh = IGR
```

**Steiber Method** (reduces Vsh in older rocks):
```
Vsh = IGR / (3 - 2 × IGR)
```

**Clavier Method**:
```
Vsh = 1.7 - √(3.38 - (IGR + 0.7)²)
```

### Typical Vsh Cutoffs

| Vsh | Classification |
|-----|----------------|
| 0-10% | Clean sand |
| 10-25% | Slightly shaly |
| 25-40% | Shaly sand |
| 40-75% | Sandy shale |
| >75% | Shale |

---

## Net Pay Determination

### Cutoff Parameters

| Parameter | Typical Cutoff | Purpose |
|-----------|----------------|---------|
| **Porosity** | > 6-10% | Minimum storage capacity |
| **Sw** | < 50-70% | Hydrocarbon present |
| **Vsh** | < 40-50% | Producible sand |
| **Permeability** | > 0.1-1 md | Flow capacity |

### Net Pay Calculation

```
Net Pay = Gross Pay × (1 - Vsh) × (1 - φ cutoff failures)

Or simply:
Net Pay = Sum of intervals meeting all cutoffs
```

### Pay Flag Logic

```
IF (φ > φ_cutoff)
   AND (Sw < Sw_cutoff)
   AND (Vsh < Vsh_cutoff)
THEN Pay = Yes
ELSE Pay = No
```

---

## Hydrocarbon Volume Calculations

### Original Oil In Place (OOIP)

```
OOIP (STB) = (7758 × A × h × φ × (1-Sw)) / Bo

Where:
7758 = Conversion factor (acre-ft to bbl)
A = Area (acres)
h = Net pay thickness (ft)
φ = Porosity (fraction)
Sw = Water saturation (fraction)
Bo = Oil formation volume factor (RB/STB)
```

### Original Gas In Place (OGIP)

```
OGIP (SCF) = (43,560 × A × h × φ × (1-Sw)) / Bg

Where:
43,560 = Conversion factor (acre-ft to ft³)
Bg = Gas formation volume factor (RCF/SCF)
```

### Quick Estimate Example

```
Given:
Area = 640 acres (1 section)
h = 20 ft net pay
φ = 18%
Sw = 25%
Bo = 1.3

OOIP = (7758 × 640 × 20 × 0.18 × 0.75) / 1.3
OOIP = 10,308,369 STB ≈ 10.3 MMSTB
```

---

## Formation Water Resistivity (Rw)

### From SP Log

```
Rmf/Rwe = 10^(SP/(-61 + 0.133×Tf))

Where:
SP = Spontaneous potential (mV)
Tf = Formation temperature (°F)
Rmf = Mud filtrate resistivity
Rwe = Equivalent formation water resistivity
```

### From Catalog

Use water analysis data from offset wells or published databases

### Temperature Correction

```
R2 = R1 × (T1 + 6.77) / (T2 + 6.77)

Where:
R1 = Resistivity at T1
R2 = Resistivity at T2
T1, T2 = Temperatures (°F)
```

---

## Quick Look Interpretation

### Gas Zone Indicators

```
┌─────────────────────────────────────────┐
│  Density─────────┐                      │
│                  │ Crossover            │
│  Neutron────────┘  (Neutron reads low)  │
│                                         │
│  High Resistivity                       │
│  Elevated Sonic (possible)              │
│  Gas on mudlog                          │
└─────────────────────────────────────────┘
```

### Oil Zone Indicators

```
┌─────────────────────────────────────────┐
│  Density and Neutron track together     │
│  (No significant crossover)             │
│                                         │
│  High Resistivity                       │
│  Low Sw calculated                      │
│  Oil shows on mudlog                    │
└─────────────────────────────────────────┘
```

### Water Zone Indicators

```
┌─────────────────────────────────────────┐
│  Density and Neutron track together     │
│  Low Resistivity                        │
│  Sw ≈ 100%                              │
│  No shows on mudlog                     │
└─────────────────────────────────────────┘
```

---

## Common Interpretation Pitfalls

| Pitfall | Cause | Solution |
|---------|-------|----------|
| **Overestimate φ in gas** | Low neutron | Use density only or gas correction |
| **Underestimate Sw** | Use Rt instead of Rxo | Verify invasion profile |
| **Wrong matrix** | Unknown lithology | Use crossplots, core data |
| **Bad Rw** | Wrong salinity | Get water sample, use SP |
| **Shale effects** | Ignoring Vsh | Use shaly sand equations |
| **Thin beds** | Below resolution | Consider resolution limits |

---

## Petrophysics Deliverables

| Deliverable | Contents | Use |
|-------------|----------|-----|
| **Interpreted log** | Calculated curves | Visualization |
| **Formation summary** | Net pay, averages | Quick reference |
| **Reservoir table** | Zone-by-zone properties | Completion design |
| **OOIP/OGIP estimate** | Volumetrics | Reserve booking |
| **Fluid contacts** | OWC, GOC, GWC | Field development |
