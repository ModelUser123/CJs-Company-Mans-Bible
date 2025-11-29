# Production Calculations

## Flow Rate Conversions

### Oil Rate Conversions
```
1 barrel (bbl) = 42 gallons = 5.615 ft³
1 bbl/day = 0.159 m³/day = 5.615 ft³/day

Stock Tank Barrels (STB) = Reservoir Barrels ÷ Formation Volume Factor
STB = RB ÷ Bo

Where Bo = Oil formation volume factor (typically 1.1-1.5)
```

### Gas Rate Conversions
```
1 Mcf = 1,000 standard cubic feet
1 MMcf = 1,000,000 standard cubic feet
1 Mcf ≈ 28.3 m³ (at standard conditions)

Surface Gas Volume = Reservoir Gas ÷ Bg
```

### Gas-Oil Ratio (GOR)
```
GOR (scf/STB) = Gas Production Rate ÷ Oil Production Rate

Example:
Gas = 500 Mcf/day, Oil = 250 STB/day
GOR = 500,000 ÷ 250 = 2,000 scf/STB
```

### Water Cut
```
Water Cut (%) = Water Rate ÷ (Water Rate + Oil Rate) × 100

or

Water Cut = Qw ÷ Qtotal × 100

Example:
Oil = 200 bpd, Water = 800 bpd
Water Cut = 800 ÷ 1000 × 100 = 80%
```

## Inflow Performance

### Productivity Index (PI)
```
PI (STB/day/psi) = Q ÷ (Pr - Pwf)

Where:
Q = Production rate (STB/day)
Pr = Reservoir pressure (psi)
Pwf = Flowing bottomhole pressure (psi)

Example:
Q = 500 STB/day, Pr = 3,000 psi, Pwf = 2,000 psi
PI = 500 ÷ (3,000 - 2,000) = 0.5 STB/day/psi
```

### IPR - Darcy's Law (Undersaturated Oil)
```
Q = (0.00708 × k × h × (Pr - Pwf)) ÷ (μ × Bo × ln(re/rw))

Where:
k = Permeability (md)
h = Net pay (ft)
μ = Viscosity (cp)
Bo = Formation volume factor
re = Drainage radius (ft)
rw = Wellbore radius (ft)
```

### IPR - Vogel's Equation (Saturated Oil)
```
Q/Qmax = 1 - 0.2×(Pwf/Pr) - 0.8×(Pwf/Pr)²

or

Q = Qmax × [1 - 0.2×(Pwf/Pr) - 0.8×(Pwf/Pr)²]

Where Qmax = Absolute open flow (AOF)
```

### IPR - Gas Well (Back Pressure Equation)
```
Q = C × (Pr² - Pwf²)^n

Where:
C = Backpressure coefficient
n = Backpressure exponent (0.5 to 1.0)

Typically from deliverability test analysis
```

## Pressure Calculations

### Bottomhole Pressure (Static)
```
BHP = Surface Pressure + Hydrostatic Pressure

BHP = Psurf + (0.052 × ρfluid × TVD)

For gas wells:
BHP = Psurf × exp(0.01875 × SG × TVD ÷ T × Z)
(Z = Compressibility factor, T = Temperature °R)
```

### Flowing Bottomhole Pressure
```
Pwf = Pwh + ΔPfriction + ΔPgravity

For tubing flow:
Account for multiphase effects using correlations:
- Hagedorn-Brown
- Beggs-Brill
- Duns-Ros
```

### Pressure Gradient
```
Gas: 0.01-0.05 psi/ft (varies with pressure)
Oil: 0.3-0.4 psi/ft (varies with density)
Water: 0.433-0.465 psi/ft (salinity dependent)
```

## Artificial Lift Calculations

### Rod Pump - Pump Displacement
```
PD (bbl/day) = 0.1166 × S × N × D²

Where:
S = Stroke length (inches)
N = Strokes per minute
D = Pump diameter (inches)

Example:
S = 86", N = 8 spm, D = 2.5"
PD = 0.1166 × 86 × 8 × 2.5² = 501 bbl/day
```

### Rod Pump - Efficiency
```
Actual Production = PD × Volumetric Efficiency

Volumetric Efficiency typically 60-90%
Affected by:
- Fluid slippage
- Gas interference
- Pump fillage
```

### ESP - Required Horsepower
```
HP = (Q × TDH × SG) ÷ 3960

Where:
Q = Flow rate (bpd)
TDH = Total dynamic head (ft)
SG = Specific gravity

Example:
Q = 1000 bpd, TDH = 6000 ft, SG = 1.0
HP = (1000 × 6000 × 1.0) ÷ 3960 = 1515 HP
```

### Gas Lift - Injection Rate
```
Gas Injection Rate = f(Production rate, GLR, injection depth)

Approximate:
Qg (Mcf/day) = Qo × Injected GLR ÷ 1000

Where Injected GLR typically 300-1000 scf/bbl
```

### Gas Lift - Gradient Design
```
Flowing Gradient = f(GLR, flow rate, tubing size)

Higher GLR → Lower gradient → Lower Pwf → Higher rate
Balance against gas availability and compression costs
```

## Reserves Calculations

### Material Balance (Volumetric)
```
OOIP (STB) = 7758 × A × h × φ × (1 - Sw) ÷ Bo

Where:
A = Area (acres)
h = Net pay (ft)
φ = Porosity (fraction)
Sw = Water saturation (fraction)
Bo = Formation volume factor

OGIP (Mcf) = 43,560 × A × h × φ × (1 - Sw) ÷ Bg
```

### Recovery Factor
```
RF = Cumulative Production ÷ OOIP

Primary Recovery: 5-20% (oil), 50-80% (gas)
Secondary (waterflood): 15-40% additional
EOR: 5-20% additional
```

### Decline Curve Analysis
```
Exponential Decline:
Q = Qi × e^(-D×t)

Hyperbolic Decline:
Q = Qi × (1 + b×D×t)^(-1/b)

Where:
Qi = Initial rate
D = Decline rate
t = Time
b = Decline exponent (0-1)
```

### EUR Calculation
```
EUR = Cumulative + Remaining Reserves

Remaining = ∫Q(t)dt from now to abandonment
```

## Wellhead and Choke Calculations

### Choke Sizing (Critical Flow - Gas)
```
Q (Mcf/day) = 879.5 × Cd × d² × P1 ÷ √(T × SG)

Where:
Cd = Discharge coefficient (~0.9)
d = Choke diameter (64ths of inch)
P1 = Upstream pressure (psia)
T = Temperature (°R)
SG = Gas specific gravity
```

### Critical Flow Condition
```
P2/P1 < 0.55 for gas
P2/P1 < [(2/(k+1))^(k/(k-1))] for ideal gas

Below this ratio: Flow is sonic (critical)
Above this ratio: Flow is subsonic
```

### Bean Size Selection
```
Rule of thumb for oil:
d (64ths) ≈ √(Q × √(Pr - Pwh)) ÷ K

K depends on oil gravity and GOR
Trial and error often used in practice
```

## Skin and Damage

### Skin Factor
```
ΔPskin = (141.2 × Q × μ × Bo × s) ÷ (k × h)

Where s = Skin factor

Positive skin: Damage
Negative skin: Stimulation effect

s = 0: No damage or stimulation
s = +5: Moderate damage
s = -3: Typical acid stimulation
s = -6 to -8: Hydraulic fracture
```

### Flow Efficiency
```
FE = (Pr - Pwf - ΔPskin) ÷ (Pr - Pwf)

or

FE = Jactual ÷ Jideal

FE > 1: Stimulated
FE = 1: Undamaged
FE < 1: Damaged
```

## Economics Quick Calculations

### Operating Cost per Barrel
```
OPEX/bbl = Total Operating Cost ÷ Production

Include:
- Lifting costs
- Workover costs
- Facility costs
- G&A allocation
```

### Net Revenue Interest
```
NRI = 1 - Royalty - Overrides - Other Burdens

Net Revenue = Gross Revenue × NRI
```

### Cash Flow
```
Monthly Cash Flow = (Revenue × NRI) - OPEX - CAPEX - Taxes
```

## Quick Reference Tables

### Typical Formation Volume Factors

| Fluid | Bo/Bg Range | Notes |
|-------|-------------|-------|
| Light Oil | 1.1-1.5 | Higher for volatile oils |
| Medium Oil | 1.05-1.2 | |
| Heavy Oil | 1.0-1.05 | Near 1.0 for very heavy |
| Gas | 0.002-0.02 | Varies with P & T |

### Typical Productivity Index Values

| Formation | PI Range (STB/day/psi) |
|-----------|----------------------|
| Poor | 0.1-0.5 |
| Average | 0.5-2.0 |
| Good | 2.0-5.0 |
| Excellent | 5.0+ |

### Common Conversion Factors

| Convert | To | Multiply By |
|---------|-----|-------------|
| bbl/day | m³/day | 0.159 |
| Mcf/day | m³/day | 28.32 |
| psi | kPa | 6.895 |
| ft | m | 0.3048 |
| °F | °C | (°F-32) × 5/9 |

---

*Production calculations should be verified with actual well test data when available.*
