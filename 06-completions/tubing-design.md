# Tubing Design

## Overview

Production tubing is the conduit for reservoir fluids to surface. Proper tubing design ensures safe operations, optimum production, and long well life while accommodating thermal and pressure changes.

---

## Tubing Selection Criteria

### Size Selection

**Factors Affecting Size**:
- Expected production rate
- Artificial lift requirements
- Pressure losses
- Well depth
- Casing size
- Intervention tools

**Common Tubing Sizes**:

| Tubing OD | ID (Typical) | Application |
|-----------|--------------|-------------|
| 2-3/8" | 1.995" | Low rate, slim holes |
| 2-7/8" | 2.441" | Common, moderate rates |
| 3-1/2" | 2.992" | Higher rates |
| 4-1/2" | 3.958" | High rate, gas wells |
| 5-1/2" | 4.892" | Very high rate |

### Nodal Analysis for Sizing

```
Pressure
    │
    │   IPR (Inflow)
    │   ╲
    │    ╲
    │     ╲
    │      ╲  Operating Point
    │       ╳─────────────
    │      ╱ TPR (Outflow)
    │     ╱
    │    ╱
    │   ╱
    └─────────────────────► Flow Rate

Select tubing size to optimize operating point
```

---

## Tubing Grades

### API Grades

| Grade | Yield Strength (psi) | Application |
|-------|---------------------|-------------|
| H-40 | 40,000 | Shallow, low stress |
| J-55 | 55,000 | Low to moderate |
| C-75 | 75,000 | Moderate stress |
| L-80 | 80,000 | Moderate, CO2 service |
| N-80 | 80,000 | Standard |
| C-90 | 90,000 | Higher stress, H2S |
| T-95 | 95,000 | High stress, H2S |
| P-110 | 110,000 | High stress |
| Q-125 | 125,000 | Deep, high pressure |

### Material Selection for Corrosion

| Environment | Material Consideration |
|-------------|----------------------|
| Sweet (CO2) | Carbon steel, L-80 |
| Sour (H2S) | NACE grades (L-80, C-90, T-95) |
| High CO2 + temperature | 13Cr, 22Cr, 25Cr |
| High chlorides | Duplex, super duplex |
| Extreme | Nickel alloys (Inconel, Hastelloy) |

---

## Tubing Connections

### Connection Types

| Type | Description | Application |
|------|-------------|-------------|
| **EUE (External Upset)** | Standard API, upset ends | General service |
| **NUE (Non-Upset)** | No upset, flush OD | Slim holes |
| **Premium** | Metal-to-metal seal | High pressure, gas |
| **Specialty** | Various designs | Specific requirements |

### Connection Performance Ratings

| Property | Significance |
|----------|--------------|
| **Tensile efficiency** | % of pipe body strength |
| **Compression** | Resistance to buckling loads |
| **Internal pressure** | Leak resistance |
| **External pressure** | Collapse resistance |
| **Gas-tight** | Metal seal vs. thread seal |

### Premium Connection Features

- Metal-to-metal seal
- Higher tensile efficiency
- Torque shoulder
- Better fatigue resistance
- Gas-tight performance

---

## Tubing Stress Analysis

### Load Cases

| Load | Cause | Effect |
|------|-------|--------|
| **Tensile** | Weight, pulling | Stretch, failure |
| **Compression** | Thermal expansion, packer | Buckling |
| **Internal pressure** | Well pressure | Burst |
| **External pressure** | Annular pressure | Collapse |
| **Bending** | Wellbore curvature | Fatigue |
| **Torsion** | Rotation during installation | Connection failure |

### Design Factors

| Load | Minimum Design Factor |
|------|----------------------|
| **Tension** | 1.4 - 1.6 |
| **Burst** | 1.1 - 1.25 |
| **Collapse** | 1.1 - 1.25 |
| **Biaxial** | 1.25 |

### Tension Calculations

**Weight in Air**:
```
Weight = Length × Weight per foot

Example: 10,000 ft of 2-7/8" 6.5 lb/ft
Weight = 10,000 × 6.5 = 65,000 lb
```

**Buoyed Weight**:
```
Buoyancy Factor = 1 - (Fluid Density / Steel Density)
                = 1 - (Mud Weight in ppg / 65.4)

Example: 9 ppg mud
BF = 1 - (9/65.4) = 0.862

Buoyed Weight = 65,000 × 0.862 = 56,030 lb
```

---

## Tubing Movement

### Causes of Movement

| Effect | Cause | Direction |
|--------|-------|-----------|
| **Temperature** | Heating = expansion | Down |
| **Ballooning** | Internal pressure increase | Down |
| **Reverse ballooning** | Internal pressure decrease | Up |
| **Buckling** | Compression | Shortening |
| **Piston effect** | Pressure on packer area | Variable |

### Movement Calculations

**Temperature Effect**:
```
ΔL = α × L × ΔT

Where:
α = Coefficient of expansion (6.9 × 10⁻⁶ /°F for steel)
L = Length
ΔT = Temperature change

Example: 10,000 ft, 100°F increase
ΔL = 6.9×10⁻⁶ × 10,000 × 100 = 6.9 ft expansion
```

**Ballooning Effect**:
```
ΔL = (2v × L × ΔPi) / E × (R² / (R² - 1))

Where:
v = Poisson's ratio (0.3)
ΔPi = Internal pressure change
E = Young's modulus
R = OD/ID ratio
```

### Movement Compensation

| Method | Mechanism |
|--------|-----------|
| **Seal assembly travel** | Allows seal to move in polished bore |
| **Expansion joint** | Telescoping joint absorbs movement |
| **Landed compression** | Set tubing in compression |
| **PBR length** | Size polished bore for expected travel |

---

## Tubing Anchors and Packers

### Tubing Anchor Catchers (TAC)

**Purpose**: Prevent tubing movement, vibration

| Type | Application |
|------|-------------|
| **Mechanical** | Standard service |
| **Hydraulic** | High tension |
| **Tension anchor** | Prevent upward movement |

### Packer-Tubing Interface

| Configuration | Movement Allowed |
|---------------|------------------|
| **Anchored** | No movement, tubing fixed to packer |
| **Free movement** | Seal in PBR, movement allowed |
| **Limited movement** | Movement within travel limits |

---

## Tubing Accessories

### Nipples

| Type | Purpose |
|------|---------|
| **Landing nipple** | Land wireline tools |
| **No-go nipple** | Positive lock for plugs |
| **Selective nipple** | Multiple positioning |
| **Flow coupling** | Protect against turbulent flow erosion |

### Safety Valves

| Type | Purpose |
|------|---------|
| **SCSSV** | Surface-controlled, fail safe close |
| **SSCSV** | Subsurface-controlled |
| **Storm choke** | Automatic closure at high rate |

### Other Accessories

| Accessory | Purpose |
|-----------|---------|
| **Blast joint** | Protect against perforation erosion |
| **Flow coupling** | Protect near restrictions |
| **Chemical injection mandrel** | Inject chemicals downhole |
| **Side pocket mandrel** | Gas lift valves |
| **Sliding sleeve** | Open/close circulation |

---

## Tubing Running Procedures

### Pre-Run Checks

- [ ] Tally pipe, verify footage
- [ ] Drift all tubing (100% drift)
- [ ] Inspect threads, protectors
- [ ] Verify accessories
- [ ] Confirm completion fluid
- [ ] Calculate running string weight

### Running Best Practices

| Practice | Purpose |
|----------|---------|
| **Clean threads** | Good seal, prevent galling |
| **Proper dope** | Lubrication, corrosion protection |
| **Correct torque** | Prevent leaks, over-torque damage |
| **Controlled speed** | Prevent surge, tool damage |
| **Fill tubing** | Reduce collapse load |
| **Monitor weights** | Detect problems |

### Make-Up Torque

| Tubing Size | EUE Torque (ft-lb) | Premium (typical) |
|-------------|-------------------|-------------------|
| 2-3/8" 4.7# | 1,300 | Per manufacturer |
| 2-7/8" 6.5# | 2,200 | Per manufacturer |
| 3-1/2" 9.3# | 3,700 | Per manufacturer |
| 4-1/2" 12.6# | 5,900 | Per manufacturer |

---

## Tubing Pressure Testing

### Test Requirements

| Test | Pressure | Duration |
|------|----------|----------|
| **Tubing** | Rated pressure or per program | 10-30 min |
| **Connection** | As tubing runs (hydrotest) | N/A |
| **Packer** | Below and above | 10-15 min |
| **System** | Full wellhead test | 10-30 min |

### Test Criteria

- No pressure drop (or < 5% allowed)
- No visible leaks
- Documentation signed

---

## Tubing Design Checklist

### Design Phase
- [ ] Size selection (nodal analysis)
- [ ] Grade selection (stress, corrosion)
- [ ] Connection selection
- [ ] Movement calculations
- [ ] Accessories specified
- [ ] Load analysis completed

### Installation Phase
- [ ] Pipe inspected and tallied
- [ ] 100% drift completed
- [ ] Torque specifications confirmed
- [ ] Running procedure reviewed
- [ ] Pressure test procedure ready

### Completion Phase
- [ ] All pressure tests passed
- [ ] Final depths recorded
- [ ] Completion schematic updated
- [ ] As-built documentation complete
