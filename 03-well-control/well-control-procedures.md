# Well Control Procedures

## Overview

Well control procedures are designed to prevent, detect, and respond to kicks. Every crew member must understand and be prepared to execute these procedures.

---

## Primary Well Control

### Definition
Using hydrostatic pressure to prevent formation fluids from entering the wellbore.

### Requirements

```
Hydrostatic Pressure > Formation Pressure

HP = 0.052 × MW × TVD

Where:
HP = Hydrostatic Pressure (psi)
MW = Mud Weight (ppg)
TVD = True Vertical Depth (ft)
```

### Maintaining Primary Control

| Factor | Action |
|--------|--------|
| Mud weight | Maintain per program |
| Trip margin | Add 0.2-0.5 ppg for trips |
| Swab effect | Control pulling speed |
| ECD | Monitor while circulating |
| Gas cut mud | Evaluate, weight up if needed |

---

## Secondary Well Control

### Definition
Using BOP equipment to contain formation pressure while circulating out influx and restoring primary control.

### When Used
- Kick has entered wellbore
- Primary control lost
- Influx cannot be circulated conventionally

---

## Shut-In Procedures

### Hard Shut-In

**When to Use:**
- Standard procedure for most operations
- When kick tolerance allows

**Procedure:**
1. Stop rotation
2. Pick up off bottom (if on bottom)
3. Space out (tool joint in BOP)
4. Shut off pumps
5. Open HCR (if used)
6. Close annular or pipe rams
7. Close choke (if not already)
8. Record SIDPP and SICP
9. Notify Company Man

### Soft Shut-In

**When to Use:**
- Sensitive formations
- Limited kick tolerance
- As specified by company policy

**Procedure:**
1. Stop rotation
2. Pick up off bottom
3. Space out
4. Shut off pumps
5. Open HCR (choke line)
6. Close annular or pipe rams
7. Close choke slowly
8. Record SIDPP and SICP
9. Notify Company Man

### Shut-In While Tripping

**Pipe Out of Hole:**
1. Set slips
2. Install full-open safety valve
3. Close safety valve
4. Close BOP
5. Record pressures

**Going in Hole:**
1. Set slips
2. Close BOP
3. Record pressures

---

## Pressure Recording

### Initial Shut-In Pressures

| Pressure | Location | Use |
|----------|----------|-----|
| SIDPP | Drill pipe pressure | Calculate KWM |
| SICP | Casing (annular) pressure | Monitor influx |

### Pressure Stabilization

- Wait for pressures to stabilize (typically 5-15 minutes)
- Longer in low-permeability formations
- Record both SIDPP and SICP
- Pressure may continue to build (migration)

---

## Kill Weight Mud Calculation

### Formula

```
KWM = MW + (SIDPP / (0.052 × TVD))

Where:
KWM = Kill Weight Mud (ppg)
MW = Current mud weight (ppg)
SIDPP = Shut-In Drill Pipe Pressure (psi)
TVD = True Vertical Depth (ft)
```

### Example

```
Current MW: 10.0 ppg
SIDPP: 520 psi
TVD: 10,000 ft

KWM = 10.0 + (520 / (0.052 × 10,000))
KWM = 10.0 + 1.0
KWM = 11.0 ppg
```

---

## Kick Information

### Determine Kick Type

| Indicator | Gas | Saltwater | Oil |
|-----------|-----|-----------|-----|
| SICP vs SIDPP | Much higher | Slightly higher | Slightly higher |
| Pressure increase rate | Fast | Slow | Slow |
| Pit gain size | Small to large | Large | Moderate |

### Estimate Kick Size

```
Kick Volume = Pit Gain (bbl)
Kick Height = Kick Volume / Annular Capacity
```

---

## Maximum Allowable Pressures

### MAASP (Maximum Allowable Annular Surface Pressure)

```
MAASP = (Frac Gradient - MW) × 0.052 × Shoe TVD

Or:

MAASP = LOT Pressure - (MW × 0.052 × Shoe TVD)
```

### Importance
- Never exceed MAASP
- Will cause underground blowout
- Must be posted at choke console

---

## Kill Sheets

### Pre-Calculated Information

**Before Drilling:**
- Hole volumes
- String volumes
- Pump strokes per volume
- Pressure schedules
- Maximum allowable pressures

### Active Kill Sheet Information

```
KILL SHEET

Date: _____________ Time: ____________

SHUT-IN DATA:
SIDPP: _________ psi
SICP:  _________ psi
Pit Gain: _______ bbl

DEPTHS:
MD: _________ ft
TVD: ________ ft
Casing Shoe TVD: _______ ft

CURRENT CONDITIONS:
Mud Weight: _______ ppg
Pump Rate: _______ SPM @ _______ GPM
Slow Circulating Pressure: _______ psi

CALCULATED VALUES:
Kill Weight Mud: _______ ppg
ICP: _______ psi
FCP: _______ psi
Strokes to bit: _______
Strokes surface to surface: _______
MAASP: _______ psi

PRESSURE SCHEDULE:
See attached chart
```

---

## Slow Circulating Pressures

### Recording Requirements

**Record at:**
- Start of each tour
- After each trip
- After significant depth change
- After BHA change
- After mud property change

### Recording Procedure

1. Position bit near bottom (500 ft off)
2. Bring pumps to kill rate (typically 1/2 normal)
3. Record pressure at stable rate
4. Record for multiple rates

### Standard Kill Rates

| Rate | Purpose |
|------|---------|
| 1/4 normal | Very low rate option |
| 1/2 normal | Standard kill rate |
| 3/4 normal | Alternative rate |

---

## Communication Protocols

### Notification Chain

1. **Immediate (within minutes):**
   - Company Man
   - Toolpusher
   - Rig crew (via PA)

2. **Within 1 hour:**
   - Operations Manager
   - Drilling Engineer

3. **As Required:**
   - Regulatory agency
   - Well control specialists
   - Partners

### Information to Report

- Well identification
- Current depth (MD/TVD)
- SIDPP and SICP
- Pit gain
- Time of shut-in
- Current status
- Plan of action

---

## Well Control Equipment

### Choke Console

**Components:**
- Manual choke
- Remote choke
- Pressure gauges
- Stroke counter
- MAASP posted

**Operation:**
- Adjust choke to maintain drill pipe pressure
- Monitor casing pressure
- Never exceed MAASP

### Kill Line

**Use:**
- Pump kill weight mud
- Bullhead operations
- Reverse circulation

---

## Documentation Requirements

### During Event

```
□ Time log of all events
□ Pressures recorded
□ Volumes pumped
□ Decisions made
□ Personnel involved
□ Communications made
```

### Post-Event

```
□ Complete incident report
□ Kill sheet completed
□ Lessons learned documented
□ Regulatory reporting (if required)
□ Review with crew
```

---

## Related Documents

- [Kick Detection](./kick-detection.md)
- [Kill Procedures](./kill-procedures.md)
- [Kill Sheet Calculations](../10-calculation-sheets/kill-sheet-calculations.md)
- [Well Control Decision Trees](../09-decision-trees/well-control-decisions.md)
- [Emergency Action Plans](../08-emergency-response/emergency-action-plans.md)
