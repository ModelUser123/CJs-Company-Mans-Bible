# Horizontal Well Operations

## Well Profile Design

### Standard Horizontal Well Profile

```
SURFACE SECTION
├── Vertical or slightly deviated
├── Set surface casing
├── Protect freshwater
└── Cement to surface

HOLD SECTION (Optional)
├── Maintain vertical or low angle
├── Build rate: 0°
├── Allows for spacing adjustment
└── Length varies

BUILD SECTION (Curve)
├── KOP: Kick-off point
├── Build rate: 6-15°/100 ft typical
├── Target: 90° inclination
├── Length: 1,500-3,000 ft typical
├── Landing depth: Target zone TVD
└── Controls
    ├── Motor bend
    ├── Rotary steerable
    └── Geosteering

LATERAL SECTION
├── Maintain 88-92° inclination
├── Azimuth control critical
├── Stay in zone
├── Length: 5,000-15,000 ft
└── Target: Maximum reservoir contact
```

### Build Rate Selection

| Build Rate | Application | Motor Bend |
|------------|-------------|------------|
| 4-6°/100 ft | Large hole, conventional | 1.0-1.25° |
| 8-10°/100 ft | Standard curve | 1.5-2.0° |
| 12-15°/100 ft | Short radius | 2.0-3.0° |
| >15°/100 ft | Ultra short radius | Special tools |

### Curve Section Calculations

```
BUILD SECTION LENGTH
├── Formula: L = ΔI × 100 / BR
├── Where:
│   ├── L = Measured depth of curve (ft)
│   ├── ΔI = Inclination change (degrees)
│   └── BR = Build rate (°/100 ft)
└── Example:
    ├── ΔI = 90° (vertical to horizontal)
    ├── BR = 10°/100 ft
    └── L = 90 × 100 / 10 = 900 ft

BUILD RADIUS
├── Formula: R = 5730 / BR
├── Example:
│   ├── BR = 10°/100 ft
│   └── R = 5730 / 10 = 573 ft
└── Smaller radius = tighter curve = more DLS
```

## Drilling the Curve

### Motor BHA Design

```
CURVE BHA COMPONENTS
├── Bit
│   ├── PDC (most common)
│   ├── 5-7 blade
│   └── Aggressive gauge protection
├── Motor
│   ├── Positive displacement (PDM)
│   ├── 1.5-2.5° bend
│   ├── 5-7 lobes
│   └── Sized for flow rate
├── MWD/LWD
│   ├── Inclination
│   ├── Azimuth
│   ├── Gamma ray
│   └── Resistivity (optional)
├── Stabilizers
│   ├── Near-bit (adjustable)
│   ├── String stabilizer
│   └── Sized for build/drop control
└── Drill Collars / HWDP
    ├── Weight for WOB
    └── Transition to drill pipe
```

### Slide vs Rotate Drilling

```
SLIDING
├── No pipe rotation
├── Motor provides all rotation
├── Used to change direction
├── Challenges
│   ├── Hole cleaning
│   ├── Stick-slip
│   ├── Tortuosity
│   └── ROP reduction
└── Minimize slide percentage

ROTATING
├── Continuous pipe rotation
├── Motor provides additional RPM
├── Straighter hole
├── Better cleaning
└── Preferred for majority of curve

SLIDE PERCENTAGE
├── Target: <15% in curve
├── Excellent: <10%
├── High slides indicate
│   ├── Wrong motor bend
│   ├── Formation tendencies
│   └── Weight distribution issues
└── Track by depth/stand
```

## Lateral Drilling

### Geosteering

```
REAL-TIME MEASUREMENTS
├── Gamma Ray
│   ├── Zone identification
│   ├── Formation boundary
│   └── Stay in zone indication
├── Resistivity
│   ├── Fluid contact detection
│   ├── Zone confirmation
│   └── Approaching boundary warning
├── Neutron/Density
│   ├── Porosity
│   ├── Gas indication
│   └── Formation quality
└── Azimuthal Tools
    ├── Boundary detection
    ├── Distance to bed
    └── Look-ahead capability

GEOSTEERING DECISIONS
├── Target Window
│   ├── Zone thickness
│   ├── Optimal position
│   └── Tolerance band
├── Adjustments
│   ├── Build up (if dropping out)
│   ├── Drop down (if near top)
│   ├── Turn left/right (lateral adjustment)
│   └── Hold course
└── Communication
    ├── Real-time with geosteering team
    ├── Clear decision protocol
    └── Document all changes
```

### Lateral Drilling Optimization

```
ROP OPTIMIZATION
├── Weight on Bit: 15-30 klb typical
├── RPM: 100-200 (motor + rotation)
├── Flow Rate: Optimize for cleaning
├── Bit Selection: Formation specific
└── Monitor: ROP vs parameters

HOLE CLEANING
├── Critical in horizontal
├── Minimum AV: 150+ ft/min
├── Rotation: Essential for cleaning
├── Sweeps: High-vis pills regular
├── Wiper trips: As needed
└── Indicators
    ├── Torque increase
    ├── Pack-off tendency
    ├── ECD increase
    └── Cuttings at surface

TORTUOSITY CONTROL
├── Target DLS: <3°/100 ft
├── Minimize slides
├── Use RSS when possible
├── Smooth motor transitions
└── Impact
    ├── Casing/liner running
    ├── Completion tools
    ├── Production string
    └── Future intervention
```

## Casing and Liner

### Lateral Casing Options

| Option | Advantages | Disadvantages |
|--------|-----------|---------------|
| Production casing | Full wellbore access | Higher cost |
| Cemented liner | Zone isolation | Limited access |
| Uncemented liner | Open hole completion | Less isolation |
| Open hole | Maximum contact | No isolation |

### Liner Running in Horizontal

```
CHALLENGES
├── Weight/drag in horizontal
├── Rotation limitations
├── Centralization
├── Cement placement
└── Shoe track filling

SOLUTIONS
├── Liner Flotation
│   ├── Fill shoe track with lighter fluid
│   ├── Close float, run in empty
│   └── Reduces drag significantly
├── Centralizers
│   ├── Solid body type
│   ├── Every joint or alternate
│   └── Proper standoff for cement
├── Rotation/Reciprocation
│   ├── Keep moving during run
│   ├── Work through tight spots
│   └── Prevent sticking
└── Top Drive
    ├── Continuous rotation capability
    ├── Better weight control
    └── Preferred for horizontal
```

### Cement Design for Horizontal

```
HORIZONTAL CEMENT CHALLENGES
├── Gravity segregation
├── Free water settling
├── Channel on low side
└── Long placement times

SOLUTIONS
├── Zero free water cement
├── Spacer design for displacement
├── Centralizer placement
├── Rotation during cement
├── Staged cementing if needed
└── Competent tail cement

VERIFICATION
├── CBL/VDL logs (if possible)
├── Cement volume returns
├── Pressure test
└── Isolation during completion
```

## Torque and Drag Management

### Friction Factors

| Section | Cased (typical) | Open Hole (typical) |
|---------|----------------|-------------------|
| Vertical | 0.15-0.25 | 0.20-0.35 |
| Curve | 0.20-0.30 | 0.25-0.40 |
| Lateral | 0.20-0.30 | 0.25-0.45 |

### Torque and Drag Reduction

```
OPERATIONAL
├── Minimize doglegs (smooth wellpath)
├── Maintain good hole condition
├── Proper mud lubricity
├── Rotation vs sliding ratio
└── Reduce unnecessary trips

TOOLS AND TECHNOLOGY
├── Non-rotating protectors (NRPs)
├── Friction reducing tools
├── Bearing subs
├── Roller reamers
└── Torque reduction sleeves

MUD SYSTEM
├── Lubricants (2-5% addition)
├── Oil-based mud (lower friction)
├── Adequate weight (hole stability)
└── Good filter cake (reduce sticking)
```

## Common Problems and Solutions

| Problem | Cause | Solution |
|---------|-------|----------|
| Can't build angle | Wrong motor, formation | Increase bend, adjust WOB |
| Over-building | Motor too aggressive | Reduce bend, add stabilizer |
| Dropping out of zone | Formation dip | Build up, adjust TVD target |
| High torque | Poor hole, DLS | Ream, improve mud |
| Stuck pipe | Pack-off, differential | Clean hole, spot pill |
| Low ROP | Bit wear, wrong parameters | Change bit, optimize parameters |
| Can't reach TD | Torque/drag limit | T&D tools, lubricity |

---

*Horizontal well drilling requires careful planning and real-time decision making. Maintain close communication with directional and geosteering teams.*
