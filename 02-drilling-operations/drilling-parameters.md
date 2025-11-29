# Drilling Parameters

## Overview

Optimizing drilling parameters maximizes rate of penetration (ROP) while maintaining hole quality and equipment integrity.

---

## Key Parameters

### Weight on Bit (WOB)

**Definition**: Axial force applied to drill bit

**Typical Ranges:**
| Bit Type | WOB (1000 lbs/inch) |
|----------|---------------------|
| PDC | 1-4 |
| Roller Cone | 2-6 |
| Diamond | 1-3 |

**Guidelines:**
- Start low, increase gradually
- Monitor for bit damage (torque spikes)
- Reduce in hard stringers
- Adjust for deviation control

### Rotary Speed (RPM)

**Definition**: Bit rotation rate

**Typical Ranges:**
| Bit Type | RPM |
|----------|-----|
| PDC | 80-200 |
| Roller Cone | 40-120 |
| Diamond | 150-400 |
| Motor drilling | 0-40 (surface) + motor |

**Guidelines:**
- Higher RPM in soft formations
- Lower RPM to control deviation
- Balance with WOB for ROP
- Monitor for vibration

### Flow Rate (GPM)

**Definition**: Mud circulation rate

**Requirements:**
1. Annular velocity for cuttings transport
2. Bit hydraulics for ROP
3. MWD signal transmission
4. Cooling/lubrication

**Minimum Annular Velocity:**
| Hole Section | Min AV (ft/min) |
|--------------|-----------------|
| Vertical | 100-150 |
| Deviated | 150-200 |
| Horizontal | 150-250 |

### Pump Pressure

**Components:**
```
Surface Pressure = 
  Bit Pressure Drop +
  Drill String Pressure Loss +
  Annular Pressure Loss +
  Surface Equipment Loss
```

**Typical Ranges:**
- Surface hole: 1,000-2,000 psi
- Intermediate: 2,000-3,500 psi
- Deep/horizontal: 3,000-5,000 psi

---

## Drilling Optimization

### ROP Optimization

**Drilloff Tests:**
1. Set constant RPM
2. Apply high WOB
3. Allow bit to drill off
4. Record ROP vs. WOB
5. Identify optimal WOB
6. Repeat for RPM optimization

**Typical Response Curves:**

| Formation | WOB Response | RPM Response |
|-----------|--------------|--------------|
| Soft | Linear | Linear |
| Medium | Diminishing | Linear to peak |
| Hard | Peak then decline | Peak then decline |

### Founder Point

**Definition**: WOB beyond which ROP decreases

**Causes:**
- Bit balling
- Bearing failure
- Cutter damage
- Drilling inefficiency

**Response:**
- Reduce WOB slightly below founder
- Consider bit change if recurring

### D-Exponent

**Calculation:**
```
d = log(ROP / 60N) / log(12WOB / 10⁶D)

Where:
ROP = ft/hr
N = RPM
WOB = lbs
D = bit diameter (inches)
```

**Corrected D-Exponent:**
```
dc = d × (NMW / AMW)

Where:
NMW = Normal mud weight (8.5 ppg)
AMW = Actual mud weight
```

**Interpretation:**
- Increasing dc: Normal compaction
- Decreasing dc: Possible overpressure
- Sudden change: Formation change or pressure transition

---

## Vibration Management

### Vibration Types

| Type | Frequency | Cause | Indicators |
|------|-----------|-------|------------|
| Axial | 1-10 Hz | Bit bounce | Weight variation |
| Lateral | 0.5-5 Hz | Mass imbalance | Whirl patterns |
| Torsional | 0.1-2 Hz | Stick-slip | Torque fluctuation |

### Stick-Slip

**Indicators:**
- Torque fluctuation at surface
- RPM variation
- Poor ROP
- Bit damage

**Mitigation:**
- Increase surface RPM
- Decrease WOB
- Improve lubricity
- Use anti-stick-slip systems
- Modify BHA

### Bit Whirl

**Indicators:**
- Erratic ROP
- Unusual cutter wear
- Gauge wear
- Irregular hole (caliper)

**Mitigation:**
- Increase WOB
- Decrease RPM
- Use stabilizers near bit
- Anti-whirl bit design

---

## Hole Cleaning

### Cuttings Transport

**Annular Velocity Calculation:**
```
AV (ft/min) = (24.5 × Q) / (Dh² - Dp²)

Where:
Q = Flow rate (GPM)
Dh = Hole diameter (in)
Dp = Pipe OD (in)
```

### Transport Ratio

**Definition**: Cuttings velocity / Mud velocity

**Target:** > 0.5 in vertical, higher in deviated

**Factors:**
- Mud rheology (YP, PV)
- Annular velocity
- Cuttings size and density
- Hole inclination

### High-Angle Hole Cleaning

**Critical Angles:** 30-60° inclination

**Challenges:**
- Cuttings beds on low side
- Mechanical sticking risk
- ECD management

**Best Practices:**
- Higher flow rates
- Increased rheology (YP)
- Pipe rotation (>80 RPM)
- Regular sweeps
- Tripping protocols (wiper trips)

---

## ECD Management

### ECD Calculation

```
ECD = MW + (APL / (0.052 × TVD))

Where:
APL = Annular Pressure Loss (psi)
MW = Mud weight (ppg)
TVD = True vertical depth (ft)
```

### ECD Control Methods

| Issue | Solution |
|-------|----------|
| High ECD | Reduce flow rate, thin mud |
| Surge | Control trip speed |
| Swab | Control pull speed |
| Losses | Reduce ECD, LCM |

### Surge and Swab

**Surge** (running in):
- Increases bottom hole pressure
- Can cause losses
- Control by running speed

**Swab** (pulling out):
- Decreases bottom hole pressure
- Can cause kick
- Control by pulling speed

**Estimation:**
```
Surge/Swab = f(pipe velocity, mud properties, annular clearance)
```

---

## Torque and Drag

### Sources of Torque

| Source | Mitigation |
|--------|------------|
| Friction | Lubricity, rotation |
| Differential sticking | MW management |
| Doglegs | Smooth wellpath |
| Hole condition | Reaming, cleaning |

### Drag Monitoring

**Normal Trends:**
- Gradual increase with depth
- Predictable based on model
- Consistent patterns

**Abnormal Indicators:**
- Sudden increase
- Higher than model
- Asymmetric (pick-up vs. slack-off)

### Mitigation

- Lubricity additives
- Drill pipe rotation
- Hole conditioning
- BHA modification
- Wellpath optimization

---

## Drilling Efficiency Metrics

### Mechanical Specific Energy (MSE)

**Calculation:**
```
MSE = (480 × T × N) / (D² × ROP) + (4 × WOB) / (π × D²)

Where:
MSE = psi
T = Torque (ft-lbs)
N = RPM
D = Bit diameter (in)
ROP = ft/hr
WOB = lbs
```

**Interpretation:**
- MSE close to rock strength = efficient
- MSE >> rock strength = inefficient (dysfunction)
- Target: Minimize MSE while maintaining ROP

### Connection Time

**Target:** 8-12 minutes per connection

**Components:**
- Pipe handling
- Making connection
- Break circulation
- Resume drilling

**Reduction Strategies:**
- Automated pipe handling
- Top drive systems
- Continuous circulation valves
- Practice and technique

### Flat Time

**Definition**: Non-drilling time

**Reduction Focus:**
- Trip time
- Connection time
- Survey time
- Equipment repair

---

## Parameter Recording

### Minimum Data Requirements

| Parameter | Frequency |
|-----------|-----------|
| WOB | Continuous |
| RPM | Continuous |
| Torque | Continuous |
| ROP | Continuous |
| Flow rate | Continuous |
| Pump pressure | Continuous |
| Pit volume | Continuous |

### Depth-Based Recording

- All parameters by depth
- Formation changes
- Drilling breaks
- Parameter changes

---

## Related Documents

- [Mud Programs](./mud-programs.md)
- [Bit Selection](./bit-selection.md)
- [Directional Planning](../04-directional-drilling/directional-planning.md)
- [Drilling Calculations](../10-calculation-sheets/drilling-calculations.md)
- [Hydraulics Calculations](../10-calculation-sheets/hydraulics-calculations.md)
