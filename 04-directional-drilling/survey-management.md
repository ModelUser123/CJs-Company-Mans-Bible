# Survey Management

## Overview

Survey management ensures accurate wellbore position knowledge throughout drilling operations. Accurate surveys are critical for target accuracy, anti-collision, and regulatory compliance.

---

## Survey Tool Types

### Magnetic Tools

| Tool Type | Accuracy (Inc/Azi) | Application |
|-----------|-------------------|-------------|
| **Single-shot** | ±0.25° / ±1.0° | Backup, verification |
| **Multi-shot** | ±0.25° / ±1.0° | Trip surveys, historic wells |
| **MWD** | ±0.1° / ±0.5° | Real-time while drilling |
| **Magnetic steering** | ±0.1° / ±0.25° | High-accuracy drilling |

**Magnetic Tool Limitations**:
- Affected by magnetic interference (casing, drill collars, hot spots)
- Requires correction for declination and dip
- Accuracy degrades near magnetic poles
- Cannot survey inside casing

### Gyroscopic Tools

| Tool Type | Accuracy (Inc/Azi) | Application |
|-----------|-------------------|-------------|
| **Rate gyro** | ±0.1° / ±0.5° | In-casing surveys, tie-ins |
| **North-seeking gyro** | ±0.1° / ±0.2° | High-accuracy, anti-collision |
| **Inertial gyro** | ±0.02° / ±0.05° | Ultra-high accuracy, relief wells |
| **Continuous gyro** | ±0.05° / ±0.1° | Continuous in-hole surveys |

**Gyro Advantages**:
- Not affected by magnetic interference
- Can survey in casing
- Higher accuracy for azimuth
- Required for anti-collision critical wells

### MWD Survey Systems

**Components**:
```
┌─────────────────────────────────────────────────────┐
│                    MWD TOOL STRING                  │
├─────────────────────────────────────────────────────┤
│  ┌─────────────┐                                    │
│  │ Power       │ → Battery or turbine powered      │
│  │ Section     │                                    │
│  └──────┬──────┘                                    │
│         │                                           │
│  ┌──────▼──────┐                                    │
│  │ Directional │ → Accelerometers & Magnetometers  │
│  │ Sensors     │   (Tri-axial)                     │
│  └──────┬──────┘                                    │
│         │                                           │
│  ┌──────▼──────┐                                    │
│  │ Telemetry   │ → Mud pulse or EM transmission    │
│  │ System      │                                    │
│  └─────────────┘                                    │
└─────────────────────────────────────────────────────┘
```

---

## Survey Calculations

### Minimum Curvature Method

The industry standard for calculating wellbore position between survey stations.

**Calculation Steps**:

1. **Calculate Ratio Factor (RF)**:
```
RF = (2/DL) × tan(DL/2)

Where DL = Dogleg angle between surveys
DL = cos⁻¹[cos(I₂-I₁) - sin(I₁)×sin(I₂)×(1-cos(A₂-A₁))]
```

2. **Calculate Position Changes**:
```
ΔN = (ΔMD/2) × (sin(I₁)×cos(A₁) + sin(I₂)×cos(A₂)) × RF
ΔE = (ΔMD/2) × (sin(I₁)×sin(A₁) + sin(I₂)×sin(A₂)) × RF
ΔTVD = (ΔMD/2) × (cos(I₁) + cos(I₂)) × RF
```

3. **Calculate Dogleg Severity**:
```
DLS (°/100 ft) = DL × (100/ΔMD)
```

### Survey Calculation Example

| Station | MD (ft) | Inc (°) | Azi (°) |
|---------|---------|---------|---------|
| 1 | 5000 | 25.0 | 135.0 |
| 2 | 5093 | 28.5 | 138.0 |

**Solution**:
- ΔMD = 93 ft
- DL = 3.69° (dogleg angle)
- RF = 0.9997
- ΔN = -38.2 ft
- ΔE = +38.9 ft
- ΔTVD = 81.6 ft
- DLS = 3.97°/100 ft

---

## Survey Quality Control

### Pre-Survey Checks

| Check | Requirement |
|-------|-------------|
| Tool calibration | Current calibration certificate |
| Battery status | Sufficient for planned depth |
| Sensor check | All sensors responding |
| Reference check | Surface readings correct |
| Temperature rating | Tool rated for expected BHT |

### Survey Station Requirements

| Parameter | Requirement |
|-----------|-------------|
| **Station interval** | Max 93 ft (28 m) or per company policy |
| **Static conditions** | Pumps off, no pipe movement |
| **Duration** | Minimum 30-60 seconds stationary |
| **Depth accuracy** | Verify depth with driller's depth |
| **Multiple readings** | Minimum 2 readings per station |

### Quality Indicators

| QC Check | Acceptance Criteria |
|----------|---------------------|
| **G-total** | 0.997 - 1.003 G (±0.003) |
| **B-total** | Within ±200 nT of reference |
| **Dip angle** | Within ±0.3° of reference |
| **Repeat surveys** | Within ±0.1° Inc, ±0.5° Azi |
| **Accelerometer match** | Three axes consistent |
| **Magnetometer match** | Three axes consistent |

### Survey Rejection Criteria

Reject survey if:
- [ ] G-total outside 0.997-1.003
- [ ] B-total deviation >350 nT
- [ ] Dip angle deviation >0.5°
- [ ] Repeat readings don't match
- [ ] Obvious magnetic interference
- [ ] Tool in motion during survey

---

## Magnetic Corrections

### Declination

**Definition**: Angular difference between magnetic north and true north

**Correction**:
```
True Azimuth = Magnetic Azimuth + Declination

East declination: Add to magnetic azimuth
West declination: Subtract from magnetic azimuth
```

**Sources**:
- NOAA Magnetic Declination Calculator
- BGGM (British Geological Survey Global Model)
- IGRF (International Geomagnetic Reference Field)
- IFR (In-Field Referencing) from local measurements

### Magnetic Dip

**Definition**: Angle of magnetic field lines from horizontal

| Latitude | Approximate Dip |
|----------|-----------------|
| 0° (Equator) | 0° |
| 30° | 45° |
| 45° | 60° |
| 60° | 75° |
| 70°+ | 80°+ |

### Grid Corrections

| Correction | Definition | When Required |
|------------|------------|---------------|
| **Grid convergence** | Angle between grid north and true north | All surveys if reporting to grid |
| **Meridian convergence** | Correction for earth curvature | Long step-outs, ERD |
| **Scale factor** | Grid distance vs. true distance | Position calculations |

### In-Field Referencing (IFR)

**Purpose**: Improve magnetic reference accuracy using local measurements

**Method**:
1. Take readings at surface (known position)
2. Calculate local magnetic field values
3. Use local values instead of global model
4. Reduces systematic errors

---

## Ellipse of Uncertainty

### Error Sources

| Error Type | Source | Impact |
|------------|--------|--------|
| **Sensor errors** | Tool accuracy limits | All surveys |
| **Depth errors** | Drill pipe measurement | Depth uncertainty |
| **Magnetic errors** | Declination, drillstring magnetism | Azimuth uncertainty |
| **Processing errors** | Calculation methods | Position uncertainty |

### Error Models

| Model | Description | Application |
|-------|-------------|-------------|
| **ISCWSA** | Industry standard error model | Standard operations |
| **Operator-specific** | Company-defined parameters | Where approved |
| **Enhanced** | Includes additional error terms | High-accuracy wells |

### Ellipse Parameters

```
                    ┌─────────────────────┐
                    │                     │
               Semi-major axis (A)        │
                    ├─────────┤           │
                    │    ╭────────╮       │
                    │   ╱          ╲      │ Semi-minor
                    │  ╱            ╲     │ axis (B)
                    │ ╱   Survey     ╲    │
                    │╱    Position    ╲   │
                    │╲    (center)    ╱   ├─────────┤
                    │ ╲              ╱    │
                    │  ╲            ╱     │
                    │   ╲          ╱      │
                    │    ╰────────╯       │
                    │                     │
                    └─────────────────────┘

Orientation defined by azimuth of semi-major axis
```

### Uncertainty Growth

| Survey Type | Typical Uncertainty at 10,000 ft MD |
|-------------|-------------------------------------|
| MWD standard | ±75-100 ft lateral, ±25 ft vertical |
| MWD with IFR | ±50-75 ft lateral, ±20 ft vertical |
| Gyro | ±25-40 ft lateral, ±15 ft vertical |

---

## Survey Frequency Requirements

### Standard Requirements

| Situation | Survey Frequency |
|-----------|------------------|
| **Vertical section** | Every 500 ft minimum |
| **Building angle** | Every stand (93 ft) or less |
| **Tangent section** | Every 500 ft minimum |
| **Near offset wells** | Every 93 ft or less |
| **Approaching target** | Every 93 ft minimum |
| **In lateral** | Every 93 ft for geosteering |

### Anti-Collision Survey Requirements

| Separation Factor | Survey Frequency |
|-------------------|------------------|
| SF > 1.5 | Standard frequency |
| SF = 1.0 - 1.5 | Every stand (93 ft) |
| SF = 0.5 - 1.0 | Every 45 ft |
| SF < 0.5 | Continuous or stop drilling |

---

## Survey Documentation

### Survey Report Contents

| Element | Details |
|---------|---------|
| **Header** | Well name, date, depth, tool type |
| **Raw data** | Measured Inc, Azi, gravity, magnetic readings |
| **QC data** | G-total, B-total, dip, repeatability |
| **Corrections** | Declination, grid convergence applied |
| **Calculated position** | MD, Inc, Azi, TVD, NS, EW, VS |
| **DLS** | Dogleg severity |
| **Comments** | Any anomalies or issues |

### Definitive Survey Requirements

| Requirement | Purpose |
|-------------|---------|
| **Final survey** | Gyro or validated MWD after TD |
| **Tie-in survey** | Surface location verification |
| **As-drilled trajectory** | Complete station listing |
| **Error model** | Uncertainty documentation |
| **Regulatory submission** | Meet state/federal requirements |

---

## Troubleshooting

### Common Survey Problems

| Problem | Cause | Solution |
|---------|-------|----------|
| **Azimuth jumping** | Magnetic interference | Increase NMDC length, check drillstring |
| **High G-total** | Vibration, tool movement | Resurvey with pipe stationary |
| **Low B-total** | Magnetic dead zone | Use gyro or adjust BHA |
| **Inconsistent dip** | Local magnetic anomaly | Apply IFR, increase NMDC |
| **Survey won't transmit** | Telemetry issue | Check mud properties, tool function |

### Magnetic Interference Solutions

| Interference Type | Solution |
|-------------------|----------|
| **Drillstring magnetism** | Degauss, add NMDC length |
| **Casing shoe** | Increase distance, use gyro near shoe |
| **Hot spots** | Identify and isolate magnetic components |
| **Formation magnetism** | Use IFR or gyro |

### Non-Magnetic Drill Collar (NMDC) Requirements

| Inclination | Minimum NMDC Length |
|-------------|---------------------|
| 0-5° | 31 ft (1 collar) |
| 5-15° | 62 ft (2 collars) |
| 15-45° | 31 ft (1 collar) |
| 45-90° | 31 ft (1 collar) |

**Note**: Increase NMDC length near casing shoes, in highly deviated sections, or when interference is detected.
