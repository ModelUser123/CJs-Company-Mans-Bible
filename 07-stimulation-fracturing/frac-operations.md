# Frac Operations

## Overview

This section covers the operational execution of hydraulic fracturing, from pre-frac testing through multi-stage completions and real-time optimization.

---

## Pre-Frac Testing

### Diagnostic Fracture Injection Test (DFIT)

**Purpose**: Determine closure stress, reservoir pressure, and permeability before main treatment

**Procedure**:
1. Inject small volume (50-500 bbl)
2. Shut in well
3. Monitor pressure decline
4. Analyze for closure pressure and permeability

**DFIT Analysis Parameters**:

| Parameter | Method |
|-----------|--------|
| **Closure pressure** | G-function, sqrt(t) analysis |
| **Reservoir pressure** | Extrapolation |
| **Permeability** | After-closure analysis |
| **Leakoff coefficient** | Before-closure analysis |

### Minifrac (Calibration Treatment)

**Purpose**: Verify parameters, optimize main treatment design

**Typical Procedure**:
1. Pump pad fluid at design rate
2. Shut in and monitor decline
3. Determine actual closure pressure
4. Calculate fluid efficiency
5. Adjust main treatment design

**Key Outputs**:

| Output | Use |
|--------|-----|
| **Closure pressure** | Confirm design stress |
| **Fluid efficiency** | Adjust pad volume |
| **Net pressure** | Verify model |
| **ISIP** | Benchmark pressure |

---

## Stage Isolation Methods

### Plug and Perf (Plug & Perf)

```
┌─────────────────────────────────────────────────────────────────┐
│                    PLUG AND PERF SEQUENCE                       │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│   Step 1: Pump plug and perforating guns on wireline           │
│                                                                 │
│   ═══════════════════════════════╦═══════════════════════════  │
│                                  ║ Wireline                     │
│                                  ║                              │
│                            ┌─────╫─────┐                        │
│                            │  Plug     │                        │
│                            │  + Guns   │                        │
│                            └───────────┘                        │
│                                                                 │
│   Step 2: Set plug, perforate, pull out                        │
│                                                                 │
│   ═══════════●●●●●●●●●════╦═════════════════════════════════   │
│              New perfs    ║ Plug set                            │
│                           ║ (isolates previous stage)           │
│                                                                 │
│   Step 3: Frac through new perfs                                │
│                                                                 │
│   ═══════════●●●●●●●●●════╬═════════════════════════════════   │
│       ↓↓↓↓↓↓↓↓↓↓         ║                                      │
│       Fractures          ║                                      │
│                                                                 │
│   Step 4: Repeat for each stage                                 │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

**Advantages**:
- Placement precision
- Proppant volume per stage
- Operational flexibility

**Considerations**:
- Time for wireline
- Plug drillout required
- Higher cost per stage

### Sliding Sleeve Systems

**Concept**: Pre-installed sleeves opened by ball drop

```
Stage 5 ←── Smallest ball
Stage 4 ←── Larger ball
Stage 3 ←── Larger ball
Stage 2 ←── Larger ball
Stage 1 ←── Largest ball opens, frac toe first
```

**Advantages**:
- Faster stage transitions
- No wireline required
- Pump continuous

**Considerations**:
- Limited stages (ball size limits)
- Sleeve reliability
- Less flexibility

### Coiled Tubing Activated

**Applications**:
- Toe initiation
- Sleeve shifting
- Plug setting
- Remedial work

---

## Perforation Strategy

### Cluster Design

| Parameter | Typical Range |
|-----------|---------------|
| **Clusters per stage** | 3-8 |
| **Cluster spacing** | 25-75 ft |
| **Perfs per cluster** | 3-6 shots |
| **Phasing** | 60° or 180° |
| **Perforation friction** | 500-1,000 psi |

### Limited Entry

**Concept**: Use perforation friction to distribute flow across clusters

**Design**:
```
Perforation Friction = Rate² / (Cd² × Nperfs² × Dperfs⁴)

Higher friction = More uniform distribution
```

### Perforation Erosion

| Concern | Mitigation |
|---------|------------|
| **Sand erosion** | Limit proppant concentration |
| **Perforation diameter growth** | Monitor treating pressure |
| **Lost limited entry** | Adjust rate |

---

## Real-Time Optimization

### Pressure Matching

**During Pumping**:
- Compare actual vs. predicted pressure
- Adjust model parameters
- Modify treatment if needed

| Observation | Adjustment |
|-------------|------------|
| **Pressure lower than expected** | Height growing, reduce rate |
| **Pressure higher than expected** | Near wellbore issues, check perfs |
| **Pressure stable, declining slightly** | Good propagation |
| **Pressure spiking** | Near screenout |

### Rate and Concentration Adjustments

| Situation | Action |
|-----------|--------|
| **Good pressure, on schedule** | Continue |
| **Pressure rising, screenout risk** | Reduce concentration, increase rate |
| **Pressure declining, overflushing** | Increase concentration |
| **Perforation pressure high** | Consider perf cleanup, rate reduction |

---

## Screenout Management

### What is a Screenout?

When proppant bridges in the fracture and pressure rises rapidly

### Screenout Indicators

| Sign | Time to React |
|------|---------------|
| **Pressure rising slowly** | Monitor, prepare |
| **Pressure rising steadily** | Reduce concentration |
| **Pressure rising rapidly** | Flush immediately |
| **Pressure maxing out** | Emergency flush |

### Screenout Response

1. **Immediately flush** - Clean fluid at maximum rate
2. **Reduce pump rate** - Allow proppant to settle
3. **Monitor pressure** - Watch for decline
4. **Document** - Record pressures and volumes

### Screenout Prevention

| Prevention | How |
|------------|-----|
| **Adequate pad** | Size pad for designed length |
| **Proper proppant ramp** | Gradual concentration increase |
| **Rate control** | Maintain design rate |
| **Fluid quality** | Ensure proper viscosity |
| **Perf maintenance** | Avoid erosion issues |

---

## Zipper Frac Operations

### Concept

Alternating between two wells during fracturing operations

```
Well A    Well B
  │         │
  │ Frac    │ Wireline
  │  ↓      │  (prep next stage)
  │         │
  │ Wireline│ Frac
  │  (prep) │  ↓
  │         │
  │ Frac    │ Wireline
  │  ↓      │
```

### Advantages

| Advantage | Benefit |
|-----------|---------|
| **Reduced idle time** | Pump continuously |
| **Efficiency** | More stages per day |
| **Stress shadow** | May improve cluster efficiency |
| **Equipment utilization** | Maximize frac spread |

### Simul-Frac

**Two wells simultaneously**:
- Even higher efficiency
- Requires two-well manifold
- Higher proppant and fluid demand
- Complex coordination

---

## Stage-by-Stage Execution

### Typical Stage Workflow

| Step | Duration | Activities |
|------|----------|------------|
| **Wireline** | 30-60 min | Pump plug/guns, perf, POOH |
| **Wellbore prep** | 15-30 min | Pressure test, prepare |
| **Pumping** | 90-180 min | Pad, slurry stages, flush |
| **Shut-in** | 5-15 min | ISIP, pressure decline |
| **Prepare next** | 15-30 min | Rig up wireline |

### Per-Stage Documentation

| Record | Details |
|--------|---------|
| **Perforations** | Depth, SPF, entry holes |
| **Volumes** | Pad, slurry by stage, flush |
| **Proppant** | Type, mesh, mass |
| **Pressures** | Treating, ISIP, breakdown |
| **Rates** | Average, max, by stage |
| **Anomalies** | Any issues or observations |

---

## Frac Fleet Coordination

### Key Roles

| Role | Responsibility |
|------|----------------|
| **Company Man** | Final authority, safety, costs |
| **Frac Supervisor** | Overall frac execution |
| **Treatment Engineer** | Design, real-time analysis |
| **Pump Operator** | Pump control, maintenance |
| **Blender Operator** | Slurry mixing, QC |
| **Wireline Operator** | Plug/perf operations |
| **Sand Coordinator** | Proppant logistics |

### Communication Protocol

| Channel | Use |
|---------|-----|
| **Radio Channel 1** | Operations (frac) |
| **Radio Channel 2** | Sand/logistics |
| **Radio Channel 3** | Safety |
| **Phone** | Office communication |
| **Data** | Real-time monitoring |

---

## End of Stage Procedures

### Flush Calculation

```
Flush Volume = Tubing Volume + Surface Line Volume + Safety Factor

Surface to Perf Volume = Tubing Volume (bbl)

Flush = Volume + (5-10% safety)
```

### Post-Stage Checks

- [ ] Confirm proppant in formation (not over-flushed)
- [ ] Record ISIP
- [ ] Monitor pressure decline
- [ ] Verify stage complete in records
- [ ] Prepare for next stage

---

## Quality Control

### Fluid QC

| Test | Frequency |
|------|-----------|
| **Viscosity** | Each tank, continuous |
| **pH** | Continuous |
| **Break time** | Sample each batch |
| **Density** | Continuous blender |

### Proppant QC

| Test | Requirement |
|------|-------------|
| **Size distribution** | Per API, each load |
| **Crush test** | Per load/source |
| **Turbidity** | Fines content |
| **Moisture** | Each load |

### Equipment QC

| Check | Frequency |
|-------|-----------|
| **Pressure test iron** | Before job, after connections |
| **Pump function** | Pre-job, continuous |
| **Blender calibration** | Pre-job |
| **Density meter** | Pre-job |

---

## Frac Operations Checklist

### Pre-Stage
- [ ] Stage design confirmed
- [ ] Perforations completed
- [ ] Wellbore prepared
- [ ] Iron tested
- [ ] Fluid/proppant ready
- [ ] All personnel in position

### During Stage
- [ ] Pressure monitored continuously
- [ ] Rate maintained per design
- [ ] Proppant schedule followed
- [ ] Real-time analysis ongoing
- [ ] Safety monitoring active

### Post-Stage
- [ ] Flush confirmed
- [ ] ISIP recorded
- [ ] Stage documentation complete
- [ ] Next stage prep initiated
- [ ] Any issues logged
