# Drilling Calculations

## Basic Drilling Parameters

### Rate of Penetration (ROP)
```
ROP (ft/hr) = (Depth Drilled (ft) × 60) ÷ Time (min)

Example:
Drilled 30 ft in 45 minutes
ROP = (30 × 60) ÷ 45 = 40 ft/hr
```

### Rotary Speed
```
Surface RPM = (Bit RPM) - (Motor RPM × Motor Bend Factor)

For motor drilling:
Bit RPM = Surface RPM + Motor RPM

Example:
Surface = 60 RPM, Motor = 180 RPM @ 40 gpm/rev
Bit RPM = 60 + 180 = 240 RPM
```

### Weight on Bit (WOB)
```
WOB = Hook Load (off bottom) - Hook Load (on bottom)

Example:
Off bottom: 250,000 lb
On bottom: 220,000 lb
WOB = 250,000 - 220,000 = 30,000 lb = 30 klb
```

## Pipe Capacities and Displacements

### Pipe Capacity (bbl/ft)
```
Capacity (bbl/ft) = ID² ÷ 1029.4

Example: 5" DP with 4.276" ID
Capacity = 4.276² ÷ 1029.4 = 0.01776 bbl/ft
```

### Pipe Displacement (bbl/ft)
```
Displacement (bbl/ft) = (OD² - ID²) ÷ 1029.4

Example: 5" DP, 4.276" ID
Displacement = (5² - 4.276²) ÷ 1029.4 = 0.00653 bbl/ft
```

### Annular Capacity (bbl/ft)
```
Annular Capacity (bbl/ft) = (Hole ID² - Pipe OD²) ÷ 1029.4

Example: 8.5" hole, 5" DP
Capacity = (8.5² - 5²) ÷ 1029.4 = 0.0459 bbl/ft
```

### Total String Capacity
```
Total Capacity (bbl) = Σ (Length × Capacity per section)

Example:
DP: 9000 ft × 0.01776 bbl/ft = 159.84 bbl
DC: 500 ft × 0.00742 bbl/ft = 3.71 bbl
HWDP: 500 ft × 0.00883 bbl/ft = 4.42 bbl
Total = 167.97 bbl
```

## Strokes and Volumes

### Strokes to Displace
```
Strokes = Volume (bbl) ÷ Pump Output (bbl/stk)

Pump Output (bbl/stk) = (Liner ID² × Stroke Length × Efficiency) ÷ 1029.4

Example: Triplex pump
Liner: 6" ID, Stroke: 12", Efficiency: 95%
Output = (6² × 12 × 0.95) ÷ 1029.4 = 0.0399 bbl/stk
```

### Bottoms Up Time
```
Time (min) = Annular Volume (bbl) ÷ Flow Rate (bbl/min)

Flow Rate (bbl/min) = GPM ÷ 42

Example:
Annular volume: 350 bbl, Flow rate: 500 gpm
Time = 350 ÷ (500/42) = 350 ÷ 11.9 = 29.4 min
```

### Lag Time
```
Lag Time (min) = Annular Volume (bbl) ÷ Flow Rate (bbl/min)

For depth to surface:
Total Lag = (Annular Volume from bit to surface) ÷ Flow Rate
```

## Drilling Fluid Hydraulics

### Annular Velocity (AV)
```
AV (ft/min) = (24.5 × GPM) ÷ (Dh² - Dp²)

Where:
Dh = Hole diameter (inches)
Dp = Pipe diameter (inches)
GPM = Flow rate

Example: 500 gpm, 8.5" hole, 5" pipe
AV = (24.5 × 500) ÷ (8.5² - 5²)
AV = 12,250 ÷ 47.25 = 259 ft/min
```

### Minimum Annular Velocity (Rule of Thumb)
```
For cuttings transport:
Minimum AV = 100-150 ft/min (vertical)
Minimum AV = 150-200 ft/min (deviated >45°)
```

### Jet Velocity
```
Vj (ft/sec) = (417.2 × GPM) ÷ (Nozzle Area)

Nozzle Area (sq in) = Σ (Nozzle Size²) × 0.7854

Example: 3 × 12/32" nozzles at 500 gpm
Area = 3 × (12/32)² × 0.7854 = 0.331 sq in
Vj = (417.2 × 500) ÷ 0.331 = 630 ft/sec
```

### Bit Hydraulic Horsepower (HHP)
```
HHP = (GPM × ΔP) ÷ 1714

Where ΔP = Pressure drop across bit (psi)

Example: 500 gpm, 1500 psi bit pressure drop
HHP = (500 × 1500) ÷ 1714 = 437.6 HP
```

### Impact Force
```
IF (lb) = (GPM × MW × Vj) ÷ 1930

Example: 500 gpm, 12 ppg mud, 630 ft/sec
IF = (500 × 12 × 630) ÷ 1930 = 1960 lb
```

## Pressure Calculations

### Hydrostatic Pressure
```
HP (psi) = 0.052 × MW (ppg) × TVD (ft)

Example: 12 ppg mud at 10,000 ft TVD
HP = 0.052 × 12 × 10,000 = 6,240 psi
```

### Pressure Gradient
```
Gradient (psi/ft) = 0.052 × MW (ppg)

Example: 12 ppg mud
Gradient = 0.052 × 12 = 0.624 psi/ft
```

### Equivalent Mud Weight (EMW)
```
EMW (ppg) = BHP (psi) ÷ (0.052 × TVD)

Example: BHP = 6,500 psi at 10,000 ft TVD
EMW = 6,500 ÷ (0.052 × 10,000) = 12.5 ppg
```

### Equivalent Circulating Density (ECD)
```
ECD (ppg) = MW + (Annular Pressure Loss ÷ (0.052 × TVD))

Example: 12 ppg mud, 500 psi APL, 10,000 ft TVD
ECD = 12 + (500 ÷ (0.052 × 10,000)) = 12.96 ppg
```

## Drilling Parameter Optimization

### Specific Energy
```
SE (psi) = (480 × WOB × RPM) ÷ (D² × ROP)

Where D = Bit diameter (inches)

Lower SE = More efficient drilling

Example: 30 klb WOB, 120 RPM, 8.5" bit, 50 ft/hr ROP
SE = (480 × 30,000 × 120) ÷ (8.5² × 50 × 1000)
SE = 1,728,000,000 ÷ 3,612,500 = 478 psi
```

### D-Exponent
```
d = log(ROP ÷ (60 × N)) ÷ log((12 × W) ÷ (1000 × D))

Where:
ROP = Rate of penetration (ft/hr)
N = Rotary speed (RPM)
W = Weight on bit (lb)
D = Bit diameter (in)
```

### Corrected D-Exponent
```
dc = d × (Normal MW ÷ Actual MW)

Used for pore pressure detection
```

## Trip Calculations

### Pipe Light Weight
```
Light Weight (lb) = (Buoyed Weight in mud) × Safety Factor

Buoyancy Factor = (65.5 - MW) ÷ 65.5

Example: 10,000 ft of 19.5 lb/ft DP in 12 ppg mud
BF = (65.5 - 12) ÷ 65.5 = 0.817
String Weight = 10,000 × 19.5 × 0.817 = 159,315 lb
```

### Swab Pressure
```
Swab Pressure (psi) ≈ Clinging Factor × Pipe Speed × Mud Properties

Rule of Thumb:
Max Trip Speed = 2-3 ft/sec to limit swab to ~50 psi
```

### Surge Pressure
```
Surge Pressure (psi) = f(Pipe Speed, Annular Clearance, Mud Properties)

Keep surge < (Frac Pressure - Static Mud Pressure)
Typical: Limit to 100-200 psi equivalent
```

## Quick Reference Tables

### Common Pipe Capacities (bbl/ft)

| Pipe | ID (in) | Capacity | Displacement |
|------|---------|----------|--------------|
| 3½" DP | 2.764 | 0.00742 | 0.00462 |
| 4½" DP | 3.826 | 0.01422 | 0.00537 |
| 5" DP | 4.276 | 0.01776 | 0.00653 |
| 5½" DP | 4.778 | 0.02219 | 0.00715 |
| 6⅝" DC | 2.25 | 0.00492 | 0.03806 |
| 8" DC | 2.813 | 0.00769 | 0.05403 |

### Common Hole Sizes and Capacities

| Hole Size | Capacity (bbl/ft) |
|-----------|------------------|
| 6" | 0.0350 |
| 8½" | 0.0702 |
| 9⅞" | 0.0947 |
| 12¼" | 0.1458 |
| 17½" | 0.2975 |

---

*Always double-check critical calculations. Use consistent units throughout.*
