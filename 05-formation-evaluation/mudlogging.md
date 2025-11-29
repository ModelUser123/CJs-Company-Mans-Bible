# Mudlogging

## Overview

Mudlogging provides real-time formation evaluation data during drilling operations. The mudlogger monitors drilling parameters, analyzes cuttings, and detects hydrocarbon shows - often providing the first indication of pay zones.

---

## Mudlogging Unit Services

### Core Services

| Service | Description | Deliverable |
|---------|-------------|-------------|
| **Cuttings analysis** | Lithology description | Strip log, sample descriptions |
| **Gas detection** | Total gas and components | Gas curves, chromatograph data |
| **Drilling parameter monitoring** | ROP, WOB, torque, etc. | Parameter log |
| **Sample collection** | Catch and store cuttings | Sample sets (10 ft, 30 ft intervals) |
| **Show evaluation** | Hydrocarbon assessment | Show descriptions, gas ratios |

### Additional Services (Optional)

| Service | Purpose |
|---------|---------|
| **Pore pressure monitoring** | D-exponent, ECD tracking |
| **Shale density** | Geopressure indicators |
| **Calcimetry** | Carbonate percentage |
| **Formation pressure indication** | Connection gas analysis |
| **Fluorescence analysis** | Hydrocarbon typing |

---

## Gas Detection System

### Total Gas Monitoring

**Gas Trap (Possum Belly)**:
```
┌─────────────────────────────────────────┐
│           FLOW LINE FROM WELL           │
│                    │                    │
│                    ▼                    │
│    ┌───────────────────────────────┐    │
│    │         POSSUM BELLY          │    │
│    │    (Degasser/Gas Trap)        │    │
│    │                               │    │
│    │    ┌─────────────────────┐    │    │
│    │    │  Gas Extraction     │────┼────┼──→ To Detector
│    │    │  (Agitator/Vacuum)  │    │    │
│    │    └─────────────────────┘    │    │
│    │                               │    │
│    └───────────────────────────────┘    │
│                    │                    │
│                    ▼                    │
│              To Shakers                 │
└─────────────────────────────────────────┘
```

### Gas Components

| Component | Formula | Significance |
|-----------|---------|--------------|
| **Methane** | C₁ | Dominant in dry gas, biogenic gas |
| **Ethane** | C₂ | Thermogenic indicator |
| **Propane** | C₃ | Heavier hydrocarbon indicator |
| **Iso-Butane** | iC₄ | Oil prone source |
| **N-Butane** | nC₄ | Thermogenic maturity |
| **Pentanes** | C₅ | Oil indicator |

### Gas Ratio Analysis

| Ratio | Formula | Interpretation |
|-------|---------|----------------|
| **Wetness (Wh)** | (C₂+C₃+C₄+C₅)/C₁ × 100 | <0.5% = dry gas, >5% = oil prone |
| **Balance** | (C₁+C₂)/(C₃+C₄+C₅) | Oil vs gas indicator |
| **Character** | C₄+C₅/C₃ | Oil maturity indicator |
| **Pixler Ratio** | C₁/C₂ | Oil vs gas discrimination |

### Gas Reading Types

| Gas Type | Cause | Interpretation |
|----------|-------|----------------|
| **Background gas** | Formation gas liberated by drilling | Baseline formation content |
| **Connection gas** | Gas released when pumps stopped | Swabbing, formation pressure |
| **Trip gas** | Gas on first bottoms-up after trip | Formation pressure, swab |
| **Drilling break gas** | Associated with ROP increase | Porous zone, possible pay |
| **Recycled gas** | Gas circulated back from cuttings pit | Not formation gas |

---

## Cuttings Analysis

### Sample Collection

| Sample Type | Interval | Purpose |
|-------------|----------|---------|
| **Wet samples** | Every 10-30 ft | Lithology, shows |
| **Washed samples** | Every 30 ft | Clean description |
| **Unwashed samples** | Every 10 ft | Preserve oil shows |
| **Grab samples** | As needed | Shows, unusual cuttings |

### Lag Time Calculation

**Lag Time = Time for cuttings to travel from bit to surface**

```
Lag Time (min) = Annular Volume (bbl) / Pump Output (bbl/min)

Annular Volume = Hole Volume - Drill String Volume
```

**Lag Depth Calculation**:
```
Lag Depth = Current Depth - (Lag Time × ROP)
```

**Strokes to Surface**:
```
Strokes = Annular Volume (bbl) × 42 gal/bbl / Pump Output (gal/stroke)
```

### Lithology Description Format

**Standard Description Order**:
1. Rock type
2. Color
3. Hardness
4. Grain size (if applicable)
5. Sorting (if applicable)
6. Cementation/porosity
7. Accessories (fossils, minerals)
8. Hydrocarbon shows

**Example Descriptions**:

| Formation | Description |
|-----------|-------------|
| **Sandstone** | SS: Lt Gry-Wh, med hd, fn-med gr, mod srt, calc cmt, gd vis por, tr glauc, no fluor |
| **Shale** | SH: Dk Gry-Blk, mod hd-hd, subfiss-fiss, slty, calc, org rich, no fluor |
| **Limestone** | LS: Tan-Lt Brn, hd, microxln, tr vug por, tr dolm, no fluor |
| **Dolomite** | DOL: Lt Gry, hd, xln, suc, fair intxln por, no fluor |

### Hardness Scale

| Term | Scratch Test |
|------|--------------|
| **Soft** | Easily scratched with fingernail |
| **Moderately Soft** | Scratched with fingernail with difficulty |
| **Moderately Hard** | Easily scratched with steel |
| **Hard** | Scratched with steel with difficulty |
| **Very Hard** | Cannot be scratched with steel |

---

## Show Evaluation

### Fluorescence Analysis

**Procedure**:
1. Place fresh cuttings on porcelain plate
2. Examine under UV light (black light)
3. Note color, intensity, and distribution
4. Apply solvent cut if fluorescence present
5. Describe cut fluorescence

**Fluorescence Colors**:

| Color | Interpretation |
|-------|----------------|
| **Gold/Yellow** | Light oil (high API gravity) |
| **Orange** | Medium oil |
| **Brown/Dull** | Heavy oil or residual |
| **Blue-White** | Condensate/light hydrocarbon |
| **Dull Brown** | Dead oil, staining |

### Cut Fluorescence

| Cut Type | Result | Interpretation |
|----------|--------|----------------|
| **Fast streaming** | Immediate bright cut | Mobile light oil |
| **Slow streaming** | Gradual color release | Medium-heavy oil |
| **Blooming** | Color spreads slowly | Heavy oil |
| **Crush cut** | Color after crushing | Tight rock, residual |
| **No cut** | No color release | No moveable oil |

### Show Classification

| Class | Description | Action |
|-------|-------------|--------|
| **Good Show** | Strong fluor, fast cut, high gas, good porosity | Log, test, core consider |
| **Fair Show** | Moderate fluor, streaming cut, elevated gas | Evaluate, possible test |
| **Poor Show** | Weak fluor, slow cut, background gas | Note, continue monitoring |
| **Trace** | Very weak fluor, minimal gas | Record, unlikely pay |

---

## Drilling Parameters

### Parameters Recorded

| Parameter | Significance |
|-----------|--------------|
| **ROP** | Formation hardness, bit condition |
| **WOB** | Drilling efficiency |
| **RPM** | Drilling efficiency |
| **Torque** | Formation, hole condition |
| **Standpipe Pressure** | Hydraulics, motor performance |
| **Flow Rate** | ECD, hole cleaning |
| **Mud Weight In/Out** | Gas influx, fluid losses |
| **Temperature In/Out** | Formation temperature |

### D-Exponent for Pore Pressure

**Corrected D-Exponent**:
```
dc = d × (MW_normal / MW_actual)

Where:
d = log(ROP/60N) / log(12W/10⁶D)

ROP = Rate of Penetration (ft/hr)
N = Rotary Speed (RPM)
W = Weight on Bit (lb)
D = Bit Diameter (in)
```

**Interpretation**:
- Increasing dc = Normal compaction trend
- Decreasing dc = Potential overpressure (pressure transition zone)

---

## Communication and Reporting

### Show Notification Protocol

| Show Severity | Notify |
|---------------|--------|
| **Any fluorescence** | Driller, Company Man |
| **Elevated gas (2x background)** | Company Man |
| **Good show** | Company Man, Geologist, Operations |
| **Possible kick indicators** | Driller immediately |

### Log Requirements

| Log Type | Contents | Delivery |
|----------|----------|----------|
| **Strip log** | Lithology, gas, parameters | Continuous |
| **Daily log** | 24-hour summary | Daily to office |
| **Final log** | Complete well record | End of well |
| **Sample descriptions** | Written descriptions | End of well |

### Morning Report Input

Mudlogger provides:
- Formations drilled
- Shows encountered
- Gas readings (max/min/background)
- Cuttings character
- Any anomalies observed

---

## Quality Control

### Gas Detector Calibration

| Check | Frequency | Requirement |
|-------|-----------|-------------|
| **Zero check** | Daily | Baseline at 0 |
| **Span check** | Daily | Known gas concentration |
| **Chromatograph calibration** | Weekly | Multi-component standard |
| **Gas trap check** | Daily | Proper operation |

### Sample Quality

| Issue | Cause | Solution |
|-------|-------|----------|
| **Cavings** | Wellbore instability | Note on log, don't over-represent |
| **Recycled cuttings** | Poor solids control | Note, verify with lag time |
| **Ground samples** | PDC bit, long circulation | Adjust description technique |
| **Contaminated samples** | LCM, cement | Note, separate from formation |

---

## Mudlogging Checklist

### Pre-Spud
- [ ] Unit positioned and leveled
- [ ] Gas detector calibrated
- [ ] Sample trays labeled
- [ ] Communication established
- [ ] Log format approved
- [ ] Offset data reviewed

### During Drilling
- [ ] Monitor gas continuously
- [ ] Catch samples per program
- [ ] Update lag time for depth
- [ ] Describe cuttings per interval
- [ ] Report shows immediately
- [ ] Maintain log quality

### At TD
- [ ] Complete final log
- [ ] Organize sample sets
- [ ] Write final show summary
- [ ] Archive electronic data
- [ ] Clean and bag samples for shipping
