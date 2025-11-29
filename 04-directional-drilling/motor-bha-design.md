# Motor & BHA Design

## Overview

The Bottom Hole Assembly (BHA) is the key to successful directional drilling. Proper motor and BHA design enables precise trajectory control while maintaining drilling efficiency.

---

## Positive Displacement Motors (PDM)

### Motor Components

```
┌──────────────────────────────────────────────────────────────┐
│                    POSITIVE DISPLACEMENT MOTOR               │
├──────────────────────────────────────────────────────────────┤
│                                                              │
│  ┌──────────────┐                                            │
│  │  Dump Sub    │ ← Allows filling/draining drill string    │
│  └──────┬───────┘                                            │
│         │                                                    │
│  ┌──────▼───────┐                                            │
│  │  Top Sub /   │ ← Adjustable bend housing (0-3°)          │
│  │  Bend Housing│                                            │
│  └──────┬───────┘                                            │
│         │                                                    │
│  ┌──────▼───────┐                                            │
│  │  Power       │ ← Stator (rubber) and Rotor (steel)       │
│  │  Section     │   Converts hydraulic to mechanical power  │
│  └──────┬───────┘                                            │
│         │                                                    │
│  ┌──────▼───────┐                                            │
│  │  Transmission│ ← Connects eccentric rotor to concentric  │
│  │  /CV Joint   │   output shaft                            │
│  └──────┬───────┘                                            │
│         │                                                    │
│  ┌──────▼───────┐                                            │
│  │  Bearing     │ ← Supports axial and radial loads         │
│  │  Section     │   Contains thrust and radial bearings     │
│  └──────┬───────┘                                            │
│         │                                                    │
│  ┌──────▼───────┐                                            │
│  │  Bit Box     │ ← Connection to bit                       │
│  └──────────────┘                                            │
│                                                              │
└──────────────────────────────────────────────────────────────┘
```

### Motor Configurations (Lobe Ratio)

| Configuration | Lobe Ratio | Speed | Torque | Application |
|---------------|------------|-------|--------|-------------|
| **High speed** | 1:2, 2:3 | High | Low | Soft formations |
| **Medium** | 3:4, 4:5 | Medium | Medium | General purpose |
| **High torque** | 5:6, 7:8 | Low | High | Hard formations |
| **Ultra-high torque** | 9:10+ | Very low | Very high | Very hard, high WOB |

### Motor Specifications by Size

| Motor OD | Hole Size | Flow Range (gpm) | Max WOB (klb) | RPM Range |
|----------|-----------|------------------|---------------|-----------|
| 4-3/4" | 6-1/8" - 6-1/2" | 150-300 | 15-25 | 80-250 |
| 6-1/2" | 7-7/8" - 8-1/2" | 300-500 | 25-40 | 80-200 |
| 6-3/4" | 8-1/2" - 8-3/4" | 350-550 | 30-50 | 70-180 |
| 8" | 9-7/8" - 10-5/8" | 450-750 | 40-60 | 60-150 |
| 9-5/8" | 12-1/4" | 600-1000 | 50-80 | 50-120 |

### Bend Settings

| Bend Angle | Build Rate Capability | Application |
|------------|----------------------|-------------|
| 0° | 0-1°/100 ft | Rotary drilling, hold angle |
| 0.5° | 1-2°/100 ft | Low build, tangent |
| 1.0° | 2-4°/100 ft | Medium build |
| 1.5° | 4-6°/100 ft | Medium-high build |
| 2.0° | 6-10°/100 ft | High build, curve drilling |
| 2.5° | 10-14°/100 ft | Short radius |
| 3.0° | 14-18°/100 ft | Ultra-short radius |

---

## Rotary Steerable Systems (RSS)

### RSS Types

| Type | Mechanism | Advantages |
|------|-----------|------------|
| **Push-the-bit** | Pads push against borehole | Smooth hole, consistent build |
| **Point-the-bit** | Internal shaft deflection | Better in hard rock, precise |
| **Hybrid** | Combined mechanisms | Versatile, wide application |

### RSS vs Motor Comparison

| Factor | Motor | RSS |
|--------|-------|-----|
| **ROP sliding** | Reduced | N/A (continuous rotation) |
| **Hole quality** | Spiral possible | Smooth, round hole |
| **Build rate** | Up to 18°/100 ft | Typically 8-12°/100 ft max |
| **Cost** | Lower | Higher (2-3x day rate) |
| **Reliability** | Good | Generally good, more complex |
| **Hole cleaning** | Moderate | Excellent (continuous rotation) |

### When to Use RSS

- Extended reach wells (torque/drag critical)
- Horizontal sections requiring good hole quality
- High ROP formations where sliding ROP loss is significant
- Wells requiring continuous rotation for hole cleaning
- Tight anti-collision situations requiring precise steering

---

## BHA Components

### Standard Directional BHA Components

```
From Bit to Surface:
┌─────────────────────────────────────────────────────────────┐
│                                                             │
│   BIT                                                       │
│    │                                                        │
│   BIT SUB (if needed for connection)                        │
│    │                                                        │
│   MOTOR (PDM with bent housing)                             │
│    │                                                        │
│   FLOAT SUB                                                 │
│    │                                                        │
│   MWD/LWD TOOLS                                             │
│    │                                                        │
│   NMDC (Non-Magnetic Drill Collar)                          │
│    │                                                        │
│   STABILIZER (string stabilizer)                            │
│    │                                                        │
│   DRILL COLLARS                                             │
│    │                                                        │
│   JAR                                                       │
│    │                                                        │
│   HWDP (Heavy Weight Drill Pipe)                            │
│    │                                                        │
│   DRILL PIPE                                                │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

### Stabilizer Functions

| Position | Function |
|----------|----------|
| **Near-bit** | Controls bit side force, affects build/drop |
| **String stabilizer** | Controls BHA tendency, reduces vibration |
| **Reamer** | Maintains hole gauge, cleans hole |

### Stabilizer Types

| Type | Description | Application |
|------|-------------|-------------|
| **Integral blade** | Blades machined into body | General purpose |
| **Sleeve** | Replaceable sleeve with blades | Wear areas |
| **Non-rotating** | Sleeve rotates on bearing | Casing wear reduction |
| **Adjustable** | Blades can be extended/retracted | Flexibility |

### Stabilizer Gauge

| Gauge | Definition | Application |
|-------|------------|-------------|
| **Full gauge** | Hole size - 1/8" to 1/4" | Standard drilling |
| **Under gauge** | Hole size - 1/2" to 1" | Reduce side force |
| **Over gauge** | Should not exceed hole size | Not recommended |

---

## BHA Design for Directional Control

### Building Angle (Increasing Inclination)

**Configuration**:
- Bent motor (1.5-2.5° bend)
- Near-bit stabilizer: Under gauge or none
- String stabilizer: Full gauge, positioned far from bit

**Mechanism**: Bent motor points bit in build direction; lack of near-bit stabilizer allows bit to side-cut

### Dropping Angle (Decreasing Inclination)

**Configuration**:
- Straight motor or low bend (0-0.5°)
- Near-bit stabilizer: Full gauge
- String stabilizer: Under gauge or none

**Mechanism**: Pendulum effect - gravity causes BHA to drop; near-bit stabilizer fulcrum point

### Holding Angle (Maintaining Inclination)

**Configuration**:
- Locked or low bend motor
- Near-bit stabilizer: Full gauge
- String stabilizer: Full gauge
- Balanced spacing

**Mechanism**: Packed hole assembly prevents deviation

### Turn Left/Right (Azimuth Control)

**Motor BHA**:
- Slide with toolface oriented to desired direction
- Toolface 90° right = turn right
- Toolface 90° left = turn left
- Reactive torque can affect toolface

**RSS**:
- Set target inclination and azimuth
- System steers automatically

---

## Slide vs Rotate Drilling

### Sliding (Oriented Drilling)

| Aspect | Consideration |
|--------|---------------|
| **When** | Building/dropping angle, turns |
| **ROP impact** | 30-70% of rotary ROP |
| **Hole quality** | Can create ledges, spiraling |
| **Stick-slip** | More common |
| **Hole cleaning** | Reduced efficiency |

**Toolface Orientation**:
```
             0° (High Side)
              │
              │
    270° ─────┼───── 90°
   (Left)     │     (Right)
              │
             180°
          (Low Side)

Build = 0° (high side)
Drop = 180° (low side)
Turn Right = 90°
Turn Left = 270°
```

### Rotating (Rotary Drilling)

| Aspect | Consideration |
|--------|---------------|
| **When** | Holding angle, lateral drilling |
| **ROP** | Maximum for BHA configuration |
| **Hole quality** | Smooth, round hole |
| **Trajectory** | Natural walk of BHA |
| **Hole cleaning** | Maximum efficiency |

### Slide/Rotate Ratio Optimization

| Objective | Slide % | Rotate % |
|-----------|---------|----------|
| Aggressive build | 80-100% | 0-20% |
| Moderate build | 50-70% | 30-50% |
| Minor correction | 20-40% | 60-80% |
| Hold angle | 0-10% | 90-100% |

---

## BHA Performance Prediction

### Factors Affecting Directional Tendency

| Factor | Effect |
|--------|--------|
| **Motor bend angle** | Higher bend = higher build rate |
| **Bit type** | Aggressive bits build faster |
| **WOB** | Higher WOB can increase build |
| **Formation dip** | Bit walks up-dip |
| **Stabilizer placement** | Controls fulcrum point |
| **Hole size** | Larger hole = more side-cutting |

### Calculating Theoretical Build Rate

**Approximate Formula**:
```
Build Rate (°/100 ft) ≈ Bend Angle (°) × 3 to 4

Example: 1.5° bend
Build Rate ≈ 1.5 × 3.5 = 5.25°/100 ft (approximate)
```

**Note**: Actual build rates vary significantly based on formation, WOB, and other factors. Use offset data and DD recommendations.

---

## BHA Troubleshooting

### Common Problems and Solutions

| Problem | Possible Causes | Solutions |
|---------|-----------------|-----------|
| **Can't build angle** | Bend too low, full gauge near-bit | Increase bend, remove near-bit stabilizer |
| **Building too fast** | Bend too high, aggressive bit | Reduce bend, change bit, increase rotation |
| **Can't drop angle** | No pendulum effect, under gauge | Add near-bit stabilizer, rotate |
| **Azimuth walking** | Formation dip, bit walk | Adjust toolface, plan for walk |
| **Toolface won't hold** | Reactive torque, differential sticking | Adjust WOB, lubricate mud |
| **High motor stalls** | Excessive WOB, tight hole | Reduce WOB, ream hole |
| **Low ROP sliding** | Friction, weight transfer | Jarring action, lubricants, lighter WOB |

### BHA Selection Checklist

- [ ] Motor size appropriate for hole size
- [ ] Bend angle matches required build rate
- [ ] Motor lobe configuration matches formation
- [ ] NMDC length adequate for inclination
- [ ] MWD/LWD tools compatible with motor
- [ ] Stabilizer placement optimized for objective
- [ ] Float equipment included
- [ ] All connections verified
- [ ] Backup plan if primary BHA fails
