# Hydraulics Calculations

## Pressure Loss Fundamentals

### Total System Pressure
```
P(total) = P(surface) + P(drillstring) + P(bit) + P(annulus)

Where each term represents pressure loss in that section
```

### Flow Regime Determination
```
Reynolds Number (NRe):
Pipe: NRe = 928 × ρ × V × D ÷ μ
Annulus: NRe = 757 × ρ × V × (Dh - Dp) ÷ μ

Where:
ρ = Mud weight (ppg)
V = Velocity (ft/sec)
D = Diameter (inches)
μ = Plastic viscosity (cp)

NRe < 2100: Laminar flow
NRe > 4000: Turbulent flow
2100 < NRe < 4000: Transition
```

## Pipe Flow Pressure Losses

### Pressure Loss in Pipe (Turbulent)
```
ΔP (psi) = (ρ^0.8 × Q^1.8 × PV^0.2 × L) ÷ (1800 × D^4.8)

Where:
ρ = Mud weight (ppg)
Q = Flow rate (gpm)
PV = Plastic viscosity (cp)
L = Length (ft)
D = Inside diameter (inches)
```

### Pressure Loss in Pipe (Laminar)
```
ΔP (psi) = (PV × L × V) ÷ (1500 × D²) + (τy × L) ÷ (225 × D)

Where:
τy = Yield point (lb/100ft²)
V = Velocity (ft/sec)
```

### Simplified Pipe Loss
```
ΔP (psi) = f × (L ÷ D) × (ρ × V²) ÷ 25.8

Where f = Fanning friction factor
```

## Annular Flow Pressure Losses

### Annular Velocity
```
V (ft/sec) = Q ÷ (2.448 × (Dh² - Dp²))

or

V (ft/min) = 24.5 × Q ÷ (Dh² - Dp²)

Where:
Q = Flow rate (gpm)
Dh = Hole/casing ID (inches)
Dp = Pipe OD (inches)
```

### Annular Pressure Loss (Turbulent)
```
ΔP (psi) = (ρ^0.8 × Q^1.8 × PV^0.2 × L) ÷ (1396 × (Dh - Dp)^3 × (Dh + Dp)^1.8)
```

### Annular Pressure Loss (Laminar)
```
ΔP (psi) = (PV × L × V) ÷ (1000 × (Dh - Dp)²) + (τy × L) ÷ (200 × (Dh - Dp))
```

## Equivalent Circulating Density (ECD)

### ECD Calculation
```
ECD (ppg) = MW + (Annular Pressure Loss ÷ (0.052 × TVD))

Example:
MW = 12.0 ppg
APL = 400 psi
TVD = 10,000 ft

ECD = 12.0 + (400 ÷ (0.052 × 10,000))
ECD = 12.0 + 0.77 = 12.77 ppg
```

### ECD with Cuttings Load
```
ECD(total) = ECD(mud) + ECD(cuttings)

ECD(cuttings) ≈ 0.2 to 0.5 ppg additional
(Depends on ROP, hole cleaning efficiency)
```

### Surge/Swab Pressure
```
Surge: Additional pressure from running pipe in
Swab: Pressure reduction from pulling pipe out

Rule of thumb:
Keep surge < 0.5 ppg EMW increase
Keep swab < 0.5 ppg EMW decrease

Controlled by:
- Trip speed
- Mud properties
- Annular clearance
```

## Bit Hydraulics

### Nozzle Area
```
Total Flow Area (TFA) in²:
TFA = Σ (Nozzle diameter in 32nds)² ÷ 1303.8

Example: 3 × 12/32" nozzles
TFA = 3 × 12² ÷ 1303.8 = 0.331 in²
```

### Pressure Drop Across Bit
```
ΔP(bit) = (ρ × Q²) ÷ (10,858 × TFA²)

Example:
12 ppg mud, 500 gpm, TFA = 0.331 in²
ΔP = (12 × 500²) ÷ (10,858 × 0.331²)
ΔP = 3,000,000 ÷ 1,189 = 2,523 psi
```

### Nozzle Velocity
```
V(nozzle) (ft/sec) = 417.2 × Q ÷ TFA

Example:
500 gpm, TFA = 0.331 in²
V = 417.2 × 500 ÷ 0.331 = 630 ft/sec
```

### Hydraulic Horsepower at Bit
```
HHP = (Q × ΔP) ÷ 1714

Example:
500 gpm, 2,500 psi bit pressure drop
HHP = (500 × 2,500) ÷ 1714 = 729 HP
```

### Hydraulic Horsepower per Square Inch (HSI)
```
HSI = HHP ÷ Bit Area

Bit Area = π × D² ÷ 4

Example: 8.5" bit, 729 HP
Area = 3.14159 × 8.5² ÷ 4 = 56.7 in²
HSI = 729 ÷ 56.7 = 12.9 HP/in²

Target: 2.5-5.0 HSI for most formations
```

### Impact Force
```
IF (lb) = 0.01823 × Q × √(ρ × ΔP)

or

IF (lb) = V(nozzle) × Q × ρ ÷ 1932.7

Example:
500 gpm, 12 ppg, 2,500 psi
IF = 0.01823 × 500 × √(12 × 2,500)
IF = 9.115 × 173.2 = 1,579 lb
```

## Optimization Methods

### Maximum Bit Hydraulics
```
Optimal ΔP(bit) = 65% of available pressure

If pump pressure = 3,000 psi available:
Parasitic losses (pipe + annulus) = 35% = 1,050 psi
Bit pressure drop = 65% = 1,950 psi
```

### Maximum Impact Force Method
```
Optimal ΔP(bit) = 48-52% of available pressure

Balance between velocity and flow rate for max cleaning force
```

### Nozzle Selection
```
Given desired ΔP(bit), solve for TFA:

TFA = Q × √(ρ ÷ (10,858 × ΔP))

Then select nozzle combination to achieve TFA

Common combinations:
- 3 equal nozzles: Simple, balanced flow
- 2 large + 1 small: Extended gauge protection
- 1 large + 2 small: Specific jetting patterns
```

## Cuttings Transport

### Slip Velocity
```
V(slip) = velocity at which cuttings fall through mud

For vertical hole:
V(slip) (ft/min) ≈ 1.04 × (d^0.667 × (ρs - ρm)^0.333) ÷ (ρm^0.333 × μ^0.333)

Where:
d = Cutting diameter (in)
ρs = Cutting density (ppg)
ρm = Mud density (ppg)
μ = Effective viscosity
```

### Transport Ratio
```
TR = (V(annular) - V(slip)) ÷ V(annular)

TR > 0.5 desired for adequate hole cleaning
TR approaching 1.0 = very good cleaning
TR < 0.3 = poor cleaning, cuttings accumulating
```

### Minimum Annular Velocity
```
Vertical well: 100-150 ft/min minimum
Deviated (30-60°): 150-180 ft/min minimum
Horizontal: 180-250 ft/min minimum

Adjust upward for:
- Larger cuttings
- Higher ROP
- Sticky formations
```

### Critical Velocity
```
V(critical) = velocity at which cuttings transport is marginal

V(crit) ≈ V(slip) × 2

Maintain V(annular) > V(critical) for all sections
```

## Power Law Model

### Power Law Parameters
```
n = 3.32 × log(θ600 ÷ θ300)
K = θ300 ÷ 511^n

Where θ readings from viscometer

Example:
θ600 = 60, θ300 = 35
n = 3.32 × log(60/35) = 3.32 × 0.234 = 0.78
K = 35 ÷ 511^0.78 = 35 ÷ 162.6 = 0.215 lb-sec^n/100ft²
```

### Power Law Pressure Loss
```
More accurate for non-Newtonian fluids
Used in advanced hydraulics software

ΔP depends on K, n, geometry, and flow rate
```

## Quick Reference

### Typical System Pressure Distribution

| Component | % of Total | Example @ 3000 psi |
|-----------|-----------|-------------------|
| Surface equipment | 5-10% | 150-300 psi |
| Drill pipe | 20-30% | 600-900 psi |
| Drill collars | 5-10% | 150-300 psi |
| Bit | 45-65% | 1350-1950 psi |
| Annulus | 10-20% | 300-600 psi |

### Minimum Annular Velocity Guidelines

| Hole Angle | Minimum AV (ft/min) |
|------------|-------------------|
| 0-30° | 100-120 |
| 30-60° | 150-180 |
| 60-90° | 180-250 |

### Target Hydraulic Parameters

| Parameter | Range | Optimal |
|-----------|-------|---------|
| HSI (HP/in²) | 2-7 | 3-5 |
| Impact Force (lb) | 800-2000 | 1200-1600 |
| Nozzle velocity (ft/s) | 250-450 | 300-400 |
| % Pressure at bit | 48-65% | 55-60% |

---

*Hydraulic optimization should be recalculated as drilling parameters and hole geometry change.*
