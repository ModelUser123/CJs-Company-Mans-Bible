# Casing Design

## Overview

Proper casing design ensures wellbore integrity, formation isolation, and safe operations throughout the life of the well.

---

## Casing Functions

### By String Type

| String | Primary Functions |
|--------|-------------------|
| Conductor | Structural support, divert drilling fluids |
| Surface | Protect fresh water, support BOP, initial pressure containment |
| Intermediate | Isolate abnormal pressures, unstable formations |
| Production | Contain production pressures, isolate zones |
| Liner | Cost-effective alternative, targeted isolation |

---

## Casing Specifications

### API Casing Grades

| Grade | Min Yield (psi) | Application |
|-------|-----------------|-------------|
| H-40 | 40,000 | Conductor |
| J-55 | 55,000 | Surface, shallow wells |
| K-55 | 55,000 | Surface, shallow wells |
| N-80 | 80,000 | Intermediate, production |
| L-80 | 80,000 | H2S service |
| C-90 | 90,000 | H2S service |
| C-95 | 95,000 | High pressure |
| T-95 | 95,000 | H2S service |
| P-110 | 110,000 | Deep, high pressure |
| Q-125 | 125,000 | HPHT |

### Common Sizes and Weights

**Surface Casing:**
| OD | Weight (ppf) | ID | Drift |
|----|--------------|-------|-------|
| 13-3/8" | 54.5-72 | 12.615-12.275 | 12.459-12.119 |
| 10-3/4" | 40.5-55.5 | 10.05-9.76 | 9.894-9.604 |

**Intermediate/Production Casing:**
| OD | Weight (ppf) | ID | Drift |
|----|--------------|-------|-------|
| 9-5/8" | 36-53.5 | 8.921-8.535 | 8.765-8.379 |
| 7" | 23-35 | 6.366-6.004 | 6.214-5.879 |
| 5-1/2" | 15.5-23 | 4.95-4.67 | 4.825-4.545 |

**Liners:**
| OD | Weight (ppf) | ID | Drift |
|----|--------------|-------|-------|
| 7" | 23-32 | 6.366-6.094 | 6.214-5.969 |
| 5" | 15-18 | 4.408-4.276 | 4.283-4.151 |
| 4-1/2" | 11.6-13.5 | 4.0-3.92 | 3.875-3.795 |

---

## Design Load Cases

### Burst Design

**Load Cases:**
1. Kick (gas to surface) - most severe
2. Pressure testing
3. Production tubing leak
4. Injection operations

**Burst Calculation:**
```
Burst Pressure = Internal Pressure - External Pressure

Design Factor: 1.1 (typical)

Required Burst Rating = Design Pressure × Design Factor
```

**Maximum Internal Pressure:**
- Gas kick: Surface pressure + gas gradient × TVD
- Test pressure: Per regulation/company policy
- Production: SITP + safety margin

### Collapse Design

**Load Cases:**
1. Cementing (wet cement outside)
2. Evacuation (lost circulation, gas migration)
3. Production drawdown

**Collapse Calculation:**
```
Collapse Pressure = External Pressure - Internal Pressure

Design Factor: 1.0-1.125 (typical)

Required Collapse Rating = Design Pressure × Design Factor
```

**Maximum External Pressure:**
- Full evacuation scenario
- Consider cement column
- Formation pressure support

### Tension Design

**Load Cases:**
1. Running string weight
2. Overpull for stuck pipe
3. Pressure testing effects

**Tension Calculation:**
```
Tension Load = String Weight + Overpull Allowance

Design Factor: 1.6-1.8 (typical)

Buoyancy Factor = 1 - (MW / 65.4)

Buoyed Weight = Air Weight × Buoyancy Factor
```

### Biaxial Loading

Combined burst/collapse with tension:
```
Effective Collapse = Published Collapse × Biaxial Factor

Biaxial Factor = √(1 - 0.75(Sa/Sy)² - 0.5(Sa/Sy))

Where:
Sa = Axial stress
Sy = Yield stress
```

---

## Connection Selection

### Connection Types

| Type | Application | Seal Mechanism |
|------|-------------|----------------|
| STC | Low pressure, shallow | Thread interference |
| LTC | Moderate pressure | Thread + shoulder |
| BTC | Higher pressure | Thread + shoulder |
| Premium | High pressure, gas | Metal-to-metal seal |

### Connection Requirements

| Environment | Recommended |
|-------------|-------------|
| Gas wells | Premium connections |
| H2S service | Premium, corrosion resistant |
| Thermal wells | Premium, thermal rated |
| High torque | Premium, high torque |
| Standard oil | STC/LTC adequate |

---

## Casing Running Procedures

### Pre-Run Checklist

```
□ Casing tally complete and verified
□ All accessories on location
□ Float equipment tested
□ Hole conditioned
□ Rig equipment inspected
□ Centralizers calculated and available
□ Mud properties correct
□ Running procedures reviewed
□ Personnel briefed
□ Weather acceptable
```

### Casing Accessories

| Accessory | Function | Location |
|-----------|----------|----------|
| Guide shoe | Guide past ledges | Bottom |
| Float shoe | Allow cement, prevent U-tube | Bottom |
| Float collar | Backup float, cement plug stop | 1-2 joints above shoe |
| Centralizers | Ensure standoff | Per program |
| Scratchers | Remove mud cake | Through pay |
| Stage collar | Multi-stage cement | Intermediate depth |

### Centralizer Placement

**Guidelines:**
- Minimum 67% standoff target
- Maximum spacing: 80-100 ft in vertical
- Reduced spacing in deviated sections
- Closer spacing through critical zones

**Standoff Calculation:**
```
Standoff % = (Pipe center to wall / Radial clearance) × 100
```

### Running Speed Limits

| Operation | Maximum Speed |
|-----------|---------------|
| Lowering | 2-3 stands/minute |
| Through tight spots | 1 stand/minute |
| Surge pressure limit | Per ECD calculation |
| Last 500 ft | Controlled, slow |

### Running Procedures

1. **Pick up shoe joint**: Verify float, fill and test
2. **Add collars**: Proper makeup torque
3. **Run in hole**: Control speed, monitor fill
4. **At shoe depth**: Circulate, condition
5. **Land casing**: Set slips, release elevators
6. **Prepare for cement**: Final circulation

---

## Casing Wear

### Causes of Casing Wear
- Drill pipe rotation
- Tripping operations
- Formation contact

### Mitigation
- Casing wear protectors
- Drill pipe protectors
- Controlled drilling parameters
- Lubricants

### Wear Monitoring
- Caliper logs
- Wear calculations
- Inspection programs

---

## Quality Control

### Inspection Requirements

**At Pipe Yard:**
```
□ Visual inspection
□ ID/OD verification
□ Wall thickness check
□ Thread inspection
□ Certification review
```

**At Rig Site:**
```
□ Drift each joint
□ Visual inspection
□ Thread protector removal/inspection
□ Tally verification
□ Damage check
```

### Makeup Torque

| Connection | Makeup Torque (ft-lb) |
|------------|----------------------|
| STC | API tables |
| LTC | API tables |
| BTC | API tables |
| Premium | Manufacturer spec |

**Torque Monitoring:**
```
□ Calibrated torque gauge
□ Torque turn monitoring
□ Shoulder makeup verification
□ Document all makeups
```

---

## Common Problems

### Tight Spots
- Symptoms: Overpull, set-down weight
- Causes: Doglegs, ledges, swelling formations
- Solutions: Ream, circulate, work pipe

### Stuck Casing
- Prevention: Hole conditioning, controlled running
- Response: Work pipe, circulate, spot pills
- Last resort: Cut and pull, sidetrack

### Fill on Bottom
- Causes: Poor circulation, unstable formations
- Prevention: Adequate circulation, proper mud
- Solutions: Circulate, use wiper trips

---

## Design Workflow

### Step-by-Step Process

1. **Determine setting depth** based on:
   - Pore pressure
   - Fracture gradient
   - Regulatory requirements

2. **Select size** based on:
   - Completion requirements
   - Previous casing constraints
   - Bit/casing clearance

3. **Determine loads** for:
   - Burst (all scenarios)
   - Collapse (all scenarios)
   - Tension (running + overpull)

4. **Select weight and grade** to:
   - Meet all load cases
   - Provide design factors
   - Optimize cost

5. **Select connections** for:
   - Pressure integrity
   - Makeup reliability
   - Service conditions

6. **Design centralizer program**

7. **Document and review**

---

## Related Documents

- [Well Design Fundamentals](../01-well-planning/well-design-fundamentals.md)
- [Cementing Operations](./cementing-operations.md)
- [Drilling Calculations](../10-calculation-sheets/drilling-calculations.md)
