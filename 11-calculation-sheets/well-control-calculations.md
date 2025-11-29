# Well Control Calculations

## Fundamental Pressure Relationships

### Formation Pressure from SIDPP
```
Formation Pressure (psi) = Hydrostatic Pressure + SIDPP

FP = (0.052 × MW × TVD) + SIDPP

Example:
MW = 10 ppg, TVD = 10,000 ft, SIDPP = 500 psi
FP = (0.052 × 10 × 10,000) + 500 = 5,700 psi
```

### Formation Pressure Gradient
```
FP Gradient (ppg) = Formation Pressure ÷ (0.052 × TVD)

Example:
FP = 5,700 psi, TVD = 10,000 ft
Gradient = 5,700 ÷ (0.052 × 10,000) = 10.96 ppg
```

## Kill Mud Weight

### Kill Mud Weight (KMW)
```
KMW (ppg) = Original MW + (SIDPP ÷ (0.052 × TVD))

Example:
Original MW = 10 ppg, SIDPP = 500 psi, TVD = 10,000 ft
KMW = 10 + (500 ÷ (0.052 × 10,000))
KMW = 10 + 0.96 = 10.96 ppg

Round UP to nearest 0.1 ppg = 11.0 ppg
```

### Kill Mud Weight with Safety Margin
```
KMW (with margin) = KMW + Safety Margin (0.2-0.5 ppg typical)

Example:
KMW = 10.96 ppg + 0.3 ppg margin = 11.26 ppg → 11.3 ppg
```

## Circulating Pressures

### Initial Circulating Pressure (ICP)
```
ICP (psi) = SIDPP + Slow Circulating Rate Pressure (SCR)

Example:
SIDPP = 500 psi, SCR @ kill rate = 800 psi
ICP = 500 + 800 = 1,300 psi
```

### Final Circulating Pressure (FCP)
```
FCP (psi) = SCR × (KMW ÷ Original MW)

Example:
SCR = 800 psi, KMW = 11.0 ppg, Original MW = 10 ppg
FCP = 800 × (11.0 ÷ 10) = 880 psi
```

### Step-Down Schedule (Wait & Weight)
```
Pressure Drop per Stroke = (ICP - FCP) ÷ Strokes to Bit

Strokes to Bit = Drill String Volume ÷ Pump Output

Example:
ICP = 1300 psi, FCP = 880 psi
Strokes to bit = 2000
Drop per stroke = (1300 - 880) ÷ 2000 = 0.21 psi/stk

Schedule:
At 0 strokes: 1300 psi
At 500 strokes: 1300 - (500 × 0.21) = 1195 psi
At 1000 strokes: 1090 psi
At 1500 strokes: 985 psi
At 2000 strokes: 880 psi (FCP)
```

## Maximum Allowable Pressures

### Maximum Allowable Annular Surface Pressure (MAASP)
```
MAASP (psi) = (Frac Gradient - MW) × 0.052 × Shoe TVD

Example:
Frac Gradient = 14.5 ppg EMW, MW = 10 ppg, Shoe TVD = 5,000 ft
MAASP = (14.5 - 10) × 0.052 × 5,000
MAASP = 4.5 × 0.052 × 5,000 = 1,170 psi
```

### MAASP (from LOT)
```
MAASP (psi) = LOT Pressure - (MW × 0.052 × Shoe TVD) + (MW × 0.052 × Shoe TVD)

Simplified:
MAASP = LOT Pressure - ((MW - Test MW) × 0.052 × Shoe TVD)
```

### Maximum Allowable Shut-In Casing Pressure (MASICP)
```
MASICP = MAASP (at surface)

Consider:
• Casing burst rating
• Wellhead rating
• BOP rating
• Use lowest of all limits
```

## Kick Volume and Migration

### Kick Volume (Pit Gain)
```
Kick Volume (bbl) = Pit Gain Observed

Note: This is initial volume. Gas will expand as it migrates.
```

### Gas Migration Rate (Uncontrolled)
```
Typical Migration Rate = 1,000-2,000 ft/hr in static conditions

Pressure increase rate = Migration Rate × 0.052 × (MW - Gas Gradient)

Example:
Migration = 1,500 ft/hr, MW = 12 ppg, Gas = 0.1 ppg
Pressure increase = 1,500 × 0.052 × (12 - 0.1) = 928 psi/hr
```

### Gas Expansion
```
At surface, gas volume = Bottomhole Volume × (BHP ÷ Surface Pressure)

Boyle's Law: P1V1 = P2V2

Example:
10 bbl gas kick at 10,000 ft, BHP = 5,200 psi
At surface (15 psi): V2 = 10 × (5,200 ÷ 15) = 3,467 bbl!
```

## Kick Tolerance

### Kick Tolerance Definition
```
Maximum kick volume that can be shut in without
exceeding MAASP at the shoe
```

### Kick Tolerance Calculation (Gas Kick)
```
KT (bbl) = (MAASP ÷ (0.052 × (MW - Gas Gradient))) × Annular Capacity at Shoe

Simplified for low pressure gas:
KT ≈ (MAASP ÷ (0.052 × MW)) × Annular Capacity

Example:
MAASP = 1,170 psi, MW = 12 ppg, Annular Capacity = 0.05 bbl/ft at shoe
KT = (1,170 ÷ (0.052 × 12)) × 0.05 × Height
```

## Volumetric Method

### Pressure Increment Selection
```
Typical Increment = 50-100 psi
Smaller increment = More control, more work
Larger increment = Less work, higher BHP variation
```

### Volume to Bleed per Increment
```
Volume (bbl) = (Pressure Increment × Annular Capacity × Length) ÷
               (0.052 × MW × Length)

Simplified:
Volume (bbl) = Pressure Increment ÷ (0.052 × MW) × Annular Capacity

Example:
100 psi increment, 12 ppg mud, 0.05 bbl/ft annular capacity
Volume per 100 psi = 100 ÷ (0.052 × 12) × 0.05 = 8 bbl per 100 ft
```

## Stripping/Snubbing Calculations

### Snub Force Required
```
Snub Force (lb) = (Closed Pressure × Pipe Area) - Pipe Weight

Pipe Area (sq in) = 0.7854 × OD²

Example:
SICP = 2,000 psi, 5" DP
Area = 0.7854 × 5² = 19.63 sq in
Snub Force = (2,000 × 19.63) - Pipe Weight
           = 39,270 lb - Pipe Weight
```

### Volume to Bleed per Stand (Stripping)
```
Bleed Volume = (Pipe Displacement × Pipe Length) ÷
               (1 - (Surface Pressure ÷ BHP))

For gas kick, approximately:
Bleed Volume ≈ Pipe Displacement × Length Stripped
```

## Kill Sheet Values Summary

| Parameter | Formula | Units |
|-----------|---------|-------|
| KMW | MW + (SIDPP ÷ 0.052 ÷ TVD) | ppg |
| ICP | SIDPP + SCR | psi |
| FCP | SCR × (KMW ÷ MW) | psi |
| MAASP | (FG - MW) × 0.052 × Shoe TVD | psi |
| Strokes to Bit | DS Volume ÷ Pump Output | strokes |
| Strokes to Surface | Annular Volume ÷ Pump Output | strokes |

## Quick Reference - Pressure Conversions

| MW (ppg) | Gradient (psi/ft) | Pressure @ 1000 ft |
|----------|-------------------|-------------------|
| 8.34 | 0.433 | 433 psi |
| 9.0 | 0.468 | 468 psi |
| 10.0 | 0.520 | 520 psi |
| 11.0 | 0.572 | 572 psi |
| 12.0 | 0.624 | 624 psi |
| 13.0 | 0.676 | 676 psi |
| 14.0 | 0.728 | 728 psi |
| 15.0 | 0.780 | 780 psi |
| 16.0 | 0.832 | 832 psi |
| 17.0 | 0.884 | 884 psi |
| 18.0 | 0.936 | 936 psi |

## Example Kill Sheet Calculation

```
GIVEN:
TVD = 12,000 ft
Original MW = 11.5 ppg
SIDPP = 450 psi
SICP = 650 psi
Pit Gain = 15 bbl
SCR @ 30 spm = 750 psi
Pump Output = 0.117 bbl/stk
Drill String Volume = 200 bbl
Annular Volume = 450 bbl
Shoe TVD = 8,000 ft
Frac Gradient at Shoe = 15.2 ppg EMW

CALCULATIONS:

1. Kill Mud Weight:
   KMW = 11.5 + (450 ÷ (0.052 × 12,000))
   KMW = 11.5 + 0.72 = 12.22 ppg → 12.3 ppg

2. Initial Circulating Pressure:
   ICP = 450 + 750 = 1,200 psi

3. Final Circulating Pressure:
   FCP = 750 × (12.3 ÷ 11.5) = 802 psi → 800 psi

4. Strokes to Bit:
   STB = 200 ÷ 0.117 = 1,709 strokes

5. Strokes to Surface:
   STS = (200 + 450) ÷ 0.117 = 5,556 strokes

6. MAASP:
   MAASP = (15.2 - 11.5) × 0.052 × 8,000 = 1,539 psi

7. Pressure Drop per 100 Strokes:
   Drop = ((1,200 - 800) ÷ 1,709) × 100 = 23.4 psi/100 stk
```

---

*All well control calculations must be verified before use. Keep kill sheet updated with current well data.*
