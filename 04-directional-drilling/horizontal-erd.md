# Horizontal & Extended Reach Drilling

## Overview

Horizontal and Extended Reach Drilling (ERD) represent advanced directional drilling techniques requiring careful planning and execution. These wells maximize reservoir exposure but present unique operational challenges.

---

## Horizontal Well Profiles

### Standard Horizontal Well Geometry

```
Surface
   │
   │ Vertical Section
   │
KOP├───────╮
   │        ╲
   │         ╲  Build Section (Curve)
   │          ╲
   │           ╲
Landing────────┼───────────────────────────────────────
Point          │            Lateral Section
               │     (Horizontal, typically 88-92°)
               │
               └─────────────────────────────────────── TD
```

### Well Profile Parameters

| Parameter | Typical Range | Notes |
|-----------|---------------|-------|
| **Vertical section** | 1,000 - 5,000 ft | Above KOP |
| **Build rate** | 6 - 12°/100 ft | Curve section |
| **Landing inclination** | 88° - 92° | "Horizontal" |
| **Lateral length** | 5,000 - 15,000+ ft | Unconventional |
| **Total MD** | 10,000 - 25,000+ ft | Varies greatly |

### Curve Types

| Curve Type | Build Rate | Curve Length | Application |
|------------|------------|--------------|-------------|
| **Long radius** | 2-6°/100 ft | 1,500-4,500 ft | Conventional, casing-friendly |
| **Medium radius** | 6-20°/100 ft | 450-1,500 ft | Most horizontal wells |
| **Short radius** | 20-50°/100 ft | 180-450 ft | Re-entries, tight targets |
| **Ultra-short** | 50-150°/100 ft | 60-180 ft | Coiled tubing, special applications |

---

## Extended Reach Drilling (ERD)

### ERD Classification

| Category | HD:TVD Ratio | Departure | Challenges |
|----------|--------------|-----------|------------|
| **Standard** | < 2:1 | < 2× TVD | Conventional techniques |
| **Extended reach** | 2:1 - 3:1 | 2-3× TVD | T&D, hole cleaning |
| **Severe ERD** | > 3:1 | > 3× TVD | All challenges critical |
| **World class** | > 5:1 | > 5× TVD | Extreme, few wells |

### ERD World Records (Approximate)

| Record | Value | Operator/Location |
|--------|-------|-------------------|
| **Longest MD** | ~50,000 ft | Various |
| **Longest departure** | ~45,000 ft | Sakhalin |
| **Highest ratio** | ~7:1 | Various |

### ERD Limiting Factors

```
┌─────────────────────────────────────────────────────────────┐
│                    ERD LIMITING FACTORS                     │
├─────────────────────────────────────────────────────────────┤
│                                                             │
│   ┌───────────────┐                                         │
│   │    TORQUE     │                                         │
│   │   (Rotating)  │ → Top drive limit, drill pipe limit    │
│   └───────┬───────┘                                         │
│           │                                                 │
│   ┌───────▼───────┐                                         │
│   │     DRAG      │                                         │
│   │  (Tripping)   │ → Hook load, pipe buckling             │
│   └───────┬───────┘                                         │
│           │                                                 │
│   ┌───────▼───────┐                                         │
│   │  HOLE CLEANING│                                         │
│   │               │ → Cuttings transport, pack-offs        │
│   └───────┬───────┘                                         │
│           │                                                 │
│   ┌───────▼───────┐                                         │
│   │      ECD      │                                         │
│   │               │ → Fracturing weak zones                │
│   └───────┬───────┘                                         │
│           │                                                 │
│   ┌───────▼───────┐                                         │
│   │  CASING WEAR  │                                         │
│   │               │ → Casing integrity                     │
│   └───────────────┘                                         │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

---

## Curve (Build Section) Drilling

### Curve Drilling Challenges

| Challenge | Cause | Mitigation |
|-----------|-------|------------|
| **Tortuosity** | Slide/rotate transitions | Minimize slides, RSS |
| **Ledges** | Hard/soft interbeds | Controlled parameters, ream |
| **Steering difficulty** | Formation effects | Adjust BHA, parameters |
| **Hole cleaning** | High angle, low velocity | Rotation, sweeps, flow rate |
| **Casing running** | Dogleg severity | Stay within DLS limits |

### Curve Drilling Best Practices

1. **Maintain consistent build rate** - Avoid sharp doglegs
2. **Rotate as much as possible** - Minimize sliding
3. **Ream curve section** - Clean hole, reduce tortuosity
4. **Monitor T&D** - Verify hole condition
5. **Plan casing running** - Consider curve tortuosity

### DLS Limits for Casing

| Casing Size | Maximum DLS | Notes |
|-------------|-------------|-------|
| 9-5/8" | 3-4°/100 ft | Surface/intermediate |
| 7" | 6-8°/100 ft | Production casing |
| 5-1/2" | 10-12°/100 ft | Production liner |
| 4-1/2" | 12-15°/100 ft | Liner/tieback |

---

## Lateral Section Drilling

### Lateral Drilling Challenges

| Challenge | Description | Impact |
|-----------|-------------|--------|
| **Hole cleaning** | Cuttings settle to low side | Pack-offs, stuck pipe |
| **Weight transfer** | Friction prevents WOB | Low ROP, sliding difficulty |
| **Wellbore stability** | Shale swelling, breakouts | Tight hole, cavings |
| **Torque** | Long drillstring | Top drive limits |
| **Drag** | Tripping friction | Tripping time, stuck risk |

### Hole Cleaning in Laterals

**Cuttings Bed Formation**:
```
                    Rotation Direction
                          ↓
       ┌─────────────────────────────────────┐
       │░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░│ ← Flow
       │░░░░░░░░░░  MUD CHANNEL  ░░░░░░░░░░░│
       │░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░│
       ├═══════════════════════════════════│ ← Drill Pipe
       │▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓│
       │▓▓▓▓▓▓▓▓  CUTTINGS BED  ▓▓▓▓▓▓▓▓▓▓▓│ ← Low Side
       └─────────────────────────────────────┘

Key: ░ = Mud  ▓ = Cuttings  ═ = Drill Pipe
```

**Hole Cleaning Guidelines**:

| Parameter | Guideline |
|-----------|-----------|
| **Flow rate** | Maximum practical (annular velocity > 120 ft/min) |
| **Rotation** | > 120-150 RPM when possible |
| **ROP control** | Match ROP to hole cleaning capacity |
| **Sweeps** | High-viscosity sweeps every 500-1,000 ft |
| **Short trips** | Wiper trips to shoe periodically |
| **Backreaming** | Ream out of hole, rotate/pump in |

### Annular Velocity Requirements

| Hole Size | Minimum Annular Velocity |
|-----------|-------------------------|
| 12-1/4" | 100-120 ft/min |
| 8-3/4" | 120-140 ft/min |
| 8-1/2" | 120-140 ft/min |
| 6-1/8" | 140-160 ft/min |

---

## Torque and Drag Management

### Torque Reduction Strategies

| Strategy | Application |
|----------|-------------|
| **Mud lubricity** | Add lubricants (oil, synthetic) |
| **Reduce WOB** | If torque-limited, back off weight |
| **Torque reducers** | Roller reamers, non-rotating stabilizers |
| **Trajectory optimization** | Minimize doglegs |
| **Wellbore quality** | Smooth hole, minimize ledges |

### Drag Reduction Strategies

| Strategy | Application |
|----------|-------------|
| **Roller reamers** | Reduce friction while tripping |
| **Float equipment** | Reduce surge pressures |
| **Pipe rotation** | Rotate while tripping where possible |
| **Mud properties** | Lubricants, appropriate weight |
| **Drill pipe friction** | Hardbanding, protectors |

### Buckling Prevention

**Sinusoidal Buckling**: First stage - pipe snakes along low side
**Helical Buckling**: Severe - pipe forms helix, can lock up

**Critical Buckling Load**:
```
Fc = 2 × √(E × I × w × sin(θ) / r)

Where:
Fc = Critical buckling force (lb)
E = Modulus of elasticity (psi)
I = Moment of inertia (in⁴)
w = Buoyed weight per unit length (lb/ft)
θ = Inclination (degrees)
r = Radial clearance (in)
```

**Prevention**:
- Use HWDP above compression zone
- Limit compression on drill pipe
- Consider drill pipe size/weight upgrades
- Model buckling before drilling

---

## Casing and Cementing Considerations

### Running Casing in Horizontal Wells

| Challenge | Mitigation |
|-----------|------------|
| **Drag** | Float equipment, rotation, lubricity |
| **Buckling** | Limit running speed, centralization |
| **Hole condition** | Condition hole before running |
| **Surge pressures** | Slow running speed, auto-fill |
| **Not reaching TD** | Float equipment, rotation, reciprocation |

### Casing Running Best Practices

1. **Condition hole** - Circulate clean, short trip
2. **Stage centralizers** - 1 per joint in curve, every 2-3 in lateral
3. **Use float equipment** - Reduce drag
4. **Monitor weights** - Watch for overpull/slack-off
5. **Rotate if possible** - Reduces friction significantly
6. **Control speed** - Avoid surge/swab issues

### Cementing Horizontal Sections

| Challenge | Solution |
|-----------|----------|
| **Free water** | Zero free-water cement |
| **Channeling** | Proper mud removal, spacers |
| **Centralization** | Adequate centralizer placement |
| **Density control** | Match cement density to hole conditions |
| **Placement** | Inner string, liner rotation |

---

## Drilling Fluids for Horizontal/ERD

### Mud Properties Requirements

| Property | Horizontal Well Requirement |
|----------|----------------------------|
| **Rheology** | Low PV, high YP (flat gels) |
| **Lubricity** | Coefficient of friction < 0.2 |
| **Inhibition** | Strong for shale stability |
| **Solids** | Minimum (<5% LGS) |
| **Density** | Minimum for well control |
| **Gel strength** | Flat (10 sec ≈ 10 min) |

### Sweep Types

| Sweep Type | Purpose | Volume |
|------------|---------|--------|
| **High-vis** | Lift cuttings bed | 25-50 bbl |
| **Tandem** | Hi-vis + weighted | 25+25 bbl |
| **Weighted** | Clean heavy cuttings | 25-50 bbl |
| **Wiper** | Condition hole | 50-100 bbl |

---

## Monitoring and Troubleshooting

### Key Indicators

| Indicator | Normal | Warning | Action Required |
|-----------|--------|---------|-----------------|
| **Torque trend** | Stable | Increasing | Investigate cause |
| **Drag trend** | Stable | Increasing | Short trip, sweep |
| **ECD** | Stable | Increasing | Reduce ROP, clean hole |
| **Pump pressure** | Stable | Increasing | Check for pack-off |
| **Cuttings returns** | Consistent | Inconsistent | Clean hole, sweep |

### Stuck Pipe Prevention

| Prevention Measure | Application |
|--------------------|-------------|
| **Monitor trends** | Torque, drag, ECD |
| **Regular sweeps** | Every stand or per program |
| **Short trips** | Every 500-1,000 ft drilled |
| **Keep pipe moving** | Never stationary for long |
| **Wiper trips** | Before logging, casing |
| **Hole condition** | Backream out of hole |
