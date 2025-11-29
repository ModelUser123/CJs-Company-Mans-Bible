# Hydraulic Fracturing

## Overview

Hydraulic fracturing creates conductive fractures in the formation to increase well productivity. This is the primary stimulation method for low-permeability reservoirs and is essential for unconventional resource development.

---

## Fracturing Fundamentals

### How Fracturing Works

```
┌─────────────────────────────────────────────────────────────┐
│                    FRACTURE CREATION                        │
├─────────────────────────────────────────────────────────────┤
│                                                             │
│   1. BREAKDOWN                                              │
│      High pressure exceeds rock strength                    │
│      Fracture initiates at wellbore                         │
│                                                             │
│   2. PROPAGATION                                            │
│      ←─────────────────●─────────────────→                 │
│         Fracture grows away from wellbore                   │
│         Fluid pressure holds fracture open                  │
│                                                             │
│   3. PROPPANT PLACEMENT                                     │
│      ←══════════════●══════════════→                      │
│         Proppant fills fracture                             │
│         Prevents closure                                    │
│                                                             │
│   4. CLOSURE                                                │
│      ←▓▓▓▓▓▓▓▓▓▓▓▓▓●▓▓▓▓▓▓▓▓▓▓▓▓▓→                        │
│         Proppant holds fracture open                        │
│         Creates conductive path                             │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

### Key Concepts

| Term | Definition |
|------|------------|
| **Breakdown pressure** | Pressure to initiate fracture |
| **Propagation pressure** | Pressure to extend fracture |
| **Closure pressure** | In-situ stress holding fracture closed |
| **Net pressure** | Treating pressure - closure pressure |
| **Fracture gradient** | Pressure per ft of depth (psi/ft) |
| **ISIP** | Instantaneous shut-in pressure |

### Fracture Geometry

| Parameter | Definition | Typical Range |
|-----------|------------|---------------|
| **Half-length (xf)** | Distance from wellbore | 100-1,000+ ft |
| **Height (hf)** | Vertical extent | 50-500 ft |
| **Width (w)** | Opening width | 0.1-0.5 inches |
| **Conductivity (kf×w)** | Flow capacity | 100-10,000 md-ft |

---

## Fracture Fluids

### Fluid Types

| Type | Base | Application |
|------|------|-------------|
| **Slickwater** | Water + friction reducer | Unconventional, low visc |
| **Linear gel** | Guar/HPG polymer | Moderate proppant transport |
| **Crosslinked gel** | Borate/metal crosslinked | High proppant concentration |
| **Oil-based** | Diesel or crude | Water-sensitive formations |
| **Foam** | N₂ or CO₃ energized | Low pressure, water-sensitive |
| **Acid** | HCl | Carbonate fracturing |

### Slickwater Properties

| Property | Typical Value |
|----------|---------------|
| **Base fluid** | Fresh water or produced water |
| **Friction reducer** | 0.25-2 gpt (gallons per thousand) |
| **Viscosity** | 1-5 cp |
| **Proppant loading** | 0.25-2 ppg |
| **Pump rate** | 80-120 bpm per stage |

### Crosslinked Gel Properties

| Property | Typical Value |
|----------|---------------|
| **Polymer loading** | 20-40 lb/1000 gal |
| **Crosslinker** | Borate, Ti, Zr |
| **Viscosity** | 100-500 cp |
| **Proppant loading** | 2-12 ppg |
| **Temperature range** | To 400°F |

---

## Proppant Selection

### Proppant Types

| Type | Crush Strength | Application |
|------|----------------|-------------|
| **Sand** | 4,000-6,000 psi | Shallow, low stress |
| **Resin-coated sand** | 6,000-8,000 psi | Moderate stress, flowback control |
| **Ceramic** | 10,000-15,000 psi | High stress, deep wells |
| **Bauxite** | 15,000-20,000 psi | Very high stress |

### Proppant Sizes

| Mesh Size | Diameter (inches) | Application |
|-----------|-------------------|-------------|
| **100 mesh** | 0.006 | Slickwater, fracture tip |
| **40/70** | 0.010-0.017 | Most common, moderate conductivity |
| **30/50** | 0.012-0.024 | Higher conductivity |
| **20/40** | 0.017-0.033 | Conventional, high perm |

### Proppant Concentration

| Stage | Concentration (ppg) | Purpose |
|-------|---------------------|---------|
| **Pad** | 0 | Create fracture geometry |
| **Slurry start** | 0.25-0.5 | Begin filling fracture |
| **Ramp** | 0.5-2 | Gradual increase |
| **Flush** | 0 | Displace to formation |

---

## Fracture Design Parameters

### Treatment Sizing

| Parameter | Conventional | Unconventional |
|-----------|--------------|----------------|
| **Fluid volume** | 20,000-100,000 gal | 100,000-500,000+ gal |
| **Proppant mass** | 50,000-200,000 lb | 200,000-1,000,000 lb |
| **Pump rate** | 30-80 bpm | 60-120 bpm |
| **Pump time** | 1-3 hours | 2-4 hours |

### Conductivity vs. Fracture Length

**Dimensionless Fracture Conductivity (FCD)**:
```
FCD = (kf × w) / (k × xf)

Where:
kf = Fracture permeability
w = Fracture width
k = Formation permeability
xf = Fracture half-length

Optimal: FCD = 1.6 (for maximum productivity)
```

### Fracture Design Optimization

| Formation k | Strategy |
|-------------|----------|
| **Very low (<0.01 md)** | Long fracture, moderate conductivity |
| **Low (0.01-0.1 md)** | Balance length and conductivity |
| **Moderate (0.1-10 md)** | Higher conductivity, shorter length |
| **High (>10 md)** | Very high conductivity, short fracture |

---

## Unconventional Frac Design

### Multi-Stage Horizontal Wells

```
┌─────────────────────────────────────────────────────────────────────┐
│                    HORIZONTAL WELL FRACTURING                       │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│   Surface ────────────────────────────────────────                 │
│                    │                                                │
│                    │ Vertical                                       │
│                    │                                                │
│   ─────────────────┼───────────────────────────────────────────    │
│                    ╲                                                │
│                     ╲ Curve                                         │
│                      ╲                                              │
│   ═════════════════════════════════════════════════════════════    │
│    │   │   │   │   │   │   │   │   │   │   │   │   │   │   │      │
│    ▼   ▼   ▼   ▼   ▼   ▼   ▼   ▼   ▼   ▼   ▼   ▼   ▼   ▼   ▼      │
│   Transverse fractures from each stage                              │
│                                                                     │
│   Toe ◄────────────────────────────────────────────────────► Heel  │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

### Stage Design Parameters

| Parameter | Typical Range |
|-----------|---------------|
| **Lateral length** | 5,000-15,000 ft |
| **Number of stages** | 20-60 |
| **Stage spacing** | 150-300 ft |
| **Clusters per stage** | 3-8 |
| **Cluster spacing** | 25-75 ft |
| **Perfs per cluster** | 3-6 |

### Slickwater Design Example

| Parameter | Value |
|-----------|-------|
| **Fluid volume/stage** | 8,000-15,000 bbl |
| **Proppant/stage** | 300,000-600,000 lb |
| **Pump rate** | 90-100 bpm |
| **Max pressure** | 9,000-12,000 psi |
| **Stage duration** | 2-3 hours |

---

## Frac Fluid Additives

### Common Additives

| Additive | Purpose | Concentration |
|----------|---------|---------------|
| **Friction reducer** | Reduce treating pressure | 0.5-2 gpt |
| **Biocide** | Prevent bacteria | 0.1-0.5 gpt |
| **Scale inhibitor** | Prevent scale | 0.5-2 gpt |
| **Clay stabilizer** | Prevent clay swelling | 0.5-2 gpt |
| **Surfactant** | Aid cleanup, water wetting | 0.5-2 gpt |
| **Iron control** | Prevent precipitation | 0.5-1 gpt |
| **Buffer** | pH control | As needed |
| **Breaker** | Degrade viscosity | 0.25-2 lb/1000 gal |

### Crosslinker Systems

| System | Temperature Range | pH |
|--------|-------------------|----|
| **Borate** | 75-300°F | 8-12 |
| **Titanium** | 150-350°F | 3-9 |
| **Zirconium** | 200-400°F | 3-11 |

---

## Pressure Analysis

### Pressure Components

```
Treating Pressure = Closure Pressure + Net Pressure + Friction

Surface Pressure = BHP - Hydrostatic + Pipe Friction + Perf Friction
```

### Key Pressure Points

| Pressure | Significance |
|----------|--------------|
| **Breakdown** | Fracture initiation |
| **Treating** | Pressure during pumping |
| **ISIP** | Pressure at instant of shut-in |
| **Closure** | In-situ stress, frac closes |
| **Final** | After fracture closes |

### Pressure Interpretation

```
Pressure
    │
    │    ┌───────────────────
    │   ╱   Treating pressure
    │  ╱
    │ ╱
    │╱     Breakdown
    │
    │
ISIP├──────────╮
    │          │╲
    │          │ ╲  Pressure decline
    │          │  ╲
Pc ─┼──────────┼───╲─────────── Closure pressure
    │          │    ╲___________
    │          │
    └──────────┴────────────────► Time
     Pumping   Shut-in
```

---

## Frac Equipment

### Surface Equipment Layout

```
┌─────────────────────────────────────────────────────────────────┐
│                    FRAC SPREAD LAYOUT                           │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│   [Water Storage]  [Sand Storage]  [Chemical Tanks]            │
│         │               │                │                      │
│         ▼               ▼                ▼                      │
│   ┌─────────────────────────────────────────┐                  │
│   │           BLENDER / MIXER               │                  │
│   │    (Combines fluid, sand, chemicals)    │                  │
│   └────────────────────┬────────────────────┘                  │
│                        │                                        │
│                        ▼                                        │
│   ┌───────────────────────────────────────────────────────┐    │
│   │              FRAC PUMPS (10-20+ units)                │    │
│   │    ╔═══╗  ╔═══╗  ╔═══╗  ╔═══╗  ╔═══╗  ╔═══╗         │    │
│   │    ║   ║  ║   ║  ║   ║  ║   ║  ║   ║  ║   ║         │    │
│   │    ╚═══╝  ╚═══╝  ╚═══╝  ╚═══╝  ╚═══╝  ╚═══╝         │    │
│   └───────────────────────┬───────────────────────────────┘    │
│                           │                                     │
│                           ▼                                     │
│              ┌────────────────────────┐                        │
│              │     MISSILE/MANIFOLD   │                        │
│              └───────────┬────────────┘                        │
│                          │                                      │
│                          ▼                                      │
│                     WELLHEAD                                    │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### Equipment Specifications

| Equipment | Specification |
|-----------|---------------|
| **Frac pump** | 2,000-2,700 HHP per unit |
| **Pump pressure** | 10,000-15,000 psi |
| **Blender** | 120-180 bpm capacity |
| **Hydration** | 80-120 bpm |
| **Iron** | 15,000 psi rated typical |

---

## Frac Job Monitoring

### Real-Time Data

| Parameter | What to Watch |
|-----------|---------------|
| **Surface pressure** | Trend, stability |
| **Rate** | Maintain design rate |
| **Proppant concentration** | As scheduled |
| **Slurry rate** | Blender output |
| **Fluid density** | Quality control |
| **Bottomhole pressure** | If gauges available |

### Warning Signs

| Observation | Possible Issue |
|-------------|----------------|
| **Pressure rising rapidly** | Screenout, bridging |
| **Pressure declining** | Height growth, out of zone |
| **Pressure erratic** | Equipment issues |
| **Rate dropping** | Pump problems |
| **Proppant not tracking** | Blender issues |

---

## Safety Considerations

### High-Pressure Hazards

| Hazard | Mitigation |
|--------|------------|
| **Treating line failure** | High-pressure rated iron, inspection |
| **Pump failure** | Isolation, pop-offs |
| **Chemical exposure** | PPE, containment |
| **Noise** | Hearing protection |
| **Struck-by** | Safety zones, barriers |

### Safety Zones

| Zone | Distance | Requirements |
|------|----------|--------------|
| **Red zone** | <50 ft | Essential personnel only |
| **Exclusion zone** | Around treating lines | No personnel during pump |
| **Control zone** | All equipment | Hard hat, safety glasses, FRC |

---

## Frac Job Checklist

### Pre-Job
- [ ] Treatment design reviewed
- [ ] Equipment positioned
- [ ] Iron pressure tested
- [ ] Chemicals staged
- [ ] Proppant tested
- [ ] BOP/wellhead tested
- [ ] Safety meeting held

### During Job
- [ ] Real-time monitoring active
- [ ] Pressure within design
- [ ] Proppant schedule tracked
- [ ] Safety monitoring continuous
- [ ] Communication established

### Post-Job
- [ ] Well shut in, monitored
- [ ] Equipment rigged down safely
- [ ] Data recorded
- [ ] Flowback plan in place
