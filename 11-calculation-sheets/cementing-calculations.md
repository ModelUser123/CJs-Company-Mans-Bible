# Cementing Calculations

## Cement Slurry Properties

### Slurry Weight
```
Standard Class G cement: 15.8 ppg (at 5.2 gal/sk water)
Class H cement: 16.4 ppg (at 4.3 gal/sk water)

Slurry Weight Range: 11.5-18.5 ppg depending on additives
```

### Slurry Yield
```
Yield = Volume produced per sack of cement

Standard Class G: 1.15 ft³/sk (at 5.2 gal/sk)
Class H: 1.06 ft³/sk (at 4.3 gal/sk)

Yield (ft³/sk) = (94 + (8.34 × gal water)) ÷ (Slurry Weight × 7.48)
```

### Water Requirements
```
Percent water = (gal water × 8.34 × 100) ÷ 94

Example:
5.2 gal/sk → (5.2 × 8.34 × 100) ÷ 94 = 46.1% BWOC
```

## Volume Calculations

### Annular Volume
```
Annular Volume (ft³) = 0.7854 × (Dh² - Dc²) × Length ÷ 144

Annular Volume (bbl) = (Dh² - Dc²) × Length ÷ 1029.4

Where:
Dh = Hole diameter (inches)
Dc = Casing OD (inches)
Length = Interval length (ft)
```

### Example Annular Volume
```
8.5" hole, 7" casing, 2,000 ft interval

Volume (bbl) = (8.5² - 7²) × 2,000 ÷ 1029.4
Volume = (72.25 - 49) × 2,000 ÷ 1029.4
Volume = 45.2 bbl = 253 ft³
```

### Casing Shoe Track Volume
```
Shoe Track (bbl) = Casing ID² × Length ÷ 1029.4

Example: 7" casing (6.366" ID), 60 ft shoe track
Volume = 6.366² × 60 ÷ 1029.4 = 2.36 bbl
```

### Lead and Tail Cement Volumes
```
Total Cement = Annular Volume + Shoe Track + Excess

Typical Excess: 30-100% depending on hole conditions

Lead Cement: Lower density, fills larger annulus
Tail Cement: Higher density, across producing zones
```

## Cement Quantity Calculations

### Sacks Required
```
Sacks = Volume (ft³) ÷ Yield (ft³/sk)

Example:
Volume needed: 300 ft³
Yield: 1.15 ft³/sk
Sacks = 300 ÷ 1.15 = 261 sacks
```

### Mix Water Required
```
Water (gal) = Sacks × Water Ratio (gal/sk)

Example:
261 sacks × 5.2 gal/sk = 1,357 gal = 32.3 bbl
```

### Additive Quantities
```
Additive (lb) = Sacks × Additive Concentration (% BWOC) × 0.94

Example: 3% CaCl₂
Amount = 261 × 0.03 × 94 = 736 lb
```

## Displacement Calculations

### Displacement Volume
```
Displacement = Casing Capacity - Plug Volume

Casing Capacity (bbl) = ID² × Length ÷ 1029.4

Example: 7" casing (6.366" ID), 10,000 ft
Capacity = 6.366² × 10,000 ÷ 1029.4 = 393.6 bbl
```

### Displacement to Plug Bump
```
Displacement Volume = Casing Volume - (Top Plug Volume + Float Volume)

Account for:
- Top plug wiper length
- Float collar position
- Surface line volume (add to pump volume)
```

### Strokes to Bump
```
Strokes = Displacement Volume (bbl) ÷ Pump Output (bbl/stk)

Example:
Displacement: 390 bbl
Pump output: 0.117 bbl/stk
Strokes = 390 ÷ 0.117 = 3,333 strokes
```

## Hydrostatic Calculations

### Cement Column Pressure
```
Pressure (psi) = 0.052 × Slurry Weight (ppg) × TVD (ft)

Example:
15.8 ppg cement, 1,000 ft column
Pressure = 0.052 × 15.8 × 1,000 = 822 psi
```

### U-Tube Effect
```
Cement will fall until:
Cement Hydrostatic = Mud Hydrostatic (inside casing)

Free fall height = (Cement Column × (ρcement - ρmud)) ÷ ρcement

Minimize by:
- Dropping plugs correctly
- Using float equipment
- Proper cement weight
```

### Differential Pressure at Shoe
```
ΔP = (Cement Hydrostatic) - (Formation Pore Pressure)

Check against:
- Fracture gradient (don't exceed)
- Pore pressure (maintain overbalance)
```

## Pump Pressure Calculations

### Expected Surface Pressure
```
Surface Pressure = Friction Losses + Hydrostatic Difference

During cement:
P = Friction (pipe + annulus) + (ρcement - ρmud) × 0.052 × Cement Height
```

### Bump Pressure
```
Bump Pressure = Pressure to seat plug + Line friction

Typical bump pressure: 500-1500 psi above circulating pressure
Hold for 5-10 minutes to verify float
```

### Pressure Limits
```
Maximum Pressure = Minimum of:
- Casing burst rating
- Formation fracture pressure
- Equipment rating
- Cement pump capacity
```

## Balanced Plug Calculations

### Balanced Plug Concept
```
Cement inside pipe = Cement outside pipe
Fluid columns balance when plug is spotted
Pipe can be pulled without disturbing cement
```

### Plug Length Calculation
```
Pipe Capacity × Cement Length (in pipe) =
Annular Capacity × Cement Length (in annulus)

Since cement is balanced:
Length in pipe = Length in annulus = Plug Length

Volume = Plug Length × (Pipe Cap + Annular Cap)
```

### Balanced Plug Procedure
```
1. Calculate cement volume for desired plug length
2. Calculate spacer volumes (above and below)
3. Pump sequence: Spacer → Cement → Spacer → Displace
4. Displace to leave cement balanced
5. Pull pipe slowly out of cement
```

### Displacement for Balanced Plug
```
Displacement = Pipe Volume - (Cement in Pipe + Top Spacer)

OR

Calculate so cement top inside pipe = cement top in annulus
```

## Excess Cement Factors

### Recommended Excess (% over gauge)

| Hole Condition | Excess Factor |
|---------------|---------------|
| Gauge hole (good caliper) | 10-20% |
| Slightly washed out | 30-50% |
| Severely washed out | 50-100% |
| Cavernous | 100-200%+ |
| Liner jobs | 5-10% |

### Hole Volume from Caliper
```
If caliper available:
Actual Volume = Σ (Caliper Reading² × Interval Length) ÷ 1029.4

This gives true volume accounting for washouts
```

## Quick Reference Tables

### Common Cement Properties

| Class | Water (gal/sk) | Yield (ft³/sk) | Weight (ppg) |
|-------|---------------|----------------|--------------|
| A | 5.2 | 1.18 | 15.6 |
| C | 6.3 | 1.32 | 14.8 |
| G | 5.2 | 1.15 | 15.8 |
| H | 4.3 | 1.06 | 16.4 |

### Additive Effects

| Additive | Purpose | Typical % |
|----------|---------|-----------|
| Calcium Chloride | Accelerator | 2-4% |
| Retarder | Extend thickening time | 0.1-0.5% |
| Fluid Loss | Reduce filtrate loss | 0.5-1.5% |
| Dispersant | Reduce viscosity | 0.2-0.5% |
| Silica Flour | High temp stability | 35-40% |
| Bentonite | Extend/lighten | 2-16% |

### Casing Capacity (bbl/ft)

| Casing Size | Weight (lb/ft) | ID (in) | Capacity |
|-------------|---------------|---------|----------|
| 5½" | 17 | 4.892 | 0.0233 |
| 7" | 26 | 6.276 | 0.0383 |
| 9⅝" | 47 | 8.681 | 0.0732 |
| 13⅜" | 68 | 12.415 | 0.1498 |

---

*Cement calculations are critical. Always verify independently and have contingency plans.*
