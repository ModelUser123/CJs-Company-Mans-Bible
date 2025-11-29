# Artificial Lift

## Overview

Artificial lift provides additional energy to move reservoir fluids to surface when natural reservoir pressure is insufficient. Selection of the optimal lift method depends on well conditions, production characteristics, and economics.

---

## Why Artificial Lift?

### When Required

| Situation | Indicator |
|-----------|-----------|
| **Depleted reservoir** | Pressure declined |
| **Low initial pressure** | Never flowed naturally |
| **High water cut** | Heavy fluid column |
| **Viscous crude** | High friction losses |
| **Deep well** | Long fluid column |
| **Low productivity** | Low inflow |

### Lift Methods Overview

| Method | Volume Capability | Depth Limit | Application |
|--------|-------------------|-------------|-------------|
| **Rod pump** | Low-moderate | 16,000 ft | Onshore, all types |
| **ESP** | High | 15,000 ft | High volume |
| **Gas lift** | Moderate-high | Deep | Offshore, deviated |
| **PCP** | Low-moderate | 6,000 ft | Heavy oil, sand |
| **Plunger** | Low | 15,000 ft | Low rate gas wells |
| **Jet pump** | Moderate | 20,000 ft | Remote, flexibility |

---

## Rod Pump (Beam Pump)

### System Components

```
┌─────────────────────────────────────────────────────┐
│                   ROD PUMP SYSTEM                   │
├─────────────────────────────────────────────────────┤
│                                                     │
│   ┌─────────────┐                                   │
│   │   Motor     │ ← Prime mover                    │
│   └──────┬──────┘                                   │
│          │                                          │
│   ┌──────▼──────┐                                   │
│   │  Gear Box   │ ← Speed reduction                │
│   └──────┬──────┘                                   │
│          │                                          │
│   ┌──────▼──────────────────┐                       │
│   │  Pumping Unit (beam)    │ ← Surface equipment  │
│   │  ↑ ↓  ↑ ↓  ↑ ↓         │                       │
│   └──────┬──────────────────┘                       │
│          │ Polished rod                             │
│          │                                          │
│   ───────┼─────── Stuffing box                     │
│          │                                          │
│   ┌──────▼──────┐                                   │
│   │  Sucker     │ ← Rod string                     │
│   │   Rods      │                                   │
│   └──────┬──────┘                                   │
│          │                                          │
│   ┌──────▼──────┐                                   │
│   │  Downhole   │ ← Traveling valve, barrel,      │
│   │   Pump      │   standing valve                 │
│   └─────────────┘                                   │
│                                                     │
└─────────────────────────────────────────────────────┘
```

### Rod Pump Advantages/Disadvantages

| Advantages | Disadvantages |
|------------|---------------|
| Low capital cost | Limited to vertical/slight deviation |
| Familiar technology | Volume limited |
| Easy to repair | Surface footprint |
| Long run life | Rod failures possible |
| Flexible rates | Not for high GOR |

### Design Parameters

| Parameter | Typical Range |
|-----------|---------------|
| **Stroke length** | 24-366 inches |
| **Pump speed** | 4-15 SPM |
| **Pump bore** | 1.06-3.75 inches |
| **Rod size** | 5/8" - 1-1/8" |

### Pump Displacement

```
PD (bbl/day) = 0.1166 × D² × S × N × E

Where:
D = Pump diameter (inches)
S = Stroke length (inches)
N = Strokes per minute
E = Volumetric efficiency (typically 0.7-0.85)
```

---

## Electric Submersible Pump (ESP)

### System Components

```
┌─────────────────────────────────────────────────────┐
│                     ESP SYSTEM                      │
├─────────────────────────────────────────────────────┤
│                                                     │
│   Surface ─────────────────────────────────        │
│   ┌─────────────┐   ┌─────────────┐                │
│   │ Transformer │   │   VSD/      │                │
│   │             │   │ Switchgear  │                │
│   └──────┬──────┘   └──────┬──────┘                │
│          └────────┬────────┘                        │
│                   │ Power cable                     │
│                   │                                 │
│   Downhole ───────┼─────────────────────────       │
│                   │                                 │
│   ┌───────────────▼───────────────┐                │
│   │  Motor (3-phase induction)    │                │
│   └───────────────┬───────────────┘                │
│   ┌───────────────▼───────────────┐                │
│   │  Seal Section (Protector)     │                │
│   └───────────────┬───────────────┘                │
│   ┌───────────────▼───────────────┐                │
│   │  Gas Separator (if needed)    │                │
│   └───────────────┬───────────────┘                │
│   ┌───────────────▼───────────────┐                │
│   │  Pump (multistage centrifugal)│                │
│   └───────────────────────────────┘                │
│                                                     │
└─────────────────────────────────────────────────────┘
```

### ESP Advantages/Disadvantages

| Advantages | Disadvantages |
|------------|---------------|
| High volume capability | High power cost |
| Good for deviated wells | Pulls for repair |
| Quiet, compact | Gas handling limited |
| Wide operating range | High capital cost |
| Can be remotely controlled | Heat from motor |

### ESP Operating Range

| Parameter | Range |
|-----------|-------|
| **Rate** | 200-30,000+ bbl/day |
| **Depth** | To 15,000 ft |
| **Temperature** | To 400°F (special) |
| **Horsepower** | 10-1,500 HP |

### Key Performance Curves

**Pump Curve**: Head vs. Flow at constant speed
- Downward sloping
- Efficiency curve overlaid
- Operating point where system and pump curves intersect

---

## Gas Lift

### System Concept

```
Gas injection at surface
         │
         ▼
    ┌─────────┐
    │   │     │
    │   │     │ ← Injected gas in annulus
    │   │     │
    │   │◄────┤ ← Gas lift valve (GLV)
    │   │     │   Injects gas into tubing
    │   │     │
    │   │◄────┤ ← GLV
    │   │     │
    │   │◄────┤ ← Operating valve
    │   │     │
    │   │     │ ← Lightened fluid column
    │   │     │   flows to surface
    │   │     │
    └───┴─────┘
```

### Gas Lift Advantages/Disadvantages

| Advantages | Disadvantages |
|------------|---------------|
| Good for deviated/horizontal | Requires gas supply |
| Handles sand, solids | Compressor required |
| Surface equipment only | Less efficient at depth |
| Easy workover | Gas injection cost |
| Wide rate range | Corrosion concerns |

### Gas Lift Design Parameters

| Parameter | Consideration |
|-----------|---------------|
| **Injection depth** | Deepest practical point |
| **Injection rate** | Match to production |
| **GLI** | Gas-liquid ratio for optimization |
| **Valve spacing** | Unloading design |
| **Operating pressure** | Compressor capacity |

### Valve Types

| Type | Operation |
|------|-----------|
| **IPO (Injection Pressure Operated)** | Opens on casing pressure |
| **PPO (Production Pressure Operated)** | Opens on tubing pressure |
| **Throttling** | Continuous operation |
| **Orifice** | Fixed opening |

---

## Progressive Cavity Pump (PCP)

### System Components

- Surface drive (direct or belted)
- Rod string (continuous or coupled)
- Rotor (helical steel)
- Stator (elastomer-lined)

### PCP Advantages/Disadvantages

| Advantages | Disadvantages |
|------------|---------------|
| Handles viscous crude | Depth limited |
| Good for sand | Elastomer temp limits |
| Low pulsation | Stator wear |
| Simple surface | H2S compatibility |
| Low shear | |

### PCP Applications

| Application | Why PCP |
|-------------|---------|
| Heavy oil | Low shear, handles viscosity |
| Sand producers | Tolerates sand |
| Low rate wells | Efficient at low rates |
| SAGD | Handles high temperature with correct elastomer |

---

## Plunger Lift

### Concept

- Free piston travels in tubing
- Well builds pressure with plunger at bottom
- Plunger rises with gas expansion
- Lifts liquid above plunger
- Cycles repeat

### Plunger Lift Applications

| Application | Suitability |
|-------------|-------------|
| **Low rate gas wells** | Ideal |
| **Liquid loading** | Removes liquids |
| **Low OPEX required** | Minimal equipment |
| **Remote locations** | Simple, reliable |

### Requirements

- Adequate gas production
- GLR typically > 300 scf/bbl
- Tubing in good condition
- Wellhead with lubricator

---

## Lift Method Selection

### Selection Criteria

| Factor | Consideration |
|--------|---------------|
| **Production rate** | Volume required |
| **Depth** | Lift method limits |
| **Well deviation** | Some methods limited |
| **GOR** | Gas handling capability |
| **Fluid properties** | Viscosity, sand, H2S |
| **Power availability** | Electric, gas, solar |
| **Capital budget** | Initial investment |
| **Operating cost** | Long-term economics |

### Selection Matrix

| Condition | Best Methods |
|-----------|--------------|
| High rate, any deviation | ESP, gas lift |
| Low rate, low deviation | Rod pump |
| Heavy oil | PCP, rod pump |
| High GOR | Gas lift |
| Remote, no power | Gas lift, solar rod pump |
| Deep well | Gas lift, jet pump |
| Sand production | PCP, jet pump |

### Selection Flowchart

```
              Start
                │
                ▼
         Rate > 1000 bpd?
            /       \
          Yes        No
           │          │
           ▼          ▼
    Deviation    Rate > 200?
    > 60°?        /      \
     /    \     Yes       No
   Yes     No    │         │
    │       │    ▼         ▼
    ▼       ▼  Rod Pump  Plunger
   ESP    ESP    or        or
   or    or     PCP       PCP
  Gas   Gas
  Lift  Lift
```

---

## Artificial Lift Monitoring

### Key Parameters

| Parameter | Purpose |
|-----------|---------|
| **Production rate** | Performance tracking |
| **Pump intake pressure** | Pump-off, submergence |
| **Motor temperature (ESP)** | Health monitoring |
| **Amperage (ESP)** | Load, problems |
| **Dynamometer (rod)** | Pump condition |
| **Gas injection rate** | Efficiency |

### Failure Indicators

| Lift Type | Failure Signs |
|-----------|---------------|
| **Rod pump** | Fluid pound, gas interference |
| **ESP** | Low flow, high temperature, amp changes |
| **Gas lift** | Valve failure, wrong injection depth |
| **PCP** | Torque increase, rate decline |

---

## Artificial Lift Checklist

### Selection Phase
- [ ] Inflow performance analyzed
- [ ] Production forecast prepared
- [ ] Candidate methods identified
- [ ] Economics compared
- [ ] Lift method selected

### Installation Phase
- [ ] Equipment sized
- [ ] Completion compatible
- [ ] Monitoring equipment specified
- [ ] Installation procedure developed
- [ ] Optimization plan prepared

### Operation Phase
- [ ] Baseline established
- [ ] Monitoring active
- [ ] Optimization ongoing
- [ ] Failure prevention measures active
