# Completion Design

## Overview

Completion design involves selecting and configuring equipment to connect the reservoir to the surface efficiently and safely. Good completion design maximizes production while protecting the wellbore and enabling future interventions.

---

## Completion Objectives

### Primary Objectives
1. **Maximize production** - Optimize flow from reservoir
2. **Wellbore integrity** - Long-term mechanical reliability
3. **Safety** - Prevent uncontrolled flow
4. **Zonal isolation** - Prevent cross-flow
5. **Future access** - Enable intervention and workover

### Design Considerations

| Factor | Considerations |
|--------|----------------|
| **Reservoir** | Pressure, temperature, fluid properties |
| **Production** | Expected rates, artificial lift |
| **Formation** | Sand production, scale, corrosion |
| **Economics** | Initial cost vs. long-term production |
| **Regulations** | Barrier requirements, testing |
| **Operations** | Intervention access, workover capability |

---

## Completion Types

### Open Hole Completions

**Description**: Production from uncased interval

```
┌─────────────────────────────────────┐
│          OPEN HOLE COMPLETION       │
├─────────────────────────────────────┤
│                                     │
│   Casing ────────│                  │
│                  │                  │
│   Packer ───────╞╡                  │
│                  │                  │
│   Tubing ────────│                  │
│                  │                  │
│   Liner Hanger ──┼─────             │
│                  │     │            │
│                  │     │ Open Hole  │
│                        │ (No Casing)│
│                        │            │
│                        │ Formation  │
│                  ──────┘            │
│                                     │
└─────────────────────────────────────┘
```

**Advantages**:
- Lower cost (no perforating)
- Full borehole flow area
- No casing damage concerns
- Easy sidetrack if needed

**Disadvantages**:
- No zonal isolation
- Wellbore stability risks
- Limited intervention options
- Sand control challenges

**Best Applications**:
- Competent formations
- Horizontal wells in single zone
- Naturally fractured carbonates

### Cased Hole Completions

**Description**: Production through perforated casing/liner

```
┌─────────────────────────────────────┐
│        CASED HOLE COMPLETION        │
├─────────────────────────────────────┤
│                                     │
│   Casing ────────│                  │
│                  │                  │
│   Packer ───────╞╡                  │
│                  │                  │
│   Tubing ────────│                  │
│                  │                  │
│   Production ────│                  │
│   Casing/Liner   │                  │
│                  │                  │
│   Perforations ──│●●●●●│            │
│                  │     │ Cement     │
│                  │●●●●●│            │
│                  │                  │
│   Cement ────────│█████│            │
│                  └─────┘            │
│                                     │
└─────────────────────────────────────┘
```

**Advantages**:
- Zonal isolation
- Wellbore stability
- Multiple zone capability
- Intervention flexibility

**Disadvantages**:
- Perforating costs
- Flow restriction through perfs
- Cement job quality critical
- Casing damage potential

### Liner Completions

**Description**: Liner hung from casing, not tied back to surface

```
Liner Hanger ──┬─┐
               │ │
               │ │ Production Liner
               │ │
Perforations ──│●│
               │●│
               └─┘
```

**Advantages**:
- Lower cost than full string
- Less tubing/casing required
- Lighter string weights

**Disadvantages**:
- Liner hanger seal critical
- More complex interventions
- Annular access issues

---

## Completion Configuration

### Single Zone Completion

| Component | Purpose |
|-----------|---------|
| Tubing | Flow conduit |
| Packer | Isolate annulus |
| Landing nipple | Enable wireline |
| Perforations | Access formation |

### Multi-Zone Completion

| Component | Purpose |
|-----------|---------|
| Dual packers | Zone isolation |
| Sliding sleeves | Zone control |
| Multiple nipples | Intervention access |
| Commingled or selective | Production strategy |

### Smart/Intelligent Completions

| Feature | Capability |
|---------|------------|
| Downhole gauges | Real-time P/T monitoring |
| Flow control valves | Remote choke adjustment |
| Zonal isolation | Selective production |
| Data transmission | Fiber optic, electronic |

---

## Inflow Performance

### Productivity Index (PI)

```
PI = Q / (Pe - Pwf)

Where:
Q = Flow rate (STB/day)
Pe = Reservoir pressure (psi)
Pwf = Flowing bottomhole pressure (psi)
PI = Productivity index (STB/day/psi)
```

### IPR (Inflow Performance Relationship)

**Vogel Equation (Solution Gas Drive)**:
```
Q/Qmax = 1 - 0.2(Pwf/Pe) - 0.8(Pwf/Pe)²
```

### Skin Effect

| Skin | Interpretation |
|------|----------------|
| Negative | Stimulated (fracture, acid) |
| Zero | No damage |
| Positive | Damaged |

**Skin Sources**:
- Drilling damage
- Perforation damage
- Partial penetration
- Limited entry

---

## Completion Interval Selection

### Selection Criteria

| Factor | Consideration |
|--------|---------------|
| **Net pay** | Exclude non-productive intervals |
| **Permeability** | Focus on high-perm zones |
| **Fluid contacts** | Stay above OWC/WOC |
| **Mechanical** | Avoid unstable zones |
| **Barriers** | Cement behind perforations |

### Perforation Strategy

| Strategy | Application |
|----------|-------------|
| **Full interval** | Uniform reservoir, maximize exposure |
| **Selective** | Variable quality, water/gas avoidance |
| **Limited entry** | Control flow profile, stimulation |
| **Oriented** | Directional fractures, stress |

---

## Completion Fluid Design

### Functions

1. Control well pressure
2. Protect formation
3. Enable equipment deployment
4. Clean and non-damaging

### Fluid Types

| Type | Density Range | Application |
|------|---------------|-------------|
| **Completion brine** | 8.4-19.2 ppg | Most common |
| **Filtered seawater** | 8.6 ppg | Offshore |
| **CaCl₂** | Up to 11.6 ppg | Higher density |
| **CaBr₂** | Up to 14.2 ppg | High density |
| **ZnBr₂** | Up to 19.2 ppg | Highest density |

### Fluid Properties

| Property | Requirement | Purpose |
|----------|-------------|---------|
| **Density** | Overbalance 200-500 psi | Well control |
| **Solids-free** | 2 micron filtered | Prevent plugging |
| **Compatible** | With formation/fluids | Prevent damage |
| **Inhibited** | Corrosion inhibitor | Protect equipment |

---

## Completion Equipment Selection

### Tubing Selection Factors

| Factor | Consideration |
|--------|---------------|
| **Size** | Match to expected rates |
| **Material** | Corrosion resistance |
| **Thread** | Leak resistance, torque |
| **Tensile** | Installation and operational loads |

### Packer Selection Factors

| Factor | Consideration |
|--------|---------------|
| **Type** | Permanent vs. retrievable |
| **Pressure rating** | Differential, collapse |
| **Temperature** | Elastomer compatibility |
| **Set method** | Mechanical, hydraulic, electric |
| **Release** | Requirements for future |

---

## Completion Schematic Requirements

### Essential Information

| Element | Details |
|---------|---------|
| **Depths** | All components (MD and TVD) |
| **Sizes** | Casing, tubing, IDs and ODs |
| **Connections** | Thread types |
| **Perforations** | Intervals, shots per foot, phasing |
| **Packers** | Type, set depth, specs |
| **Accessories** | Nipples, valves, gauges |

### Standard Schematic Format

```
WELL: Example 1-H
COMPLETION DATE: XX/XX/XXXX

Surface Casing: 13-3/8" @ 1,500' MD
Intermediate: 9-5/8" @ 8,500' MD
Production Liner: 5-1/2" @ 15,000' MD

COMPLETION:
┌──────────────────────────────┐
│ Tubing Head                  │ 0' MD
│ 4-1/2" 12.6# L-80 PH6 Tubing │
│                              │
│ SCSSV @ 500' MD              │
│                              │
│ Landing Nipple @ 8,200' MD   │
│                              │
│ Production Packer @ 8,400' MD│
│                              │
│ Seal Assembly                │
│                              │
│ 5-1/2" 17# P-110 Liner       │
│                              │
│ Perfs: 8,600-8,650' MD       │
│ 4 SPF, 60° phasing           │
└──────────────────────────────┘
```

---

## Completion Testing

### Required Tests

| Test | Purpose | Acceptance |
|------|---------|------------|
| **Tubing pressure test** | Verify tubing integrity | Hold pressure, no leak |
| **Packer test** | Verify seal | Annular pressure test |
| **SCSSV test** | Verify function | Close/open verification |
| **Annular test** | Verify annular integrity | Hold pressure |

### Flow Testing

| Measurement | Purpose |
|-------------|---------|
| **Flow rate** | Establish productivity |
| **Flowing pressure** | Calculate PI |
| **Water cut** | Baseline water production |
| **GOR** | Baseline gas production |
| **Temperature** | Verify flow |

---

## Completion Checklist

### Design Phase
- [ ] Reservoir data reviewed
- [ ] Production forecast developed
- [ ] Completion type selected
- [ ] Equipment specifications finalized
- [ ] Completion schematic approved
- [ ] Procedures written

### Installation Phase
- [ ] Hole conditioned
- [ ] Tubing inspected and drifted
- [ ] Equipment function tested
- [ ] Completion fluid prepared
- [ ] Tubing run per procedure
- [ ] All depths verified
- [ ] Pressure tests passed

### Commissioning Phase
- [ ] Perforations shot
- [ ] Well flowed and cleaned up
- [ ] Production tests completed
- [ ] SCSSV tested
- [ ] Final completion report issued
