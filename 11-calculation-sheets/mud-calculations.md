# Mud Calculations

## Mud Weight Adjustments

### Weight Up with Barite
```
Barite Required (sk/100 bbl) = 1470 × (W2 - W1) ÷ (35 - W2)

Where:
W1 = Initial mud weight (ppg)
W2 = Desired mud weight (ppg)
35 = Barite specific gravity × 8.34

Example:
Weight up from 10.0 to 11.0 ppg
Barite = 1470 × (11.0 - 10.0) ÷ (35 - 11.0)
Barite = 1470 ÷ 24 = 61.25 sacks per 100 bbl
```

### Volume Increase from Barite
```
Volume Increase (bbl) = Barite (sacks) × 0.091

Example:
Adding 61 sacks barite to 100 bbl
Volume increase = 61 × 0.091 = 5.6 bbl
New volume = 105.6 bbl
```

### Weight Up with Hematite
```
Hematite Required (sk/100 bbl) = 1470 × (W2 - W1) ÷ (42 - W2)

Where 42 = Hematite specific gravity × 8.34 (approximate)
```

### Weight Down (Dilution)
```
Water to Add (bbl) = V1 × (W1 - W2) ÷ (W2 - Wwater)

Where:
V1 = Initial volume
Wwater = 8.34 ppg (fresh) or 8.6 ppg (seawater)

Example:
100 bbl of 12.0 ppg mud, reduce to 11.0 ppg
Water = 100 × (12.0 - 11.0) ÷ (11.0 - 8.34)
Water = 100 ÷ 2.66 = 37.6 bbl water needed
```

## Volume Calculations

### Total Circulating Volume
```
Surface Volume = Active pits + reserve + trip tank
Hole Volume = Drill string + annulus
Total = Surface + Hole Volume
```

### Pit Volume
```
Rectangular: V (bbl) = L × W × H ÷ 5.615

Cylindrical: V (bbl) = π × r² × H ÷ 5.615

Where L, W, H, r in feet
```

### Mud Required to Fill Hole
```
Open Hole: V (bbl) = Hole Diameter² × Length ÷ 1029.4
Cased Hole: V (bbl) = Casing ID² × Length ÷ 1029.4

Total Fill Volume = Drill String Capacity + Annular Capacity
```

## Material Additions

### Bentonite for Yield Point
```
Bentonite (lb/bbl) ≈ 0.5-1.5 lb per lb/100 ft² YP increase

Varies by mud type and existing solids
```

### Caustic Soda for pH
```
Approximate:
0.25 lb/bbl caustic raises pH by ~0.5 unit
(Varies with existing pH and buffering)

Target pH: 9.5-10.5 for most water-based muds
```

### Lignite/Lignosulfonate
```
For fluid loss control:
0.5-2.0 lb/bbl reduces API fluid loss

For rheology modification:
0.25-0.5 lb/bbl reduces gel strengths
```

### Salt Additions
```
Salt Required (lb/bbl) = 3.5 × (Cl₂ - Cl₁)

Where Cl in mg/L (ppm) and result is approximate

For saturated salt mud:
~127 lb/bbl NaCl to saturate freshwater
```

## Solids Analysis

### Percent Solids by Volume
```
% Solids = (MW - 8.34) ÷ (SG of solids - 1) × 8.34 × 100

For low gravity solids (SG = 2.6):
% Solids ≈ (MW - 8.34) ÷ 13.33 × 100

For barite (SG = 4.2):
% Barite ≈ (MW - 8.34) ÷ 26.7 × 100
```

### Low Gravity Solids (LGS)
```
% LGS = % Total Solids - % Barite

High LGS indicates:
- Drilled solids buildup
- Need for dilution or solids control
- Target: <6-8% in most muds
```

### Retort Analysis
```
From retort:
% Oil + % Water + % Solids = 100%

Corrected Solids:
% Solids = 100 - % Oil - % Water
% Suspended Solids = % Solids - % Salt (if any)
```

## Oil-Based Mud Calculations

### Oil/Water Ratio
```
OWR = % Oil ÷ (% Oil + % Water) × 100 / % Water ÷ (% Oil + % Water) × 100

Example:
70% oil, 10% water, 20% solids
OWR = 70 ÷ 80 × 100 / 10 ÷ 80 × 100 = 87.5/12.5 or ~88/12
```

### Adjusting OWR
```
To increase oil ratio:
Oil to add (bbl/100 bbl) = 100 × (R2 - R1) ÷ (100 - R2)

Where R1 = current oil ratio, R2 = desired oil ratio

Example: Change from 75/25 to 85/15
Oil to add = 100 × (85 - 75) ÷ (100 - 85) = 67 bbl per 100 bbl
```

### Electrical Stability (ES)
```
Target ES: >300-500 volts (varies by operator)

Low ES indicates:
- Water contamination
- Emulsifier depletion
- Solids wetting

Increase ES by:
- Adding emulsifier/wetting agent
- Adding lime
- Removing water
```

## Mixing Calculations

### Dilution for Density Reduction
```
V2 = V1 × (W1 - Wd) ÷ (Wd - W2)

Where:
V1 = Volume of heavy mud
W1 = Weight of heavy mud
Wd = Weight of diluent (water or base oil)
W2 = Desired weight
V2 = Volume of diluent needed
```

### Blending Two Muds
```
Final Weight:
W3 = (V1 × W1 + V2 × W2) ÷ (V1 + V2)

Volume of each:
V1 = Vtotal × (W3 - W2) ÷ (W1 - W2)
V2 = Vtotal - V1

Example: Blend 12 ppg and 10 ppg to get 11 ppg
Equal volumes needed: 50% of each
```

## Pump and Flow Calculations

### Pump Output
```
Triplex: Output (bbl/stk) = 0.000243 × D² × L × Eff

Where:
D = Liner diameter (in)
L = Stroke length (in)
Eff = Volumetric efficiency (typically 0.90-0.98)

Example: 6" liners, 12" stroke, 95% efficiency
Output = 0.000243 × 36 × 12 × 0.95 = 0.0996 bbl/stk
```

### Flow Rate
```
GPM = SPM × Pump Output (bbl/stk) × 42

Example:
80 SPM × 0.10 bbl/stk × 42 = 336 GPM
```

### Time to Circulate
```
Bottoms Up Time (min) = Annular Volume (bbl) ÷ (GPM ÷ 42)

Total Circulation Time = (String + Annular Volume) ÷ (GPM ÷ 42)
```

## Cost Calculations

### Mud Cost per Foot
```
Cost/ft = (Material Cost + Service Cost) ÷ Footage Drilled

Track:
- Barite consumption
- Chemical additions
- Lost circulation material
- Mud losses
```

### Material Cost per Barrel
```
Cost/bbl = Σ (Material × Unit Cost) ÷ Total Volume

Include:
- Base fluid
- Weighting material
- Chemicals
- LCM
```

## Quick Reference Tables

### Common Material Weights

| Material | lb/gal | lb/ft³ | Specific Gravity |
|----------|--------|--------|------------------|
| Fresh Water | 8.34 | 62.4 | 1.00 |
| Seawater | 8.6 | 64.3 | 1.03 |
| Diesel | 7.0 | 52.4 | 0.84 |
| Barite | 35.0 | 262 | 4.2 |
| Hematite | 42.0 | 315 | 5.0 |
| Calcium Carbonate | 22.5 | 169 | 2.7 |
| Bentonite | 21.5 | 161 | 2.6 |

### Barite Requirements (sacks per 100 bbl)

| From → To | 10 ppg | 11 ppg | 12 ppg | 13 ppg | 14 ppg |
|-----------|--------|--------|--------|--------|--------|
| 9 ppg | 59 | 122 | 191 | 268 | 355 |
| 10 ppg | - | 61 | 128 | 200 | 280 |
| 11 ppg | - | - | 64 | 131 | 204 |
| 12 ppg | - | - | - | 65 | 134 |
| 13 ppg | - | - | - | - | 67 |

### Dilution Requirements (bbl water per 100 bbl mud)

| From → To | 10 ppg | 11 ppg | 12 ppg |
|-----------|--------|--------|--------|
| 13 ppg | 113 | 75 | 38 |
| 14 ppg | 142 | 100 | 60 |
| 15 ppg | 167 | 122 | 79 |
| 16 ppg | 189 | 142 | 96 |

---

*Mud calculations affect well control, hole cleaning, and formation damage. Verify all calculations before implementation.*
