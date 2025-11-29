# Bit Selection

## Overview

Proper bit selection maximizes drilling efficiency and minimizes overall drilling costs. Selection depends on formation characteristics, well profile, and operational constraints.

---

## Bit Types

### Roller Cone Bits

**Types:**
| Type | Teeth | Application |
|------|-------|-------------|
| Mill Tooth | Steel teeth | Soft formations |
| Insert | Tungsten carbide | Medium to hard |
| TCI | Sealed bearing | Extended runs |

**Characteristics:**
- Crushing/chipping action
- Tolerance to formation changes
- Good in abrasive formations
- Lower ROP than PDC in soft

**Selection Guide:**
| IADC Code | Formation | Typical Formations |
|-----------|-----------|-------------------|
| 1-1-1 to 1-2-1 | Very soft | Unconsolidated |
| 2-1-1 to 2-3-1 | Soft | Shales, soft limestone |
| 3-1-1 to 3-4-1 | Medium | Sandy shales |
| 4-1-1 to 4-4-1 | Medium-hard | Limestone, dolomite |
| 5-1-1 to 7-4-1 | Hard | Hard limestone, granite |
| 8-1-1 to 8-4-1 | Very hard | Chert, hard quartzite |

### PDC Bits

**Cutter Types:**
| Type | Size | Application |
|------|------|-------------|
| Standard | 13mm | General purpose |
| Premium | 16mm | Soft-medium |
| Large | 19mm | Soft formations |
| Shaped | Various | Hard formations |

**Blade Configurations:**
| Blades | Application |
|--------|-------------|
| 4-5 | Soft formations, high ROP |
| 6-7 | Medium formations, balanced |
| 8+ | Hard formations, aggressive |

**Bit Profiles:**
| Profile | Description | Use |
|---------|-------------|-----|
| Flat | Long gauge, flat face | Vertical, sliding |
| Parabolic | Moderate dome | General purpose |
| Deep cone | High dome | Steering, directional |

### Diamond Bits

**Types:**
- Natural diamond
- Thermally stable polycrystalline (TSP)
- Impregnated diamond

**Applications:**
- Very hard, abrasive formations
- Coring operations
- Specialized applications

### Hybrid Bits

**Combination designs:**
- PDC + roller cone elements
- Best of both technologies
- Specific applications

---

## Selection Criteria

### Formation Properties

| Property | Bit Choice Impact |
|----------|-------------------|
| Hardness | Cutter/insert type |
| Abrasiveness | Wear resistance |
| Plasticity | Cutter design |
| Drillability | Aggressiveness |
| Interbedding | Versatility |

### Operational Requirements

| Requirement | Consideration |
|-------------|---------------|
| ROP target | Aggressiveness |
| Directional | Steerability |
| Extended reach | Durability |
| Motor drilling | Profile, size |
| Hole cleaning | Junk slot area |

### Historical Data

**Offset Well Analysis:**
- Bit types used
- Footage drilled
- Hours on bit
- Dull condition
- Problems encountered

---

## Bit Sizing

### Standard Bit Sizes

| Hole Size | Casing OD | Clearance |
|-----------|-----------|-----------|
| 26" | 20" | 3" |
| 17-1/2" | 13-3/8" | 2-1/16" |
| 12-1/4" | 9-5/8" | 1-5/16" |
| 8-1/2" | 7" | 3/4" |
| 6-1/8" | 4-1/2" | 13/16" |

### Clearance Requirements

**Minimum Clearances:**
- Casing drift: 0.75" larger than bit
- Bit to casing: 0.75" clearance
- Consider tool joints and stabilizers

---

## PDC Bit Selection Guide

### By Formation

| Formation | Blade Count | Cutter Size | Profile |
|-----------|-------------|-------------|---------|
| Shale, soft | 4-5 | 16-19mm | Flat-parabolic |
| Sand/shale | 5-6 | 13-16mm | Parabolic |
| Limestone | 6-7 | 13mm | Parabolic |
| Dolomite | 7-8 | 13mm | Deep cone |
| Hard/abrasive | 8+ | 13mm | Deep cone |

### Directional Considerations

**Sliding Operations:**
- Shorter gauge
- Lower blade count
- Active gauge cutters

**Rotary Steerable:**
- Stable design
- Balanced forces
- Consistent response

---

## Bit Hydraulics

### Nozzle Selection

**Total Flow Area (TFA):**
```
TFA = Σ (π × d² / 4) / 1024

Where:
d = nozzle diameter (32nds of inch)
TFA = square inches
```

**Hydraulic Horsepower:**
```
HHP = (P × Q) / 1714

Where:
P = Pressure drop across bit (psi)
Q = Flow rate (GPM)
```

**Impact Force:**
```
IF = Q × √(MW × ΔP) / 58

Where:
IF = lbs
Q = GPM
MW = ppg
ΔP = psi across bit
```

**Nozzle Velocity:**
```
Vn = Q / (3.117 × TFA)

Where:
Vn = ft/sec
Q = GPM
TFA = in²
```

### Optimization Guidelines

| Parameter | Target |
|-----------|--------|
| Bit pressure drop | 50-65% of SPP |
| Nozzle velocity | 250-450 ft/sec |
| HSI | 2-5 HP/in² |
| Impact force | Maximize for cleaning |

---

## Bit Dull Grading

### IADC Dull Grading System

**Format:** I - O - D - L - B - G - O - R

| Position | Code | Description |
|----------|------|-------------|
| I | 0-8 | Inner rows wear |
| O | 0-8 | Outer rows wear |
| D | Code | Dull characteristic |
| L | Code | Location |
| B | Code | Bearing/seal |
| G | Code | Gauge condition |
| O | Code | Other dull characteristic |
| R | Code | Reason pulled |

### Dull Characteristics (D)

| Code | Description |
|------|-------------|
| BC | Broken cone |
| BT | Broken teeth/cutters |
| BU | Balled up |
| CC | Cracked cone |
| CD | Cone dragged |
| CI | Cone interference |
| CR | Cored |
| CT | Chipped teeth/cutters |
| ER | Erosion |
| FC | Flat crested wear |
| HC | Heat checking |
| JD | Junk damage |
| LC | Lost cone |
| LN | Lost nozzle |
| LT | Lost teeth/cutters |
| OC | Off-center wear |
| PB | Pinched bit |
| PN | Plugged nozzle |
| RG | Rounded gauge |
| RO | Ring out |
| SD | Shirttail damage |
| SS | Self-sharpening wear |
| TR | Tracking |
| WO | Washed out |
| WT | Worn teeth/cutters |

### Reason Pulled (R)

| Code | Description |
|------|-------------|
| BHA | Change BHA |
| CM | Condition mud |
| CP | Core point |
| DMF | Downhole motor failure |
| DP | Drill plug |
| DSF | Drill stem failure |
| DST | Drill stem test |
| DTF | Downhole tool failure |
| FM | Formation change |
| HP | Hole problems |
| HR | Hours |
| LOG | Run logs |
| PP | Pump pressure |
| PR | Penetration rate |
| RIG | Rig repair |
| TD | Total depth |
| TQ | Torque |
| TW | Twist off |
| WC | Weather/conditions |
| WO | Washout |

---

## Bit Performance Analysis

### Cost per Foot

```
CPF = (Bc + Rc × (Tb + Tt)) / F

Where:
CPF = Cost per foot ($)
Bc = Bit cost ($)
Rc = Rig cost ($/hr)
Tb = Time on bit (hrs)
Tt = Trip time (hrs)
F = Footage (ft)
```

### Bit Selection Optimization

**Goal:** Minimize overall cost per foot

**Balance:**
- Higher bit cost may reduce rig time
- Longer runs reduce trip time
- ROP impacts rig time

### Performance Metrics

| Metric | Calculation | Target |
|--------|-------------|--------|
| Average ROP | Footage / Hours | Formation dependent |
| Cost per foot | See formula | Minimize |
| Run length | Footage | Maximize |
| Trips to TD | Count | Minimize |

---

## Bit Operating Parameters

### PDC Guidelines

| Formation | WOB (klbs/in) | RPM | Notes |
|-----------|---------------|-----|-------|
| Soft | 1-2 | 150-250 | High ROP, watch balling |
| Medium | 2-3 | 100-150 | Balance WOB/RPM |
| Hard | 3-4 | 80-120 | Control vibration |

### Roller Cone Guidelines

| Formation | WOB (klbs/in) | RPM | Notes |
|-----------|---------------|-----|-------|
| Soft | 3-4 | 100-150 | Watch bearing life |
| Medium | 4-5 | 80-120 | Optimize WOB |
| Hard | 5-6 | 60-100 | Monitor for damage |

---

## Common Problems

### PDC Issues

| Problem | Cause | Solution |
|---------|-------|----------|
| Balling | Soft/sticky formations | Increase flow, reduce WOB |
| Chipping | Hard stringers | Reduce WOB, RPM |
| Ring out | Abrasion | Harder cutters |
| Tracking | Low WOB | Increase WOB |

### Roller Cone Issues

| Problem | Cause | Solution |
|---------|-------|----------|
| Cone loss | Bearing failure | Reduce parameters |
| Tooth wear | Abrasion | Harder inserts |
| Gauge wear | Abrasive formation | Gauge protection |
| Tracking | Worn teeth | Replace bit |

---

## Related Documents

- [Drilling Parameters](./drilling-parameters.md)
- [Hydraulics Calculations](../10-calculation-sheets/hydraulics-calculations.md)
- [Drilling Problems Decision Trees](../09-decision-trees/drilling-problems.md)
