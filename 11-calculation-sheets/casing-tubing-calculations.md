# Casing & Tubing Calculations

## Weight and Capacity

### Pipe Weight (in air)
```
Weight (lb/ft) = Nominal weight from manufacturer

Approximate weight:
Weight ≈ 10.68 × (OD - t) × t

Where:
OD = Outside diameter (inches)
t = Wall thickness (inches)
```

### Buoyed Weight
```
Buoyancy Factor (BF) = (65.5 - MW) ÷ 65.5

or

BF = 1 - (MW ÷ 65.5)

Buoyed Weight = Air Weight × BF

Example:
10,000 ft of 47 lb/ft casing in 12 ppg mud
BF = (65.5 - 12) ÷ 65.5 = 0.817
Air Weight = 10,000 × 47 = 470,000 lb
Buoyed Weight = 470,000 × 0.817 = 384,000 lb
```

### Pipe Capacity
```
Capacity (bbl/ft) = ID² ÷ 1029.4

Capacity (gal/ft) = ID² × 0.0408

Example: 7" casing, 6.366" ID
Capacity = 6.366² ÷ 1029.4 = 0.0394 bbl/ft
```

### Pipe Displacement
```
Closed End: Displacement = (OD² - ID²) ÷ 1029.4

Open End: Displacement = OD² ÷ 1029.4

Example: 7" casing, 6.366" ID (closed)
Displacement = (7² - 6.366²) ÷ 1029.4 = 0.0083 bbl/ft
```

## Burst and Collapse Ratings

### Burst Pressure (Barlow Formula)
```
P(burst) = (2 × YS × t) ÷ OD

Where:
YS = Yield strength (psi)
t = Wall thickness (inches)
OD = Outside diameter (inches)

Example: 7" 29# N-80 casing
t = 0.362", YS = 80,000 psi
P(burst) = (2 × 80,000 × 0.362) ÷ 7 = 8,274 psi

Apply design factor (typically 1.1-1.25)
Working burst = 8,274 ÷ 1.1 = 7,522 psi
```

### Collapse Pressure
```
Collapse rating from API tables (more complex formula)

Approximate for thin wall:
P(collapse) ≈ 2 × YS × (t/OD)²

For D/t ratios:
- Yield collapse: D/t < 12
- Plastic collapse: 12 < D/t < 20
- Transition collapse: 20 < D/t < 25
- Elastic collapse: D/t > 25
```

### Tension Rating
```
P(tension) = YS × A(cross-section)

A = 0.7854 × (OD² - ID²)

Example: 7" 29# N-80
A = 0.7854 × (7² - 6.276²) = 8.53 in²
P(tension) = 80,000 × 8.53 = 682,400 lb
```

## Design Factors

### Minimum Design Factors
```
Burst: DF ≥ 1.1 (exploration) to 1.25 (production)
Collapse: DF ≥ 1.0 to 1.125
Tension: DF ≥ 1.6 to 2.0
Triaxial: DF ≥ 1.25
```

### Design Factor Calculation
```
DF = Rating ÷ Load

Example:
Casing burst rating = 8,300 psi
Maximum internal pressure = 6,000 psi
DF = 8,300 ÷ 6,000 = 1.38 (acceptable)
```

## Load Calculations

### Burst Load
```
Internal Pressure = Formation pressure (or test pressure)
External Pressure = Mud hydrostatic (or pore pressure)

Net Burst = Internal - External

Example:
Test pressure = 5,000 psi inside
Mud outside = 0.052 × 10 × 8,000 = 4,160 psi
Net Burst = 5,000 - 4,160 = 840 psi
```

### Collapse Load
```
External Pressure = Mud hydrostatic (or formation pressure)
Internal Pressure = Fluid inside casing

Net Collapse = External - Internal

Worst case: Empty casing (evacuation scenario)
Net Collapse = 0.052 × MW × TVD - 0
```

### Tension Load
```
Running Tension:
T = Buoyed weight of casing below point

At surface during landing:
T = Total buoyed weight + drag + shock loads

Shock Load (approximate):
Shock (lb) = 3,200 × Weight per foot
```

### Biaxial Loading
```
Axial tension reduces collapse resistance
Combined loading check required

Reduced Collapse = Collapse Rating × √(1 - (Tension/Yield Tension)²)
```

## Thread Calculations

### Thread Makeup Torque
```
From API/manufacturer specifications

Approximate minimum:
Torque (ft-lb) ≈ 0.12 × Yield × OD × t

Actual torque depends on:
- Thread type (API, premium)
- Pipe grade
- Thread compound
```

### Thread Tensile Rating
```
API thread joint efficiency:
Round (STC): 50-60% of pipe body
Round (LTC): 65-75% of pipe body
Buttress (BTC): 85-95% of pipe body
Premium: 95-100% of pipe body
```

## Casing Wear

### Wear Calculation
```
Wear (%) = (Original Wall - Remaining Wall) ÷ Original Wall × 100

Remaining Strength:
Burst: Linear with remaining wall
Collapse: Approximately linear
Tension: Based on remaining cross-section
```

### Maximum Allowable Wear
```
Typically limit wear to:
- 20% for production casing
- 15% for critical wells
- Industry specific requirements apply
```

## Stretch and Elongation

### Free Pipe Stretch
```
ΔL (ft) = (W × L²) ÷ (2 × A × E)

Where:
W = Buoyed weight per foot
L = Length of pipe (ft)
A = Cross-sectional area (in²)
E = Modulus of elasticity (30 × 10⁶ psi for steel)

Simplified:
ΔL (ft) ≈ L² × Weight(lb/ft) × BF ÷ (2.55 × 10⁸ × A)
```

### Stretch from Applied Load
```
ΔL (inches) = (F × L × 12) ÷ (A × E)

Where F = applied force (lb)

Example: 50,000 lb on 10,000 ft of 5" DP (5.275 in² area)
ΔL = (50,000 × 10,000 × 12) ÷ (5.275 × 30,000,000)
ΔL = 37.9 inches = 3.16 ft
```

### Thermal Expansion
```
ΔL (ft) = α × L × ΔT

α = 6.9 × 10⁻⁶ /°F for steel

Example: 10,000 ft casing, 100°F temperature increase
ΔL = 6.9 × 10⁻⁶ × 10,000 × 100 = 6.9 ft
```

## Buckling

### Neutral Point
```
Neutral Point = Depth where buoyed string weight = 0

Below neutral point: Tension
Above neutral point: Compression (buckling possible)
```

### Critical Buckling Force
```
Helical Buckling Force:
F(crit) = √(8 × E × I × W × sin(θ) ÷ r)

Where:
I = Moment of inertia
W = Buoyed weight per unit length
θ = Inclination
r = Radial clearance
```

### Buckling Prevention
```
- Apply sufficient set-down weight
- Use proper centralization
- Consider pre-tensioned completions
- Check for temperature effects
```

## Quick Reference Tables

### Common Casing Data

| Size | Weight | Grade | ID | Burst | Collapse | Tension |
|------|--------|-------|-----|-------|----------|---------|
| 5½" | 17 | N-80 | 4.892 | 7,740 | 6,220 | 404k |
| 7" | 26 | N-80 | 6.276 | 6,340 | 4,320 | 502k |
| 7" | 29 | N-80 | 6.184 | 7,030 | 5,410 | 563k |
| 9⅝" | 47 | N-80 | 8.681 | 6,870 | 4,750 | 918k |
| 13⅜" | 68 | N-80 | 12.415 | 5,020 | 2,260 | 1,069k |

### Common Tubing Data

| Size | Weight | Grade | ID | Burst | Collapse | Tension |
|------|--------|-------|-----|-------|----------|---------|
| 2⅜" | 4.7 | N-80 | 1.995 | 11,200 | 10,250 | 106k |
| 2⅞" | 6.5 | N-80 | 2.441 | 10,570 | 9,520 | 146k |
| 3½" | 9.3 | N-80 | 2.992 | 10,000 | 8,600 | 213k |
| 4½" | 12.75 | N-80 | 3.958 | 9,460 | 7,520 | 284k |

### Buoyancy Factors

| Mud Weight (ppg) | Buoyancy Factor |
|-----------------|-----------------|
| 8.34 | 0.873 |
| 9.0 | 0.863 |
| 10.0 | 0.847 |
| 11.0 | 0.832 |
| 12.0 | 0.817 |
| 13.0 | 0.802 |
| 14.0 | 0.786 |
| 15.0 | 0.771 |
| 16.0 | 0.756 |

---

*Always use API specifications and manufacturer data for critical design calculations. Field calculations are for estimation only.*
