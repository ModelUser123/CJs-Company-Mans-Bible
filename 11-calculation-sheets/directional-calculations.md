# Directional Calculations

## Basic Survey Calculations

### Inclination and Azimuth
```
Inclination (I): Angle from vertical (0° = vertical, 90° = horizontal)
Azimuth (A): Compass direction (0°/360° = North, 90° = East, 180° = South, 270° = West)
```

### Measured Depth (MD) vs True Vertical Depth (TVD)
```
For a single survey station:
TVD = MD × cos(I)

Note: This is simplified. Actual calculations use methods below.
```

## Survey Calculation Methods

### Tangential Method (Least Accurate)
```
ΔN = ΔMD × sin(I2) × cos(A2)
ΔE = ΔMD × sin(I2) × sin(A2)
ΔTVD = ΔMD × cos(I2)

Where I2, A2 are values at lower survey station
```

### Average Angle Method
```
Average Inclination: Iavg = (I1 + I2) ÷ 2
Average Azimuth: Aavg = (A1 + A2) ÷ 2

ΔN = ΔMD × sin(Iavg) × cos(Aavg)
ΔE = ΔMD × sin(Iavg) × sin(Aavg)
ΔTVD = ΔMD × cos(Iavg)
```

### Minimum Curvature Method (Industry Standard)
```
Ratio Factor (RF):
RF = (2 ÷ DL) × tan(DL ÷ 2)

Where DL = Dogleg angle in radians

ΔN = (ΔMD ÷ 2) × (sin(I1)×cos(A1) + sin(I2)×cos(A2)) × RF
ΔE = (ΔMD ÷ 2) × (sin(I1)×sin(A1) + sin(I2)×sin(A2)) × RF
ΔTVD = (ΔMD ÷ 2) × (cos(I1) + cos(I2)) × RF

When DL is very small, RF ≈ 1
```

## Dogleg Severity (DLS)

### Dogleg Calculation
```
cos(DL) = cos(I1)×cos(I2) + sin(I1)×sin(I2)×cos(A2-A1)

DL = arccos[cos(I1)×cos(I2) + sin(I1)×sin(I2)×cos(A2-A1)]
```

### Dogleg Severity (°/100 ft)
```
DLS = (DL × 100) ÷ ΔMD

Example:
DL = 2° over 95 ft course length
DLS = (2 × 100) ÷ 95 = 2.1°/100 ft
```

### Maximum Recommended DLS

| Application | Max DLS (°/100 ft) |
|------------|-------------------|
| Rotary drilling | 3-5 |
| Motor drilling | 8-15 |
| Production casing | 3-5 |
| Liner running | 5-8 |
| Logging tools | 10-15 |
| Coiled tubing | 15-20 |

## Build Rate and Turn Rate

### Build Rate
```
Build Rate (°/100 ft) = (I2 - I1) × 100 ÷ ΔMD

Example:
I1 = 15°, I2 = 18°, ΔMD = 90 ft
Build Rate = (18 - 15) × 100 ÷ 90 = 3.33°/100 ft
```

### Turn Rate
```
Turn Rate (°/100 ft) = (A2 - A1) × 100 ÷ ΔMD

Note: Account for azimuth crossing through 0°/360°
```

### Combined Build and Turn
```
DLS² ≈ Build Rate² + (Turn Rate × sin(Iavg))²

Approximate relationship for planning
```

## Build Radius and Arc Length

### Build Radius
```
R (ft) = 5729.58 ÷ Build Rate (°/100 ft)

or

R (ft) = 18000 ÷ (π × Build Rate)

Example:
Build Rate = 3°/100 ft
R = 5729.58 ÷ 3 = 1,910 ft
```

### Arc Length (to build to target inclination)
```
Arc Length (ft) = (Target Inc - Initial Inc) × 100 ÷ Build Rate

Example:
Build from 0° to 90° at 3°/100 ft
Arc Length = (90 - 0) × 100 ÷ 3 = 3,000 ft MD
```

## Horizontal Displacement

### Horizontal Departure (at any point)
```
Departure = √(North² + East²)

Direction = arctan(East ÷ North)
(Adjust quadrant based on signs)
```

### Closure Distance and Azimuth
```
Closure Distance = √((Target N - Actual N)² + (Target E - Actual E)²)

Closure Azimuth = arctan((Target E - Actual E) ÷ (Target N - Actual N))
```

### Section View Calculations
```
Vertical Section (VS) = Departure × cos(VS Azimuth - Well Azimuth)

VS shows progress toward target in 2D plane
```

## Toolface Calculations

### Toolface Orientation
```
Gravity Toolface (GTF): Used when I > 5°
Magnetic Toolface (MTF): Used when I < 5°

GTF: 0° = High side, 90° = Right, 180° = Low side, 270° = Left
MTF: Magnetic compass direction of tool face
```

### Required Toolface for Target Direction
```
For building angle: TF = 0° (high side)
For dropping angle: TF = 180° (low side)
For turning right: TF = 90°
For turning left: TF = 270°

Combined builds/turns require intermediate toolface angles
```

### Toolface to Achieve Direction Change
```
TF = arctan((Turn Rate × sin(I)) ÷ Build Rate)

Where rates are desired °/100 ft values
```

## Anti-Collision Calculations

### Separation Factor (SF)
```
SF = Center-to-Center Distance ÷ Combined Position Uncertainty

SF > 1.5 typically required for safe separation
```

### Traveling Cylinder (simple check)
```
Minimum Separation = Wellbore Radius 1 + Wellbore Radius 2 + Safety Margin

Typical safety margin: 50-100 ft depending on uncertainty
```

### Ellipse of Uncertainty (EOU)
```
Semi-major axis = Survey tool lateral error × MD
Semi-minor axis = Survey tool high-side error × MD

Survey uncertainty grows with depth
```

## Motor Yield Calculations

### Motor Bend Contribution
```
Theoretical Build Rate = (Bend Angle × 100) ÷ (Bit to Bend Distance)

Example:
1.5° bend, 3 ft bit to bend
Theoretical = (1.5 × 100) ÷ 3 = 50°/100 ft

Actual rate is typically 30-50% of theoretical due to:
- Hole enlargement
- BHA flex
- Formation effects
```

### Slide vs Rotate
```
Slide drilling: Full motor build rate
Rotate drilling: Reduced or no build rate
Combined: Use slide percentage to control build

Slide % = (Desired Build ÷ Slide-only Build) × 100
```

## Tortuosity

### Tortuosity Index
```
TI = Σ |DLS| × ΔMD ÷ 100

Lower TI = Smoother wellbore
Higher TI = More doglegs, more drag
```

### Accumulated DLS
```
Used to estimate total wellbore curvature for:
- Casing wear prediction
- Drill string fatigue
- Running tool selection
```

## Quick Reference Tables

### Common Survey Tool Accuracy

| Tool Type | Inclination | Azimuth |
|-----------|------------|---------|
| Single shot | ±0.25° | ±1.5° |
| MWD | ±0.1-0.2° | ±1.0-1.5° |
| Gyro (surface) | ±0.1° | ±0.5° |
| Gyro (memory) | ±0.1° | ±0.2° |

### Build Radius Quick Reference

| Build Rate | Radius (ft) |
|------------|-------------|
| 1°/100 ft | 5,730 |
| 2°/100 ft | 2,865 |
| 3°/100 ft | 1,910 |
| 4°/100 ft | 1,432 |
| 5°/100 ft | 1,146 |
| 6°/100 ft | 955 |
| 8°/100 ft | 716 |
| 10°/100 ft | 573 |
| 15°/100 ft | 382 |

---

*Survey calculations should be performed using validated software. Hand calculations are for verification and field estimates only.*
