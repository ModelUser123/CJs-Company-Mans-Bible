# Directional Planning

## Overview

Directional planning is the process of designing a well trajectory from surface to target. A well-designed directional plan optimizes drilling efficiency while ensuring the wellbore reaches the intended target within tolerance.

---

## Well Trajectory Types

### Build and Hold (J-Curve)
```
Surface ─────────┐
                 │ Vertical
                 │
           KOP → ├─────╮
                 │      ╲ Build Section
                 │       ╲
                 │        ├────────────────────────
                 │        │    Hold Section (Tangent)
                 │        │
                 └────────┴──────────────────────── Target
```
- **Application**: Horizontal wells, shallow targets with offset
- **Advantages**: Simple, minimal dogleg, good for laterals
- **Considerations**: Higher TVD at target than vertical

### S-Curve (Build-Hold-Drop)
```
Surface ─────────┐
                 │ Vertical
                 │
           KOP → ├─────╮
                 │      ╲ Build
                 │       ├────────────┐
                 │       │    Hold    │
                 │       ├────────────┘
                 │      ╱ Drop
                 │     ╱
                 └────┴── Target (near vertical entry)
```
- **Application**: Deep targets requiring near-vertical entry
- **Advantages**: Vertical wellbore at target, easier completion
- **Considerations**: More complex, higher torque and drag

### Modified S-Curve
- Hold section at lower inclination than standard S
- Drop to vertical or near-vertical at target
- Used when S-curve dogleg would be too severe

### Extended Reach Drilling (ERD)
```
Surface ─────────┐
                 │
           KOP → ├─────────────────────────────────────────────
                 │                Very Long Tangent
                 │         TVD:HD ratio > 1:2
                 └─────────────────────────────────────────────
```
- **Definition**: Step-out ratio (HD:TVD) > 2:1
- **Challenges**: Hole cleaning, torque, ECD, casing wear
- **Limits**: Typically 40,000-50,000 ft MD achievable

---

## Key Planning Parameters

### Kickoff Point (KOP)

| Factor | Consideration |
|--------|---------------|
| **Formation stability** | Avoid kicking off in unstable zones |
| **Casing setting depth** | Typically after surface casing |
| **Build rate capability** | Formation must support planned BUR |
| **Target geometry** | Determines required departure |
| **Anti-collision** | Clear of offset wells at KOP |

**Typical KOP Depths**:
- Surface casing shoe + 100-300 ft
- Below unstable formations
- In competent shale or limestone

### Build Rate (BUR)

| Classification | Build Rate | Application |
|----------------|------------|-------------|
| **Low** | 1-3°/100 ft | Deep wells, casing wear concerns |
| **Medium** | 3-6°/100 ft | Standard directional wells |
| **High** | 6-10°/100 ft | Short radius, tight targets |
| **Ultra-high** | 10-20°/100 ft | Short radius horizontal |

**Build Rate Calculation**:
```
BUR (°/100 ft) = (Inclination Change) / (Measured Depth Change) × 100

Example: Build from 0° to 30° over 500 ft
BUR = (30 - 0) / 500 × 100 = 6°/100 ft
```

### Turn Rate

| Parameter | Description |
|-----------|-------------|
| **Turn rate** | Azimuth change per 100 ft (°/100 ft) |
| **Walk** | Natural tendency of BHA to turn |
| **Right-hand walk** | Common with standard rotation |
| **Left-hand walk** | Some formations, certain BHAs |

**Turn Rate Considerations**:
- Plan for walk tendency in tangent sections
- Account for magnetic declination changes
- Consider formation dip effects

### Dogleg Severity (DLS)

**Definition**: Total curvature rate combining build and turn

**DLS Calculation**:
```
DLS = √(BUR² + (TR × sin(I))²)

Where:
- BUR = Build rate (°/100 ft)
- TR = Turn rate (°/100 ft)
- I = Inclination (degrees)
```

**DLS Limits**:

| Casing Size | Maximum DLS |
|-------------|-------------|
| 9-5/8" | 3-4°/100 ft |
| 7" | 6-8°/100 ft |
| 5-1/2" | 10-12°/100 ft |
| 4-1/2" | 15-18°/100 ft |

**DLS Effects**:
- Casing wear
- Key seating
- Fatigue failures
- Running/cementing difficulties
- Logging tool sticking

---

## Target Definition

### Target Types

| Type | Description | Tolerance |
|------|-------------|-----------|
| **Point target** | Single coordinate | Radius from point |
| **Line target** | Two endpoints | Distance from line |
| **Box target** | Rectangular area | Within box boundaries |
| **Ellipse target** | Oval area | Semi-major/minor axes |

### Landing Zone Parameters

| Parameter | Definition |
|-----------|------------|
| **Landing point** | Where wellbore reaches target inclination |
| **Landing azimuth** | Direction at landing |
| **Landing inclination** | Angle at landing (typically 88-92° for horizontal) |
| **TVD tolerance** | Allowable TVD variance (± X ft) |
| **Azimuth tolerance** | Allowable direction variance (± X°) |

### Target Sizing Factors

1. **Geological uncertainty** - Structure, dip, faulting
2. **Survey accuracy** - Ellipse of uncertainty
3. **Drilling capability** - Steering precision
4. **Wellbore position accuracy** - Cumulative survey error
5. **Business requirements** - Reservoir contact needed

---

## Anti-Collision Planning

### Separation Criteria

| Separation Factor (SF) | Status | Action |
|-----------------------|--------|--------|
| SF > 1.5 | Normal | Continue drilling |
| SF = 1.0 - 1.5 | Watch | Increase survey frequency |
| SF = 0.5 - 1.0 | Alert | Consider trajectory change |
| SF < 0.5 | Stop | Halt drilling, evaluate |

**Separation Factor Calculation**:
```
SF = Actual Center-to-Center Distance / Combined Ellipse of Uncertainty
```

### Offset Well Data Requirements

| Data | Purpose |
|------|---------|
| **Survey data** | Position of offset wellbores |
| **Survey tool type** | Accuracy assumptions |
| **Casing depths** | Protected intervals |
| **Total depth** | Full wellbore length |
| **Current status** | Active, P&A, injection, etc. |

### Anti-Collision Scan Parameters

| Parameter | Typical Setting |
|-----------|-----------------|
| **Scan radius** | 200-500 ft from planned path |
| **Alert threshold** | 75-100 ft separation |
| **Critical threshold** | 25-50 ft separation |
| **Survey frequency** | Every 90 ft or less in close proximity |

---

## Torque and Drag Analysis

### Pre-Drill Analysis

| Calculation | Purpose |
|-------------|---------|
| **Hook load** | Verify rig capacity |
| **Surface torque** | Verify top drive capacity |
| **Buckling analysis** | Identify buckling depths |
| **Casing wear** | Predict wear locations/severity |

### Friction Factors

| Condition | Cased Hole | Open Hole |
|-----------|------------|-----------|
| **Rotating** | 0.20-0.25 | 0.25-0.35 |
| **Sliding** | 0.25-0.35 | 0.35-0.45 |
| **Tripping** | 0.25-0.35 | 0.30-0.40 |

### Drag Reduction Strategies

1. **Wellbore trajectory** - Minimize dogleg severity
2. **Mud lubricity** - Add lubricants
3. **Drill pipe** - Hardbanding, protectors
4. **Rotation** - Rotate while tripping where possible
5. **Hole cleaning** - Remove cuttings bed

---

## Directional Proposal Contents

### Required Elements

| Section | Contents |
|---------|----------|
| **Objective** | Target coordinates, TVD, tolerance |
| **Well path** | KOP, build rates, inclination, azimuth |
| **Survey program** | Tool type, frequency, QC requirements |
| **BHA proposals** | Motor specs, stabilizers, MWD |
| **Anti-collision** | Offset well analysis, separation factors |
| **Torque/Drag** | Analysis results, limits |
| **Risk assessment** | Technical risks and mitigations |
| **Contingencies** | Alternative plans if problems encountered |

### Trajectory Table Format

| MD (ft) | Inc (°) | Azi (°) | TVD (ft) | NS (ft) | EW (ft) | VS (ft) | DLS (°/100ft) |
|---------|---------|---------|----------|---------|---------|---------|---------------|
| 0 | 0.00 | 0.00 | 0 | 0 | 0 | 0 | 0.00 |
| 2000 | 0.00 | 0.00 | 2000 | 0 | 0 | 0 | 0.00 |
| 2500 | 15.00 | 135.00 | 2485 | -53 | 53 | 75 | 3.00 |
| 3000 | 30.00 | 135.00 | 2942 | -176 | 176 | 249 | 3.00 |
| ... | ... | ... | ... | ... | ... | ... | ... |

---

## Planning Checklist

### Pre-Planning
- [ ] Obtain target coordinates and tolerance
- [ ] Gather offset well survey data
- [ ] Review geological prognosis
- [ ] Identify casing setting depths
- [ ] Determine rig capabilities

### Trajectory Design
- [ ] Select well profile type
- [ ] Determine KOP depth
- [ ] Calculate build/turn rates
- [ ] Verify DLS within limits
- [ ] Check anti-collision clearances

### Analysis
- [ ] Run torque and drag model
- [ ] Perform hydraulics analysis
- [ ] Calculate casing wear predictions
- [ ] Model buckling potential
- [ ] Verify hole cleaning capability

### Documentation
- [ ] Create trajectory tables
- [ ] Prepare survey program
- [ ] Document BHA recommendations
- [ ] Compile contingency plans
- [ ] Review and approve plan

---

## Common Planning Mistakes

| Mistake | Consequence | Prevention |
|---------|-------------|------------|
| Insufficient target tolerance | Excessive correction runs | Realistic uncertainty analysis |
| Ignoring formation walk | Miss target azimuth | Plan for walk, adjust BHA |
| Aggressive build rates | Hole problems, tool failures | Match BUR to formation/tools |
| Poor KOP selection | Unstable hole, steering difficulty | Consider formation properties |
| Inadequate T&D analysis | Stuck pipe, inability to reach TD | Full analysis with realistic friction |
