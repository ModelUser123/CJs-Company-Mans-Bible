# Matrix Acidizing

## Overview

Matrix acidizing involves pumping acid into the formation at pressures below fracturing pressure. The acid dissolves damage or creates new flow channels, improving well productivity without creating fractures.

---

## When to Use Matrix Acidizing

### Objectives

| Objective | Mechanism |
|-----------|-----------|
| **Remove damage** | Dissolve drilling mud, completion fluids |
| **Restore permeability** | Clean perforation tunnels |
| **Stimulate carbonates** | Create wormholes |
| **Clean wellbore** | Remove scale, deposits |

### Candidate Selection

| Good Candidate | Poor Candidate |
|----------------|----------------|
| Near-wellbore damage | Deep damage |
| Acid-soluble minerals | Low permeability sandstone |
| Carbonate formations | High clay content |
| Scale-related damage | Mechanical damage |
| Positive skin | Already negative skin |

---

## Acid Types

### Hydrochloric Acid (HCl)

| Strength | Application |
|----------|-------------|
| **5%** | Scale removal, tubing wash |
| **10%** | Perforation cleanup |
| **15%** | Standard carbonate stimulation |
| **28%** | Deep penetration, limited use |

**Reaction with Limestone**:
```
CaCO₃ + 2HCl → CaCl₂ + H₂O + CO₂
(Limestone)      (Calcium chloride, water, carbon dioxide)
```

### Hydrofluoric Acid (HF) - Mud Acid

**Mixture**: Typically HCl/HF blends

| Blend | HCl % | HF % | Application |
|-------|-------|------|-------------|
| **Standard mud acid** | 12 | 3 | General sandstone |
| **Mild** | 6 | 1.5 | High clay |
| **Strong** | 12 | 6 | Low clay, quartz |

**Reaction with Silica**:
```
SiO₂ + 4HF → SiF₄ + 2H₂O
(Quartz)     (Silicon tetrafluoride, water)
```

### Organic Acids

| Acid | Strength | Application |
|------|----------|-------------|
| **Formic (HCOOH)** | 10-15% | High temperature, corrosion sensitive |
| **Acetic (CH₃COOH)** | 10-15% | Mild stimulation, carbonate |

### Specialty Acids

| Type | Description |
|------|-------------|
| **Emulsified acid** | HCl in diesel emulsion, retarded |
| **Gelled acid** | HCl with polymer, diversion |
| **Foamed acid** | CO₂ or N₂ energized |
| **Self-diverting** | Viscosity increase on spending |

---

## Sandstone Acidizing

### Three-Stage Process

```
┌─────────────────────────────────────────────────────────────┐
│               SANDSTONE ACIDIZING SEQUENCE                  │
├─────────────────────────────────────────────────────────────┤
│                                                             │
│   STAGE 1: PREFLUSH                                        │
│   ┌─────────────────────────────────────────────┐          │
│   │  5-15% HCl                                  │          │
│   │  - Dissolve carbonates                      │          │
│   │  - Displace formation brine                 │          │
│   │  - Prevent CaF₂ precipitation               │          │
│   └─────────────────────────────────────────────┘          │
│                         │                                   │
│                         ▼                                   │
│   STAGE 2: MAIN ACID                                       │
│   ┌─────────────────────────────────────────────┐          │
│   │  HCl/HF (Mud Acid)                          │          │
│   │  - Dissolve clays                           │          │
│   │  - Dissolve silicates                       │          │
│   │  - Remove drilling damage                   │          │
│   └─────────────────────────────────────────────┘          │
│                         │                                   │
│                         ▼                                   │
│   STAGE 3: OVERFLUSH                                       │
│   ┌─────────────────────────────────────────────┐          │
│   │  3-5% HCl or NH₄Cl                          │          │
│   │  - Push reaction products away              │          │
│   │  - Prevent precipitation                    │          │
│   │  - Clean up wellbore                        │          │
│   └─────────────────────────────────────────────┘          │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

### Sandstone Acidizing Guidelines

| Formation Type | Preflush | Main Acid | Overflush |
|----------------|----------|-----------|-----------|
| **Low clay (<5%)** | 10% HCl | 12/3 HCl/HF | 3% HCl |
| **Med clay (5-10%)** | 7.5% HCl | 9/1 HCl/HF | NH₄Cl |
| **High clay (>10%)** | 5% HCl | 6/1.5 HCl/HF | NH₄Cl |
| **High temp (>250°F)** | 10% Acetic | Organic mud acid | NH₄Cl |

---

## Carbonate Acidizing

### Wormhole Formation

**Concept**: In carbonates, acid creates preferential flow paths (wormholes) rather than uniform dissolution

```
       Injection Well
            │
            │
            ▼
      ╭─────────────╮
      │ ~~ ~~ ~~ ~~ │  ← Wormhole network
      │~~ ~ ~ ~ ~ ~~│
      │ ~ ~ ~~ ~ ~ ~│
      │~~ ~ ~ ~ ~ ~ │
      ╰─────────────╯
       Matrix
```

### Wormhole Optimization

| Injection Rate | Result |
|----------------|--------|
| **Too low** | Face dissolution, limited penetration |
| **Optimal** | Dominant wormholes, deep penetration |
| **Too high** | Uniform dissolution, acid waste |

### Carbonate Acidizing Guidelines

| Situation | Acid | Concentration |
|-----------|------|---------------|
| **Limestone** | HCl | 15-28% |
| **Dolomite** | HCl | 15% (slower reaction) |
| **High temp** | Gelled or emulsified | Per design |
| **Deep penetration** | Retarded acid | Per design |

---

## Acid Volume Design

### Volume Guidelines

| Application | Volume (gal/ft) |
|-------------|-----------------|
| **Damage removal** | 50-100 |
| **Carbonate stimulation** | 100-200 |
| **Deep penetration** | 200-500 |
| **Preflush** | 25-50 |
| **Overflush** | 50-100 |

### Calculation Example

```
Zone: 50 ft net pay
Objective: Damage removal (75 gal/ft)
Preflush: 25 gal/ft
Main acid: 75 gal/ft
Overflush: 50 gal/ft

Volumes:
Preflush = 50 ft × 25 gal/ft = 1,250 gal (30 bbl)
Main acid = 50 ft × 75 gal/ft = 3,750 gal (89 bbl)
Overflush = 50 ft × 50 gal/ft = 2,500 gal (60 bbl)

Total = 179 bbl
```

---

## Acid Additives

### Common Additives

| Additive | Purpose | Concentration |
|----------|---------|---------------|
| **Corrosion inhibitor** | Protect tubulars | 0.2-2% |
| **Surfactant** | Water wetting, cleanup | 0.1-0.5% |
| **Iron control** | Prevent Fe precipitation | 0.5-1% |
| **Clay stabilizer** | Prevent fines migration | 0.1-0.5% |
| **Mutual solvent** | Water/oil compatibility | 5-10% |
| **Scale inhibitor** | Prevent scale | Per design |
| **Friction reducer** | Reduce pump pressure | 0.1-0.5% |

### Temperature Considerations

| Temperature | Issue | Solution |
|-------------|-------|----------|
| < 150°F | Standard acids work well | Standard inhibitor |
| 150-250°F | Faster reaction, corrosion | Intensifier, higher inhibitor |
| 250-350°F | Rapid spending, severe corrosion | Organic acids, special inhibitor |
| > 350°F | Extreme conditions | Specialty systems |

---

## Diversion

### Why Diversion?

Without diversion, acid enters highest permeability zones, bypassing damaged zones that need treatment.

### Diversion Methods

| Method | Mechanism |
|--------|-----------|
| **Mechanical** | Ball sealers, packers |
| **Chemical** | Viscous gels, foams |
| **Particulate** | Benzoic acid flakes, wax |
| **Self-diverting** | Acid viscosity increases on spending |

### Ball Sealers

| Factor | Guideline |
|--------|-----------|
| **Number** | 2-4 × number of perforations |
| **Density** | Match to fluid density |
| **Size** | Larger than perforation entry holes |

---

## Pumping Operations

### Rate Guidelines

| Formation | Rate (bpm/ft) |
|-----------|---------------|
| **Sandstone** | 0.1-0.25 |
| **Carbonate** | 0.25-0.5 |
| **High perm** | Lower rates |
| **Low perm** | Higher rates |

### Maximum Pressure

```
Max Surface Pressure = Frac Gradient × TVD - Hydrostatic + Friction

Stay BELOW fracturing pressure for matrix treatment
```

### Monitoring

| Parameter | Watch For |
|-----------|-----------|
| **Surface pressure** | Dropping = good, rising = problems |
| **Rate** | Maintain design rate |
| **Temperature** | Monitor returns |
| **pH** | Indicates acid spending |

---

## Safety Considerations

### Acid Hazards

| Hazard | Mitigation |
|--------|------------|
| **Corrosive** | Full PPE (face shield, gloves, apron) |
| **Reactive** | Keep away from incompatibles |
| **Fumes** | Respiratory protection |
| **Skin contact** | Immediate wash, medical attention |
| **Environmental** | Containment, neutralization |

### Emergency Response

| Situation | Action |
|-----------|--------|
| **Skin contact** | Flush with water 15+ minutes |
| **Eye contact** | Flush with water, seek medical help |
| **Spill** | Neutralize with soda ash, contain |
| **HF exposure** | Special treatment required, calcium gluconate |

---

## Job Evaluation

### Success Indicators

| Indicator | Interpretation |
|-----------|----------------|
| **Pressure decline** | Acid reaching formation |
| **Rate increase** | Treatment effective |
| **Returns pH rising** | Acid spending |
| **Production increase** | Primary goal |
| **Skin reduction** | Quantified improvement |

### Post-Job Analysis

| Analysis | Purpose |
|----------|---------|
| **Production test** | Quantify improvement |
| **Pressure buildup** | Calculate new skin |
| **Production log** | Verify treated interval |

---

## Acid Job Checklist

### Pre-Job
- [ ] Candidate selection confirmed
- [ ] Acid system designed
- [ ] Additives specified
- [ ] Volumes calculated
- [ ] Equipment tested
- [ ] Safety meeting held
- [ ] Spill containment in place

### During Job
- [ ] Monitor pressure vs. rate
- [ ] Track volumes pumped
- [ ] Watch for anomalies
- [ ] Record all parameters
- [ ] Safety monitoring active

### Post-Job
- [ ] Flush lines
- [ ] Flow well for cleanup
- [ ] Collect samples
- [ ] Document results
- [ ] Production test
