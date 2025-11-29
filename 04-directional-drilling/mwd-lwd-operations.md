# MWD/LWD Operations

## Overview

Measurement While Drilling (MWD) and Logging While Drilling (LWD) provide real-time data from the bottomhole assembly during drilling operations. These tools are essential for directional control and formation evaluation.

---

## MWD Systems

### Core MWD Measurements

| Measurement | Sensor | Purpose |
|-------------|--------|---------|
| **Inclination** | Accelerometers (3-axis) | Wellbore angle from vertical |
| **Azimuth** | Magnetometers (3-axis) | Wellbore compass direction |
| **Toolface** | Accelerometers + Magnetometers | Bit orientation for steering |
| **Temperature** | Thermistor | Downhole conditions |
| **Gamma Ray** | Scintillation detector | Basic formation ID |
| **Shock/Vibration** | Accelerometers | Drilling dynamics |

### Toolface Types

| Type | Measurement Reference | Application |
|------|----------------------|-------------|
| **Magnetic Toolface (MTF)** | Magnetic north | Inclination < 5° |
| **Gravity Toolface (GTF)** | High side of hole | Inclination > 5° |
| **Hybrid** | Automatic switching | All inclinations |

**Toolface Display**:
```
Magnetic Toolface          Gravity Toolface
(Low Inclination)          (High Inclination)

      N (0°)                    HS (0°)
        │                          │
        │                          │
  W ────┼──── E             L ────┼──── R
        │                          │
        │                          │
      S (180°)                  LS (180°)

MTF references magnetic north    GTF references high side (top)
```

### MWD Telemetry Systems

| System | Data Rate | Depth Limit | Advantages |
|--------|-----------|-------------|------------|
| **Positive pulse** | 1-6 bps | 25,000+ ft | Most common, reliable |
| **Negative pulse** | 1-6 bps | 20,000+ ft | Less affected by gas |
| **Continuous wave** | 6-20 bps | 30,000+ ft | Higher data rate |
| **EM (Electromagnetic)** | 10-50 bps | 10,000 ft | Works in aerated fluids |
| **Wired pipe** | 1 Mbps | Unlimited | Highest data rate |

### Data Transmission Requirements

**Mud Properties for Pulse Telemetry**:

| Property | Requirement | Issue if Out of Spec |
|----------|-------------|---------------------|
| **Mud weight** | > 8.5 ppg | Signal attenuation |
| **Viscosity** | 35-50 sec/qt | Signal distortion |
| **Solids** | < 5% LGS | Valve erosion |
| **Gas** | < 5% | Signal loss |
| **LCM** | Avoid fibrous | Valve plugging |

---

## LWD Systems

### Common LWD Measurements

| Tool | Measurement | Primary Use |
|------|-------------|-------------|
| **Gamma Ray** | Natural radioactivity | Shale/sand identification |
| **Resistivity** | Formation resistivity | Fluid identification |
| **Density** | Formation bulk density | Porosity, lithology |
| **Neutron** | Hydrogen index | Porosity (gas detection) |
| **Sonic** | Acoustic velocity | Porosity, geomechanics |
| **Caliper** | Hole diameter | Hole condition |
| **Imaging** | Borehole images | Fractures, dip, faults |
| **Pressure** | Formation pressure | Pore pressure, permeability |

### LWD Tool String Configuration

```
Typical LWD/MWD BHA Configuration:

  BIT
   │
  MOTOR
   │
  GAMMA RAY (GR) ─────────────── First measurement (shallowest)
   │
  RESISTIVITY ────────────────── Multiple depths of investigation
   │
  DENSITY / NEUTRON ──────────── Porosity measurements
   │
  MWD DIRECTIONAL ────────────── Surveys
   │
  PRESSURE WHILE DRILLING ────── PWD
   │
  NMDC
   │
  DRILL COLLARS
```

### Depth of Investigation

| Tool | Depth of Investigation |
|------|----------------------|
| Gamma Ray | 6-12 inches |
| Resistivity (shallow) | 10-15 inches |
| Resistivity (medium) | 20-30 inches |
| Resistivity (deep) | 60-90 inches |
| Density | 4-6 inches |
| Neutron | 10-12 inches |

---

## Geosteering

### Geosteering Fundamentals

**Definition**: Using real-time LWD data to steer the wellbore within the target zone

**Key Objectives**:
1. Maximize reservoir exposure
2. Stay within pay zone
3. Avoid water/gas contacts
4. Optimize completion

### Geosteering Workflow

```
┌─────────────────────────────────────────────────────────────┐
│                    GEOSTEERING LOOP                         │
├─────────────────────────────────────────────────────────────┤
│                                                             │
│   ┌────────────┐     ┌────────────┐     ┌────────────┐     │
│   │  Receive   │────▶│  Interpret │────▶│   Update   │     │
│   │  LWD Data  │     │  Formation │     │   Model    │     │
│   └────────────┘     └────────────┘     └────────────┘     │
│         ▲                                      │            │
│         │                                      ▼            │
│   ┌─────┴──────┐     ┌────────────┐     ┌────────────┐     │
│   │   Execute  │◀────│  Make      │◀────│  Compare   │     │
│   │   Changes  │     │  Decision  │     │  to Plan   │     │
│   └────────────┘     └────────────┘     └────────────┘     │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

### Geosteering Indicators

| Indicator | Interpretation |
|-----------|----------------|
| **GR increasing** | Approaching shale, may need to steer down |
| **GR decreasing** | Entering cleaner sand |
| **Resistivity decreasing** | Approaching water contact or shale |
| **Resistivity increasing** | Entering hydrocarbon zone |
| **Gas increasing** | Entering gas zone or approaching gas cap |
| **ROP increasing** | Formation change (softer) |
| **ROP decreasing** | Formation change (harder) |

### Formation Dip and Steering

| Scenario | Response |
|----------|----------|
| **Drilling up-dip** | Wellbore rises through formation |
| **Drilling down-dip** | Wellbore drops through formation |
| **Crossing fault** | Sudden log response change |
| **Approaching boundary** | Gradual log response change |

---

## Real-Time Operations

### Data Display and Monitoring

**Essential Real-Time Displays**:

| Display | Contents |
|---------|----------|
| **Survey plot** | TVD vs MD, plan vs actual |
| **Stick plot** | Azimuth and inclination vs depth |
| **Log display** | GR, resistivity vs depth |
| **Drilling parameters** | WOB, RPM, torque, ROP |
| **Toolface** | Current orientation |
| **PWD** | ECD, annular pressure |

### Communication Protocol

| Party | Responsibility |
|-------|----------------|
| **Company Man** | Final drilling decisions |
| **DD/MWD Hand** | Toolface control, survey QC |
| **Geosteering** | Formation interpretation, steering recommendations |
| **Driller** | Drilling parameters execution |
| **Geologist** | Formation correlation |

### Survey Transmission Sequence

1. Drill to survey depth
2. Work pipe to clear cuttings
3. Stop rotation, pumps on
4. Wait for static conditions (30-60 seconds)
5. Transmit survey data
6. Verify QC parameters
7. Accept or reject survey
8. Resume drilling

---

## Tool Failures and Troubleshooting

### Common MWD Problems

| Problem | Symptoms | Possible Causes | Solutions |
|---------|----------|-----------------|-----------|
| **No signal** | No pulses detected | Dead battery, tool failure, mud issues | Check surface equipment, verify mud properties |
| **Weak signal** | Low pulse amplitude | Gas in mud, low mud weight, depth | Increase MW, degas mud, check receivers |
| **Erratic data** | Inconsistent readings | Vibration, interference, tool damage | Reduce parameters, check for damage |
| **Wrong data** | Values don't match offset | Calibration, magnetic interference | Re-calibrate, check NMDC |
| **Intermittent signal** | Signal comes and goes | Valve issues, power issues | May need to trip for tool |

### LWD Data Quality Issues

| Issue | Cause | Solution |
|-------|-------|----------|
| **Depth offset** | Lag time calculation | Verify lag time, adjust depth |
| **Washed out readings** | Large hole/rugose | Note on log, use image data |
| **Standoff effects** | Eccentric tool | Use azimuthal corrections |
| **Mud effects** | Heavy/conductive mud | Apply environmental corrections |
| **Statistical noise** | Low count rates, high ROP | Slow down, increase averaging |

### Emergency Procedures

**If MWD Fails**:
1. Attempt to re-establish communication
2. Pull to casing shoe if able to circulate
3. Verify well position with available data
4. Consider gyro survey if position critical
5. Trip for replacement tool if necessary
6. Re-survey from known point before continuing

---

## Tool Specifications

### Typical MWD Specifications

| Specification | Typical Value |
|---------------|---------------|
| **Operating temperature** | 300-350°F (150-175°C) |
| **Operating pressure** | 20,000-25,000 psi |
| **Battery life** | 150-250 hours |
| **Inclination accuracy** | ±0.1° |
| **Azimuth accuracy** | ±0.25° to ±1.0° |
| **Tool OD** | 4-3/4" to 9-1/2" |

### Typical LWD Specifications

| Tool | Accuracy | Resolution |
|------|----------|------------|
| **Gamma Ray** | ±5% | 1 API |
| **Resistivity** | ±5% | 0.01 ohm-m |
| **Density** | ±0.015 g/cc | 0.001 g/cc |
| **Neutron** | ±2 PU | 0.1 PU |
| **Sonic** | ±2 µs/ft | 0.5 µs/ft |

---

## Pre-Job Checklist

### MWD/LWD Preparation

- [ ] Review well program and objectives
- [ ] Verify tool ratings vs expected conditions
- [ ] Confirm tool calibration dates
- [ ] Test surface receiving equipment
- [ ] Verify communication protocol
- [ ] Establish data transmission schedule
- [ ] Confirm geosteering support availability
- [ ] Review offset well data
- [ ] Verify NMDC length adequate
- [ ] Test backup systems

### At Rig Site

- [ ] Function test all tools before running
- [ ] Verify battery status
- [ ] Record tool serial numbers
- [ ] Verify proper make-up torque
- [ ] Confirm telemetry before drilling
- [ ] Establish baseline readings
- [ ] Document all tool settings
