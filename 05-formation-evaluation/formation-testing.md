# Formation Testing

## Overview

Formation testing measures reservoir pressure and fluid properties, providing critical data for reservoir characterization, completion design, and reserve estimation. Tests range from wireline formation testers to full drill stem tests.

---

## Wireline Formation Testers

### Tool Types

| Tool | Description | Application |
|------|-------------|-------------|
| **RFT (Repeat Formation Tester)** | Original wireline tester | Legacy tool |
| **MDT (Modular Formation Dynamics Tester)** | Modular, multiple probes | Most common |
| **XPT, FRT, etc.** | Various service company tools | Similar capabilities |

### Measurement Capabilities

| Measurement | Use |
|-------------|-----|
| **Formation pressure** | Reservoir pressure, gradient |
| **Fluid mobility** | Permeability-thickness product |
| **Fluid samples** | PVT, composition, contamination |
| **Pressure transient** | Permeability, skin |
| **Interval pressure** | Dual packer capability |

### Test Types

**Pretests (Pressure Points)**:
- Small volume test (5-20 cc)
- Quick pressure measurement
- Multiple points per run
- Mobility estimate

**Sampling**:
- Larger volume extraction (1-6 gallons)
- Fluid collected in sample chambers
- Monitor contamination real-time
- Multiple PVT samples possible

**Mini-DST (Interval Tests)**:
- Dual packer isolation
- Flow formation to surface or chamber
- Pressure transient analysis
- Larger radius of investigation

---

## Pressure Interpretation

### Pressure vs. Depth Plot

```
Depth (ft)          Pressure (psi)

   │
8000├────────┐
   │        ●────── Gas gradient (0.1-0.2 psi/ft)
   │        │
8200├────────┼──────●─────────────────── GOC
   │        │      ●
   │        │      │ Oil gradient (0.3-0.35 psi/ft)
8400├────────┼──────┼────●
   │        │      │    ●
   │        │      │    │
8600├────────┼──────┼────┼─────●──────── OWC
   │        │      │    │     ●
   │        │      │    │     │ Water gradient (0.43-0.52 psi/ft)
8800├────────┼──────┼────┼─────┼───●
   │        │      │    │     │   │
   └────────┴──────┴────┴─────┴───┴──────►
            3600   3700 3800  3900 4000
```

### Fluid Gradients

| Fluid | Typical Gradient (psi/ft) |
|-------|---------------------------|
| **Gas** | 0.05 - 0.20 |
| **Condensate** | 0.15 - 0.25 |
| **Light oil** | 0.28 - 0.32 |
| **Medium oil** | 0.32 - 0.38 |
| **Heavy oil** | 0.38 - 0.43 |
| **Fresh water** | 0.433 |
| **Salt water** | 0.45 - 0.52 |

### Pressure Gradient Calculation

```
Gradient (psi/ft) = ΔP / ΔD = (P₂ - P₁) / (D₂ - D₁)

Example:
P₁ = 3,850 psi at D₁ = 8,200 ft
P₂ = 3,970 psi at D₂ = 8,550 ft

Gradient = (3970 - 3850) / (8550 - 8200) = 120/350 = 0.343 psi/ft
→ This indicates oil
```

---

## Drill Stem Testing (DST)

### DST Objectives

1. **Confirm producibility** - Will formation flow?
2. **Estimate deliverability** - How much?
3. **Obtain fluid samples** - PVT analysis
4. **Measure reservoir pressure** - Initial pressure
5. **Estimate permeability** - From buildup analysis
6. **Confirm fluid contacts** - Verify log interpretation

### DST String Components

```
┌──────────────────────────────────────────────────────┐
│                   DST STRING                         │
├──────────────────────────────────────────────────────┤
│                                                      │
│   ┌──────────────┐                                   │
│   │ Surface      │ ← Flow to test equipment         │
│   │ Equipment    │                                   │
│   └──────┬───────┘                                   │
│          │                                           │
│   ┌──────▼───────┐                                   │
│   │ Drill Pipe   │ ← Conduit for flow               │
│   └──────┬───────┘                                   │
│          │                                           │
│   ┌──────▼───────┐                                   │
│   │ Circulating  │ ← Allows reverse circulation     │
│   │ Sub          │                                   │
│   └──────┬───────┘                                   │
│          │                                           │
│   ┌──────▼───────┐                                   │
│   │ Safety Valve │ ← Shuts in well if needed        │
│   └──────┬───────┘                                   │
│          │                                           │
│   ┌──────▼───────┐                                   │
│   │ Pressure     │ ← Records downhole P/T           │
│   │ Recorders    │                                   │
│   └──────┬───────┘                                   │
│          │                                           │
│   ┌──────▼───────┐                                   │
│   │ Test Valve   │ ← Opens/closes for flow periods  │
│   │ (Tester)     │                                   │
│   └──────┬───────┘                                   │
│          │                                           │
│   ┌──────▼───────┐                                   │
│   │ Bypass Valve │ ← Equalizes pressure for POOH    │
│   └──────┬───────┘                                   │
│          │                                           │
│   ┌──────▼───────┐                                   │
│   │ Packer       │ ← Isolates test interval         │
│   └──────┬───────┘                                   │
│          │                                           │
│   ┌──────▼───────┐                                   │
│   │ Perforated   │ ← Allows flow from formation     │
│   │ Anchor       │                                   │
│   └──────────────┘                                   │
│                                                      │
└──────────────────────────────────────────────────────┘
```

### DST Sequence

| Period | Duration | Purpose |
|--------|----------|---------|
| **Initial flow** | 5-15 min | Clean up, establish flow |
| **Initial shut-in** | 30-60 min | Initial pressure buildup |
| **Main flow** | 1-4 hrs | Sustained flow, sample |
| **Final shut-in** | 1-4 hrs | Final pressure buildup |

### DST Pressure Record

```
Pressure
    │
    │                                    ┌─────────────
    │                                   ╱ Final Shut-in
    │                                  ╱  (Buildup)
    │              ┌─────────        ╱
    │             ╱ Initial         ╱
    │            ╱  Shut-in       ╱
    │           ╱              ╱ Main Flow
    │    ─────┘              ╱  Period
    │    Initial            ╱
    │    Flow             ─┘
    │    ──────
    └────────────────────────────────────────────────► Time
          │      │          │               │
        Open   Close      Open           Close
```

---

## Flow Period Analysis

### Flow Rate Measurement

| Method | Application |
|--------|-------------|
| **Separator** | Accurate metering |
| **Flow through choke** | Rate estimate |
| **Tank gauging** | Oil volume |
| **Flare/vent** | Gas estimation |

### Productivity Index

```
PI = Q / (Pe - Pwf)

Where:
PI = Productivity Index (STB/day/psi)
Q = Flow rate (STB/day)
Pe = Reservoir pressure (psi)
Pwf = Flowing bottomhole pressure (psi)
```

### Flow Efficiency

```
FE = (Pe - Pwf - ΔPskin) / (Pe - Pwf)

Where:
ΔPskin = Pressure drop due to skin
```

---

## Pressure Buildup Analysis

### Horner Analysis

**Horner Time**:
```
Horner Time = (tp + Δt) / Δt

Where:
tp = Producing time
Δt = Shut-in time
```

**Permeability from Slope**:
```
k = (162.6 × Q × μ × B) / (m × h)

Where:
k = Permeability (md)
Q = Flow rate (STB/day)
μ = Viscosity (cp)
B = Formation volume factor
m = Slope of Horner plot
h = Net pay thickness (ft)
```

### Skin Factor

```
s = 1.151 × [(P1hr - Pwf)/m - log(k/(φμctrw²)) + 3.23]

Where:
P1hr = Pressure at 1 hour shut-in
Pwf = Final flowing pressure
s = Skin factor
```

**Skin Interpretation**:

| Skin Value | Interpretation |
|------------|----------------|
| s < 0 | Stimulated (fractured, acidized) |
| s = 0 | No damage |
| s = 1-5 | Slight damage |
| s = 5-10 | Moderate damage |
| s > 10 | Severe damage |

---

## Fluid Sampling

### Sample Quality Requirements

| Parameter | Requirement |
|-----------|-------------|
| **Contamination** | < 5% (ideally < 1%) |
| **Single phase** | Maintain above bubble point |
| **Representative** | True reservoir fluid |
| **Volume** | Adequate for PVT analysis |

### Contamination Monitoring

| Indicator | Interpretation |
|-----------|----------------|
| **GOR trending up** | Improving quality |
| **Resistivity stable** | Lower contamination |
| **Fluorescence** | Crude vs. OBM |
| **Optical density** | Real-time contamination |

### Sample Containers

| Type | Capacity | Application |
|------|----------|-------------|
| **Single phase** | 450-600 cc | Liquids |
| **Multi-chamber** | 2.75-6 gal | Multiple samples |
| **PVT** | Various | Lab analysis |

---

## Test Interpretation Deliverables

### Data Required

| Parameter | Use |
|-----------|-----|
| **Initial pressure** | Reservoir energy |
| **Flow rates** | Deliverability |
| **Pressure transients** | Permeability, skin |
| **Fluid samples** | PVT properties |
| **Temperature** | Reservoir conditions |

### Calculated Results

| Result | Significance |
|--------|--------------|
| **Permeability (k)** | Flow capacity |
| **Skin (s)** | Formation damage |
| **Radius of investigation** | Test coverage |
| **Productivity Index** | Well potential |
| **Reservoir limits** | Boundaries if seen |

---

## Testing Considerations

### Pre-Test Checklist

- [ ] Test objectives defined
- [ ] Test interval confirmed
- [ ] Equipment rated for conditions
- [ ] Well control equipment ready
- [ ] Test string made up
- [ ] Surface test equipment rigged up
- [ ] Sample containers ready
- [ ] Disposal/storage for fluids arranged

### Safety Considerations

| Hazard | Mitigation |
|--------|------------|
| **H2S** | Monitors, breathing air, training |
| **High pressure** | Rated equipment, barriers |
| **Hydrocarbons** | Fire watch, no ignition sources |
| **Well control** | BOP tested, kill fluid ready |
| **Fluid handling** | Containment, PPE |

### Common Problems

| Problem | Cause | Solution |
|---------|-------|----------|
| **Won't flow** | Low permeability, damage | Swab, perforate, stimulate |
| **Tight hole** | Debris, swelling | Circulate, wash, POOH |
| **Packer leak** | Poor seal, damaged packer | Reset, replace |
| **Poor buildup** | Short flow, tool issues | Extend test, verify equipment |
| **Contaminated sample** | Insufficient cleanup | Continue pumping, better technique |
