# BOP Equipment Specifications

## Ram Type Preventers

### Ram Preventer Pressure Ratings

| API Rating | Working Pressure (psi) | Test Pressure (psi) |
|------------|----------------------|---------------------|
| 2M | 2,000 | 3,000 |
| 3M | 3,000 | 4,500 |
| 5M | 5,000 | 7,500 |
| 10M | 10,000 | 15,000 |
| 15M | 15,000 | 22,500 |
| 20M | 20,000 | 30,000 |

### Ram Preventer Bore Sizes

| Bore (in) | Common Applications |
|-----------|-------------------|
| 7-1/16 | Workover, shallow wells |
| 9 | Light duty land rigs |
| 11 | Standard land drilling |
| 13-5/8 | Standard offshore, deep land |
| 16-3/4 | Deepwater, high pressure |
| 18-3/4 | Ultra-deepwater, HPHT |
| 21-1/4 | Large bore operations |

### Ram Types and Applications

```
PIPE RAMS
├── Fixed Size
│   ├── Sized for specific pipe OD
│   ├── Best seal quality
│   └── Must match pipe in hole
├── Variable Bore
│   ├── Adjustable for range of sizes
│   ├── Reduced seal quality
│   └── 2-3" size range typical
└── Specifications
    ├── Pipe OD tolerance: ±1/16"
    └── Seal: Rubber or urethane

BLIND RAMS
├── Purpose: Close on open hole
├── Application: No pipe in hole
└── Seal: Full metal-to-metal + elastomer

SHEAR RAMS
├── Purpose: Cut drill pipe
├── Capacity: Cut grade and size specific
├── Shearing Pressure Formula:
│   P = (A × UTS × SF) / Ram Area
└── Types
    ├── Standard (DP only)
    ├── Super Shear (DC capable)
    └── Casing Shear (casing capable)

BLIND SHEAR RAMS (BSR)
├── Combined shear and seal
├── Critical for deepwater
├── Must seal after cutting
└── Rated for specific pipe grades

CASING SHEAR RAMS
├── Cut and seal on casing
├── Ultra-high pressure required
├── Specialized applications
└── Subsea stacks primarily
```

### Ram Preventer Specifications Table

| Manufacturer | Model | Bore | WP (psi) | Rams | Height (in) |
|-------------|-------|------|----------|------|-------------|
| Cameron | U | 11" | 10,000 | Single | 32 |
| Cameron | U | 13⅝" | 15,000 | Single | 36 |
| NOV | Shaffer LWS | 13⅝" | 10,000 | Single | 28 |
| NOV | Shaffer SL | 13⅝" | 15,000 | Single | 34 |
| Hydril | RAM | 18¾" | 15,000 | Single | 48 |

---

## Annular Preventers

### Annular Preventer Specifications

| Manufacturer | Model | Bore (in) | WP (psi) | Height (in) | Weight (lb) |
|-------------|-------|-----------|----------|-------------|-------------|
| Hydril | GK | 7-1/16 | 5,000 | 24 | 2,500 |
| Hydril | GK | 11 | 5,000 | 30 | 5,500 |
| Hydril | GK | 13⅝ | 10,000 | 36 | 12,000 |
| Cameron | DL | 11 | 5,000 | 28 | 5,000 |
| Cameron | DL | 13⅝ | 10,000 | 34 | 10,000 |
| NOV | Shaffer | 11 | 5,000 | 26 | 4,500 |
| NOV | Shaffer | 13⅝ | 10,000 | 32 | 9,500 |

### Annular Operating Characteristics

```
CLOSING SEQUENCE
├── Operating Pressure Range
│   ├── Minimum close: 200-400 psi
│   ├── Full close: 1000-1500 psi
│   └── Maximum: 3000 psi
├── Closing Time
│   ├── Target: <30 seconds
│   └── API requirement varies by size
└── Stripping Pressure
    ├── Lower than close pressure
    ├── Typically 500-800 psi
    └── Adjusted for pipe speed

ELEMENT LIFE
├── Closure Cycles: 100-300
├── Stripping: Reduces life significantly
├── Temperature: Max 250-300°F
└── H2S: Special compounds required
```

### Annular Element Sizing

| Pipe Range | Element Selection |
|-----------|-------------------|
| 2⅜" - 5½" DP | Standard element |
| 5" - 9⅝" casing | Standard element |
| 9⅝" - 13⅜" | Large bore element |
| Open hole | Standard element |
| Kelly/square | Special element |

---

## Accumulator Systems

### Accumulator Sizing Requirements

```
MINIMUM CAPACITY (Per API RP 53)
├── Close all BOPs + 50% reserve
│   AND
├── Have remaining 200 psi above precharge
│   AND
├── Operate with pumps off

VOLUME CALCULATION
├── Usable Volume = Total - (Precharge × Bottles / WP)
├── Required = Σ (Close Volumes) × 1.5
└── Bottles Needed = Required / Usable per bottle
```

### Accumulator Bottle Specifications

| Size (gal) | Precharge (psi) | Working (psi) | Usable (gal) |
|------------|-----------------|---------------|--------------|
| 10 | 1000 | 3000 | 6.7 |
| 11 | 1000 | 3000 | 7.3 |
| 15 | 1000 | 3000 | 10.0 |
| 20 | 1000 | 3000 | 13.3 |
| 11 | 1500 | 3000 | 5.5 |
| 15 | 1500 | 3000 | 7.5 |

### Accumulator Precharge

| Working Pressure | Minimum Precharge |
|-----------------|-------------------|
| 1500 psi | 750 psi |
| 3000 psi | 1000-1500 psi |
| 5000 psi | 1500-2000 psi |

### Accumulator Pump Unit Specifications

| Output (gpm) | Pressure (psi) | Motor (HP) | Type |
|-------------|----------------|-----------|------|
| 5-10 | 3000 | 15-25 | Electric triplex |
| 10-15 | 3000 | 30-50 | Electric triplex |
| 15-25 | 3000 | 50-75 | Electric triplex |
| 5-10 | 5000 | 25-40 | Electric |
| Air-operated | 3000 | N/A | Pneumatic backup |

---

## Choke Manifold

### Choke Manifold Configuration

```
STANDARD CONFIGURATION
├── Inlet (2)
│   ├── From BOP stack (primary)
│   └── Kill line connection
├── Chokes
│   ├── Manual adjustable
│   ├── Hydraulic adjustable
│   └── Fixed (backup)
├── Gauges
│   ├── Casing pressure
│   ├── Drill pipe pressure
│   └── Choke downstream
└── Outlets
    ├── Mud gas separator
    ├── Flare
    └── Reserve pit (emergency)
```

### Choke Specifications

| Type | Size | Pressure Rating | Application |
|------|------|-----------------|-------------|
| Positive (manual) | 2-4" | 5,000-15,000 | Primary control |
| Positive (hydraulic) | 2-4" | 10,000-15,000 | Remote operation |
| Fixed | 2-4" | 15,000 | Backup |
| Rotating disc | 3-4" | 15,000 | Drilling choke |

### Choke Manifold Pressure Ratings

| System Class | Working Pressure | Test Pressure |
|--------------|-----------------|---------------|
| 3M | 3,000 psi | 4,500 psi |
| 5M | 5,000 psi | 7,500 psi |
| 10M | 10,000 psi | 15,000 psi |
| 15M | 15,000 psi | 22,500 psi |
| 20M | 20,000 psi | 30,000 psi |

---

## BOP Testing Requirements

### Pressure Test Schedule

| Event | Test Type | Pressure |
|-------|-----------|----------|
| Initial (new) | Full pressure | 100% WP |
| Installation | High/Low | 70% WP / 200-300 psi |
| Every 14 days | High/Low | 70% WP / 200-300 psi |
| After repair | High/Low | 70% WP / 200-300 psi |
| Ram change | High/Low | 70% WP / 200-300 psi |
| Casing change | High only | 70% WP |

### Pressure Test Duration

| Test Type | Hold Time | Acceptable Pressure Drop |
|-----------|-----------|-------------------------|
| Low pressure | 5 minutes | Zero |
| High pressure | 5 minutes | Zero |
| Final acceptance | 10 minutes | Zero |

### Function Test Schedule

| Component | Frequency | Test Method |
|-----------|-----------|-------------|
| Ram preventers | Weekly | Open/Close |
| Annular | Weekly | Open/Close |
| Fail-safe valves | Weekly | Function |
| Remote panels | Weekly | Operation |
| Accumulators | Weekly | Pressure/volume |
| Chokes | Before use | Operation |

### Function Test Acceptance Criteria

| Component | Criteria |
|-----------|----------|
| Rams | Close in <30 seconds |
| Annular | Close in <45 seconds |
| Accumulator | Maintain 200 psi above precharge after closes |
| Regulators | Hold set pressure ±50 psi |
| Indicators | Correctly show position |

---

## BOP Stack Configurations

### Surface Stack (Land/Platform)

```
MINIMUM CONFIGURATION (Land)
├── Annular Preventer
├── Double Ram (or 2 singles)
│   ├── Pipe rams (for pipe in hole)
│   └── Blind rams
├── Drilling Spool
│   ├── Kill line connection
│   └── Choke line connection
└── Casing Head

ENHANCED CONFIGURATION
├── Annular Preventer
├── Triple Ram
│   ├── Upper pipe rams
│   ├── Blind/Shear rams
│   └── Lower pipe rams
├── Drilling Spool
└── Casing Head
```

### Subsea Stack Configuration

```
TYPICAL DEEPWATER STACK
├── Lower Marine Riser Package (LMRP)
│   ├── Annular (2)
│   ├── Connector
│   └── Control pods (2)
├── BOP Stack
│   ├── Blind Shear Ram
│   ├── Casing Shear Ram
│   ├── Pipe Rams (2-3)
│   ├── Variable Bore Rams
│   └── Test Ram
├── Wellhead Connector
│   ├── 18¾" typical
│   └── Hydraulic lock
└── Support Systems
    ├── Multiplex control
    ├── Acoustic backup
    └── ROV intervention
```

---

## Component Life and Replacement

### Recommended Replacement Intervals

| Component | Interval | Condition |
|-----------|----------|-----------|
| Ram packers | 3-5 years | Or when damaged |
| Annular element | 2-3 years | Or 200 cycles |
| O-rings | Annual | Or when leaking |
| Seals | Annual | Or when leaking |
| Bonnets | 5 years | NDT inspection |
| Accum bladder | 3-5 years | Or failure |

### Inspection Requirements

| Component | Method | Frequency |
|-----------|--------|-----------|
| Ram bodies | Visual + NDT | Annual |
| Ram packers | Visual | Each test |
| Annular element | Visual | Each test |
| Bolting | Visual + torque | Annual |
| Accum bottles | UT + visual | 5 years |
| Control system | Function test | Weekly |

---

## Quick Reference

### BOP Operating Pressures

| Function | Typical Pressure |
|----------|-----------------|
| Ram close | 1500 psi |
| Ram open | 1500 psi |
| Annular close | Variable (see table) |
| Annular open | 1500 psi |
| Shear rams | 3000 psi |
| Emergency | 3000 psi |

### Annular Close Pressure Guide

| Operation | Pressure (psi) |
|-----------|---------------|
| Close on drill pipe | 800-1200 |
| Close on drill collars | 1200-1500 |
| Close on open hole | 1500-2000 |
| Stripping pipe | 500-800 |

---

*Always reference manufacturer specifications and API standards for specific equipment. This guide provides general information only.*
