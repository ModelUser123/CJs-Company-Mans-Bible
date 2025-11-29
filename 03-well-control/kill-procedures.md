# Kill Procedures

## Overview

Kill procedures restore primary well control after a kick. Selection of the appropriate method depends on well conditions, equipment, and personnel capabilities.

---

## Kill Methods

### Driller's Method

**Description:** Circulate out kick with original mud, then circulate kill weight mud.

**Advantages:**
- Simpler execution
- Can begin immediately
- Less calculation required

**Disadvantages:**
- Higher casing shoe pressure
- Longer circulation time
- More casing wear (two circulations)

**When to Use:**
- Weighting materials not immediately available
- Simple well geometry
- Adequate shoe strength

### Wait and Weight Method (Engineer's Method)

**Description:** Weight up mud, then circulate out kick and kill well in one circulation.

**Advantages:**
- Lower casing shoe pressures
- Shorter overall time
- One circulation

**Disadvantages:**
- Requires time to weight up
- More complex execution
- Requires accurate calculations

**When to Use:**
- Weighting materials available
- Marginal shoe strength
- Standard recommended practice

### Concurrent Method

**Description:** Begin circulating immediately while weighting up; switch to kill weight when available.

**Advantages:**
- Immediate start
- Optimizes time and pressure

**Disadvantages:**
- Complex execution
- Variable pressure schedules
- Requires close monitoring

### Volumetric Method

**Description:** Control pressure while gas migrates without circulation.

**When to Use:**
- No circulation possible
- Pipe off bottom
- Pipe plugged

### Bullheading

**Description:** Force formation fluids back into formation by pumping down annulus or drill string.

**When to Use:**
- Kill fluid readily available
- Formation will accept fluids
- Conventional circulation not possible

**Risks:**
- Underground blowout
- Casing damage
- Loss of well control

---

## Driller's Method Procedure

### First Circulation (Remove Kick)

1. **Bring pump to kill rate**
   - Hold casing pressure constant
   - Note initial circulating pressure (ICP)
   - ICP = SIDPP + SCR

2. **Circulate kick out**
   - Maintain ICP constant
   - Adjust choke as needed
   - Monitor for gas expansion near surface

3. **Complete first circulation**
   - Pump strokes to bit + surface
   - Verify SIDPP returns to original

### Second Circulation (Kill Well)

1. **Pump kill weight mud**
   - Maintain constant ICP initially
   - Reduce pressure per schedule as kill mud fills drill string

2. **Pressure Schedule:**
   - ICP at start
   - FCP when kill mud at bit
   - Linear reduction between

3. **Complete circulation**
   - Continue at FCP until kill mud at surface
   - Monitor for full circulation
   - Verify zero pressures

---

## Wait and Weight Procedure

### Preparation

1. **Calculate kill weight mud:**
   ```
   KWM = MW + (SIDPP / (0.052 × TVD))
   ```

2. **Calculate Initial Circulating Pressure:**
   ```
   ICP = SIDPP + SCR
   ```

3. **Calculate Final Circulating Pressure:**
   ```
   FCP = SCR × (KWM / MW)
   ```

4. **Prepare pressure schedule:**
   - ICP at surface (stroke 0)
   - FCP when kill mud at bit
   - Linear reduction between

### Execution

1. **Bring pump to kill rate**
   - Hold casing pressure constant
   - Establish ICP

2. **Begin pumping kill weight mud**
   - Follow pressure schedule
   - Reduce drill pipe pressure per schedule
   - Maintain constant BHP

3. **Kill mud at bit**
   - Pressure should be at FCP
   - Maintain FCP constant

4. **Continue circulation**
   - Maintain FCP
   - Circulate until kill mud at surface
   - Monitor for gas expansion

5. **Verify kill**
   - Shut in
   - Check for zero pressures
   - If pressure, continue circulation

---

## Pressure Schedule

### Calculating Strokes

**Strokes to Bit:**
```
Strokes = (Drill String Volume (bbl) × 42) / Pump Output (gal/stroke)
```

**Component Volumes:**
```
Drill Pipe: V = (ID²/1029.4) × Length
Drill Collars: V = (ID²/1029.4) × Length
```

### Example Pressure Schedule

| Strokes | Pressure (psi) |
|---------|----------------|
| 0 | 1,200 (ICP) |
| 200 | 1,160 |
| 400 | 1,120 |
| 600 | 1,080 |
| 800 | 1,040 |
| 1,000 | 1,000 (FCP) |

**Note:** Maintain FCP until kill mud returns to surface

---

## Gas Expansion Management

### Near-Surface Expansion

**Gas expands significantly in upper portion of well**
- Volume doubles from 1000 psi to 500 psi
- Volume doubles again from 500 psi to 250 psi
- Most expansion in last few hundred feet

### Choke Management

**As gas approaches surface:**
- Choke opens rapidly
- Pressure decreases quickly
- Must maintain BHP

**Techniques:**
- Anticipate choke adjustment
- Open choke as needed
- Monitor pit volume for gas volume

### After Gas at Surface

- Continue circulating
- Monitor for additional gas
- Verify well dead

---

## Volumetric Method

### When to Use

- Cannot circulate
- Drill string off bottom
- Plugged string

### Procedure

1. **Allow gas to migrate**
   - Monitor casing pressure increase
   - Calculate pressure increase per unit height

2. **Bleed volume to maintain constant BHP**
   ```
   Pressure build-up allowed = Safety margin × 0.052 × gas migration distance
   
   Volume to bleed = Casing capacity × migration distance
   ```

3. **Repeat as gas migrates**
   - Allow pressure to build
   - Bleed calculated volume
   - Repeat until gas at surface

4. **Vent gas at surface**
   - Control bleed rate
   - Monitor for additional migration

### Example

```
Allow casing pressure to build 100 psi
Then bleed to reduce pressure 100 psi
Repeat until gas at surface
```

---

## Bullheading

### Procedure

1. **Calculate volumes**
   - Annular volume to shoe
   - Kill fluid requirements

2. **Pump down annulus (or drill string)**
   - Control pump rate
   - Monitor pressure vs. rate

3. **Maintain pressure below formation strength**
   - Do not exceed fracture pressure
   - Risk of underground blowout

4. **Continue until well dead**
   - Full annulus displacement
   - Zero surface pressure

### Risks

- Formation breakdown
- Underground blowout
- Casing failure
- H2S/gas at surface

---

## Kill Sheet Example

```
KILL SHEET

Well: Example #1
Date: ___________

SHUT-IN DATA:
SIDPP: 520 psi
SICP: 650 psi
Pit Gain: 15 bbl

DEPTHS:
MD: 12,500 ft
TVD: 10,000 ft
Casing Shoe TVD: 3,000 ft

MUD DATA:
Current MW: 10.0 ppg
SCR @ 30 SPM: 600 psi
Pump Output: 0.1 bbl/stroke

CALCULATIONS:
Kill Weight Mud = 10.0 + (520/(0.052 × 10,000))
KWM = 11.0 ppg

ICP = SIDPP + SCR = 520 + 600 = 1,120 psi
FCP = SCR × (KWM/MW) = 600 × (11.0/10.0) = 660 psi

STROKES:
Drill String Volume: 100 bbl
Strokes to Bit: 100/0.1 = 1,000 strokes

PRESSURE SCHEDULE:
Strokes    Pressure
0          1,120 psi
250        1,005 psi
500        890 psi
750        775 psi
1,000      660 psi (FCP)

MAASP: 800 psi
```

---

## Verification of Kill

### After Circulation Complete

1. **Stop pumps**
2. **Close choke**
3. **Monitor pressures (15 minutes)**
   - SIDPP should be zero
   - SICP should be zero

4. **If zero pressures:**
   - Open BOP
   - Resume operations
   - Document event

5. **If pressure present:**
   - Evaluate cause
   - Continue circulating
   - Recalculate if needed

---

## Complications

### Problems During Kill

| Problem | Response |
|---------|----------|
| Pump failure | Switch to backup, volumetric if needed |
| Choke plugs | Use backup choke, clear obstruction |
| Exceeding MAASP | Reduce pump rate, evaluate |
| Pipe sticking | Continue kill, address after |
| Lost circulation | Evaluate severity, may need to bullhead |

### Unusual Situations

**Stripping:**
- Moving pipe with well under pressure
- Required if pipe must be moved to bottom
- Use stripping procedure with BOP

**Snubbing:**
- Running pipe against pressure
- When pipe weight < hydraulic force
- Requires specialized equipment

---

## Related Documents

- [Well Control Procedures](./well-control-procedures.md)
- [Kill Sheet Calculations](../10-calculation-sheets/kill-sheet-calculations.md)
- [Well Control Decision Trees](../09-decision-trees/well-control-decisions.md)
- [Blowout Response](../08-emergency-response/blowout-response.md)
