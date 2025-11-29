# Wellhead & Tree

## Overview

The wellhead and tree system provides mechanical support for casing and tubing strings, pressure containment, and flow control at surface. Proper selection and installation are critical for well safety and operations.

---

## Wellhead System Components

### Basic Configuration

```
┌─────────────────────────────────────────────────────┐
│              TYPICAL WELLHEAD SYSTEM                │
├─────────────────────────────────────────────────────┤
│                                                     │
│            Christmas Tree                           │
│            ┌───────────────┐                        │
│            │   Flow Tee    │ ← To flowline         │
│            │  Master Valve │                        │
│            │  (Upper/Lower)│                        │
│            └───────┬───────┘                        │
│   Tubing Head ─────┼─────                           │
│                    │                                │
│   Casing Head ─────┼───── ← Intermediate annulus   │
│   (Spool)          │        access                 │
│                    │                                │
│   Casing Head ─────┼───── ← Surface annulus access │
│   (Starter Head)   │                                │
│                    │                                │
│   Surface ─────────┼─────                           │
│   Casing           │                                │
│                    │                                │
└─────────────────────────────────────────────────────┘
```

### Component Functions

| Component | Function |
|-----------|----------|
| **Casing head (starter)** | Support surface casing, seal |
| **Casing spool** | Hang intermediate casing, annulus access |
| **Tubing head** | Hang tubing, seal around tubing |
| **Tubing hanger** | Supports tubing weight, provides seal |
| **Christmas tree** | Flow control, pressure containment |

---

## Wellhead Ratings

### Pressure Ratings

| API Rating | Working Pressure (psi) |
|------------|----------------------|
| 2,000 | 2,000 |
| 3,000 | 3,000 |
| 5,000 | 5,000 |
| 10,000 | 10,000 |
| 15,000 | 15,000 |
| 20,000 | 20,000 |

### Material Classes

| API Class | Service |
|-----------|---------|
| **AA** | Non-corrosive (carbon steel) |
| **BB** | Non-corrosive (carbon steel) |
| **CC** | Mildly corrosive |
| **DD** | Sour service (H2S) |
| **EE** | Sour + high strength |
| **FF** | Severe sour |
| **HH** | Extreme sour |

### Temperature Ratings

| Rating | Temperature Range |
|--------|-------------------|
| **K** | -75°F to 180°F |
| **L** | -50°F to 180°F |
| **P** | -20°F to 180°F |
| **U** | 0°F to 250°F |
| **V** | 0°F to 350°F |

---

## Casing Head (Housing)

### Types

| Type | Description |
|------|-------------|
| **Slip-on weld** | Welded to casing |
| **Thread-on** | Screws onto casing |
| **Mandrel** | Integral with hanger |

### Features

| Feature | Purpose |
|---------|---------|
| **Bowl** | Receives casing hanger |
| **Pack-off** | Seals around casing |
| **Test ports** | Pressure testing |
| **Outlets** | Annular access |
| **Flange/connector** | Connect to next spool |

---

## Casing Hangers

### Hanger Types

| Type | Setting Method |
|------|----------------|
| **Slip type** | Slips grip casing |
| **Mandrel** | Lands on shoulder |
| **Wrap-around** | Assembled around casing |
| **Weld-on** | Welded to casing |

### Casing Hanger Seal

| Seal Type | Description |
|-----------|-------------|
| **Pack-off** | Compressed elastomer |
| **Metal seal** | Metal-to-metal ring |
| **Combination** | Elastomer + metal backup |

---

## Tubing Head

### Functions

1. Support tubing hanger
2. Seal tubing-casing annulus
3. Provide annular access (side outlets)
4. Connect to Christmas tree

### Tubing Hanger Types

| Type | Description |
|------|-------------|
| **Wrap-around** | Assembled around tubing at surface |
| **Mandrel** | Run with tubing |
| **Threaded** | Threads into tubing head bowl |

### Tubing Hanger Penetrations

| Penetration | Purpose |
|-------------|---------|
| **Main bore** | Production flow |
| **Control line** | SCSSV control |
| **Chemical injection** | Corrosion inhibitor, scale |
| **Gauge line** | Downhole pressure |
| **Electrical** | ESP, gauges |

---

## Christmas Tree

### Tree Types

| Type | Description | Application |
|------|-------------|-------------|
| **Conventional** | Standard flanged |Onshore |
| **Solid block** | Machined from solid | High pressure |
| **Composite** | Welded construction | Various |
| **Horizontal** | Valves on side | Dual completion, workover |
| **Subsea** | Subsea installation | Offshore subsea |

### Standard Tree Configuration

```
                    ┌───┐
                    │   │ Cap (Crown Plug)
                    └─┬─┘
                      │
                   ┌──┴──┐
        Wing ───► │     │ ◄─── Wing (Choke)
        Valve     └──┬──┘      Valve
                      │
                 ┌────┴────┐
                 │   SWAB  │ Swab Valve
                 │  VALVE  │
                 └────┬────┘
                      │
                 ┌────┴────┐
                 │  UPPER  │ Upper Master Valve
                 │ MASTER  │
                 └────┬────┘
                      │
                 ┌────┴────┐
                 │  LOWER  │ Lower Master Valve
                 │ MASTER  │
                 └────┬────┘
                      │
                 To Tubing Head
```

### Tree Valve Functions

| Valve | Function |
|-------|----------|
| **Lower master** | Primary barrier, closed for workover |
| **Upper master** | Operational shutoff |
| **Wing valve** | Production outlet isolation |
| **Swab valve** | Wireline access |
| **Choke** | Flow control, rate regulation |
| **Crown plug** | Positive isolation, well entry |

---

## Surface Controlled Subsurface Safety Valve (SCSSV)

### Function

- Fail-safe well closure
- Prevents uncontrolled flow if wellhead damaged
- Required by most operators and regulations

### Types

| Type | Closure Mechanism |
|------|-------------------|
| **Tubing retrievable** | Flapper closes, tubing removed to service |
| **Wireline retrievable** | Inner mechanism retrievable by wireline |

### Control System

```
Surface Control Panel
         │
    Hydraulic line
         │
         ▼
    ┌─────────────┐
    │    SCSSV    │ ← Held open by hydraulic pressure
    │   (Open)    │   Closes on loss of pressure
    └─────────────┘
```

### Testing Requirements

| Test | Frequency |
|------|-----------|
| **Function test** | Every 6-12 months |
| **Leak test** | After function test |
| **Failsafe test** | Verify closure on pressure loss |

---

## Wellhead Installation

### Surface Casing Wellhead

1. Land surface casing
2. Cut casing to proper height
3. Install casing head (weld or thread)
4. Test casing head
5. Install BOP for next hole section

### Intermediate Casing

1. Run and cement casing
2. Hang casing in casing spool
3. Install pack-off/seal
4. Test annular seal
5. Install BOP adaptor

### Completion

1. Run and hang tubing
2. Install tubing hanger seal
3. Pressure test seals
4. Nipple up Christmas tree
5. Test tree valves
6. Install SCSSV (if not already run)
7. Test SCSSV

---

## Wellhead Testing

### Required Tests

| Test | Purpose | Pressure |
|------|---------|----------|
| **Casing seal** | Verify annular isolation | Per program |
| **Tubing hanger** | Verify tubing seal | Working pressure |
| **Tree body** | Verify tree integrity | Rated working pressure |
| **SCSSV** | Verify function | Per API 14B |
| **Control lines** | Verify no leaks | Operating pressure |

### Test Duration

| Test Type | Minimum Duration |
|-----------|------------------|
| **Low pressure** | 5-10 minutes |
| **High pressure** | 10-30 minutes |
| **SCSSV** | Per procedure |

---

## Wellhead Safety

### Key Safety Features

| Feature | Purpose |
|---------|---------|
| **Dual master valves** | Redundant isolation |
| **SCSSV** | Subsurface barrier |
| **Metal-to-metal seals** | High integrity seals |
| **Material specifications** | Match environment |
| **Fire-safe valves** | Function in fire |

### Barrier Philosophy

**Two-Barrier Rule**:
- Always maintain two tested barriers
- Primary: Tubing, SCSSV, master valves
- Secondary: Annular access available

---

## Wellhead Maintenance

### Regular Checks

| Item | Frequency |
|------|-----------|
| **Visual inspection** | Daily |
| **Valve operation** | Weekly/Monthly |
| **Seal integrity** | With production tests |
| **Corrosion check** | Per program |
| **SCSSV test** | Per regulation (typically annual) |

### Common Problems

| Problem | Cause | Solution |
|---------|-------|----------|
| **Valve leak** | Seat damage, corrosion | Repair/replace |
| **Seal leak** | Elastomer failure | Replace seal |
| **Corrosion** | Inadequate protection | Inhibitor, replace |
| **Stuck valve** | Scale, debris, corrosion | Grease, work, repair |
| **SCSSV won't close** | Debris, hydraulic issue | Clean, repair control |

---

## Wellhead Documentation

### Required Records

| Document | Purpose |
|----------|---------|
| **Wellhead schematic** | Configuration record |
| **Test records** | Compliance, integrity |
| **Manufacturer data** | Specifications, ratings |
| **Maintenance log** | Service history |
| **Valve inspection** | Condition tracking |

### Wellhead Schematic Content

- All component sizes and ratings
- Valve types and specifications
- Control line routing
- Penetrations (chemical, gauge, electrical)
- Sealing elements
- Test port locations
