# Lost Circulation Decision Tree

## Initial Loss Detection

```
┌─────────────────────────────────────────────────────────────┐
│                 PIT VOLUME DECREASING                       │
│            (Not due to surface transfer)                    │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│              QUANTIFY THE LOSS RATE                         │
│    • Stop drilling, pick up off bottom                     │
│    • Measure losses over 15-30 minutes                     │
│    • Calculate bbl/hr loss rate                            │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
              ┌───────────────────────────────┐
              │     WHAT IS LOSS RATE?        │
              └───────────────────────────────┘
                 │         │          │
    ┌────────────┘         │          └────────────┐
    ▼                      ▼                       ▼
┌──────────┐        ┌──────────────┐        ┌──────────────┐
│ SEEPAGE  │        │  PARTIAL     │        │   TOTAL      │
│ <10 bbl/hr│        │ 10-50 bbl/hr │        │  >50 bbl/hr  │
│          │        │              │        │ or complete  │
└──────────┘        └──────────────┘        └──────────────┘
    │                      │                       │
    ▼                      ▼                       ▼
```

## Seepage Losses (<10 bbl/hr)

```
┌─────────────────────────────────────────────────────────────┐
│                  SEEPAGE LOSSES                             │
│                    <10 bbl/hr                               │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│    1. ADD FINE LCM TO ACTIVE SYSTEM                        │
│       • 5-15 lb/bbl concentration                          │
│       • Fine nut plug, mica, cellophane                    │
│       • Continue drilling with LCM in mud                  │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
              ┌───────────────────────────────┐
              │   LOSSES STOPPED?             │
              └───────────────────────────────┘
                     │              │
                 YES │              │ NO
                     ▼              ▼
         ┌───────────────┐   ┌───────────────────────┐
         │ Continue ops  │   │ Increase concentration│
         │ Monitor for   │   │ to 20-30 lb/bbl      │
         │ recurrence    │   │ Add medium grades    │
         └───────────────┘   └───────────────────────┘
                                    │
                                    ▼
                       ┌──────────────────────┐
                       │ STILL LOSING?        │
                       │ If yes, treat as     │
                       │ PARTIAL losses       │
                       └──────────────────────┘
```

## Partial Losses (10-50 bbl/hr)

```
┌─────────────────────────────────────────────────────────────┐
│                   PARTIAL LOSSES                            │
│                   10-50 bbl/hr                              │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│          IDENTIFY LOSS ZONE TYPE                            │
└─────────────────────────────────────────────────────────────┘
         │              │              │              │
         ▼              ▼              ▼              ▼
    ┌─────────┐   ┌──────────┐   ┌──────────┐   ┌──────────┐
    │ POROUS  │   │ FRACTURED│   │ CAVERNOUS│   │ INDUCED  │
    │ SAND/   │   │ FORMATION│   │ FORMATION│   │ FRACTURE │
    │ GRAVEL  │   │          │   │          │   │          │
    └─────────┘   └──────────┘   └──────────┘   └──────────┘
         │              │              │              │
         ▼              ▼              ▼              ▼
┌─────────────────────────────────────────────────────────────┐
│                    LCM SELECTION                            │
└─────────────────────────────────────────────────────────────┘
```

### LCM Selection by Loss Type

```
POROUS FORMATION:
┌─────────────────────────────────────────────────────────────┐
│ • Fine to medium granular LCM                              │
│ • Ground nut shells, calcium carbonate                     │
│ • Sized to match pore throats (1/3 to 1/2 pore size)      │
│ • Concentration: 20-40 lb/bbl                              │
└─────────────────────────────────────────────────────────────┘

FRACTURED FORMATION:
┌─────────────────────────────────────────────────────────────┐
│ • Flaky/fibrous LCM + granular blend                       │
│ • Mica, cellophane, cedar fiber + nut plug                 │
│ • Need bridging across fracture width                      │
│ • Concentration: 30-50 lb/bbl                              │
│ • May need high-fluid-loss squeeze                         │
└─────────────────────────────────────────────────────────────┘

CAVERNOUS/VUGGY:
┌─────────────────────────────────────────────────────────────┐
│ • Coarse granular + fibrous                                │
│ • Large nut plug, cedar bark, fiber                        │
│ • May need cement plug or gunk squeeze                     │
│ • Concentration: 50-100 lb/bbl                             │
│ • Often requires multiple treatments                       │
└─────────────────────────────────────────────────────────────┘

INDUCED FRACTURE (MW too high):
┌─────────────────────────────────────────────────────────────┐
│ • Reduce MW if possible (maintain well control!)           │
│ • Medium/coarse LCM                                        │
│ • Consider reducing ECD (flow rate, rotation)              │
│ • May need to set casing                                   │
└─────────────────────────────────────────────────────────────┘
```

### LCM Pill Spotting Procedure

```
┌─────────────────────────────────────────────────────────────┐
│              LCM PILL SPOTTING                              │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│ 1. Position bit above loss zone (50-100 ft)                │
│    • Know where losses started                             │
│    • Use drilling breaks, returns as indicators            │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│ 2. Mix LCM pill in slug pit                                │
│    • Volume: 25-50 bbl typical                             │
│    • Higher concentration for larger losses                │
│    • Mix blend of sizes                                    │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│ 3. Pump pill at reduced rate                               │
│    • 2-4 bpm typical                                       │
│    • Too fast = bypass zone                                │
│    • Too slow = settling in string                         │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│ 4. Chase with mud to position pill at loss zone            │
│    • Calculate displacement volume                         │
│    • Over-displace by 50% to ensure coverage               │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│ 5. Shut in and wait (squeeze optional)                     │
│    • 30-60 minutes minimum                                 │
│    • Light squeeze pressure if possible (200-500 psi)      │
│    • Allow LCM to set and dehydrate                        │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│ 6. Slowly break circulation                                │
│    • Start at 1-2 bpm                                      │
│    • Check returns                                         │
│    • If losses stopped, resume operations                  │
│    • If still losing, repeat or escalate treatment         │
└─────────────────────────────────────────────────────────────┘
```

## Total/Severe Losses (>50 bbl/hr)

```
┌─────────────────────────────────────────────────────────────┐
│                    TOTAL LOSSES                             │
│              >50 bbl/hr or complete loss                    │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│         CRITICAL: ASSESS WELL CONTROL RISK                  │
│    • Is there influx potential?                            │
│    • Maintain annulus full if possible                     │
│    • Consider U-tube effects                               │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
              ┌───────────────────────────────┐
              │  CAN MAINTAIN FULL ANNULUS?   │
              └───────────────────────────────┘
                     │              │
                 YES │              │ NO
                     ▼              ▼
         ┌───────────────┐   ┌───────────────────────┐
         │ Continue LCM  │   │ CRITICAL SITUATION    │
         │ treatments    │   │ • Fill annulus with   │
         │ May need      │   │   lighter fluid/foam  │
         │ cement plug   │   │ • Pump continuously   │
         └───────────────┘   │ • Consider kill mud   │
                             │   through annulus     │
                             └───────────────────────┘
                              │
                              ▼
```

### Cement Plug Decision

```
┌─────────────────────────────────────────────────────────────┐
│          WHEN TO USE CEMENT PLUG                            │
│                                                             │
│  • Multiple LCM treatments failed                          │
│  • Losses are cavernous/vuggy                              │
│  • Loss zone is defined and isolated                       │
│  • Time/cost of LCM treatments exceeds cement option       │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│              CEMENT PLUG PROCEDURE                          │
│                                                             │
│  1. Condition hole, establish circulation if possible      │
│  2. Spot cement across loss zone                           │
│     • Use balanced plug or dump bailer                     │
│     • Consider thixotropic or foamed cement                │
│  3. Pull out of cement, displace above plug                │
│  4. Wait on cement (WOC) - minimum 8-12 hours              │
│  5. Tag cement, drill out if successful                    │
│  6. Test formation before continuing                       │
└─────────────────────────────────────────────────────────────┘
```

### Gunk Squeeze (Diesel-Bentonite-Cement)

```
┌─────────────────────────────────────────────────────────────┐
│              GUNK SQUEEZE APPLICATION                       │
│                                                             │
│  For severe/total losses where LCM ineffective             │
│  Works by: Diesel + bentonite reacts with water            │
│            to create rapid-setting plug                    │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│  GUNK FORMULA (typical):                                   │
│  • Diesel: 1 bbl                                           │
│  • Bentonite: 200-400 lb                                   │
│  • Cement: 50-100 lb (optional, increases strength)        │
│                                                             │
│  Mix bentonite in diesel (won't react until water contact) │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│  PROCEDURE:                                                │
│  1. Mix gunk pill in slug tank                             │
│  2. Pump gunk to loss zone                                 │
│  3. Chase with water spacer (triggers reaction)            │
│  4. Apply squeeze pressure (500-1000 psi)                  │
│  5. Wait 2-4 hours                                         │
│  6. Attempt circulation                                    │
└─────────────────────────────────────────────────────────────┘
```

## LCM Quick Reference Table

| Loss Rate | LCM Type | Concentration | Treatment Method |
|-----------|----------|---------------|------------------|
| Seepage <10 bbl/hr | Fine (nut, mica) | 5-15 lb/bbl | Add to system |
| Partial 10-30 bbl/hr | Fine-Medium blend | 20-40 lb/bbl | LCM pill, circulate |
| Partial 30-50 bbl/hr | Medium-Coarse blend | 40-60 lb/bbl | LCM squeeze |
| Severe 50-100 bbl/hr | Coarse + fiber | 60-100 lb/bbl | Multiple squeezes |
| Total >100 bbl/hr | Gunk or cement | N/A | Squeeze/plug |

## LCM Materials Reference

| Material | Size Grade | Best For | Notes |
|----------|------------|----------|-------|
| Ground walnut | F/M/C | Porous formations | Acid soluble |
| Nut plug | F/M/C | General use | Good bridging |
| Mica | F/M/C | Fractured zones | Platelet shape |
| Cellophane | F/M | Fractured zones | Flake form |
| Cedar fiber | M/C | Cavernous | Fibrous mat |
| Calcium carbonate | F/M | Reservoir zones | Acid soluble |
| Gilsonite | M | Seepage | Temp sensitive |
| Graphite | F/M | Seepage | Lubricating |

F = Fine, M = Medium, C = Coarse

## Prevention Strategies

```
BEFORE DRILLING INTO KNOWN LOSS ZONES:
┌─────────────────────────────────────────────────────────────┐
│ • Pre-treat mud with LCM                                   │
│ • Reduce MW to minimum safe weight                         │
│ • Reduce flow rate (lower ECD)                             │
│ • Reduce ROP to minimize surge                             │
│ • Have LCM materials staged and ready                      │
│ • Consider managed pressure drilling (MPD)                 │
│ • Set casing above loss zone if severe anticipated         │
└─────────────────────────────────────────────────────────────┘
```

---

*Lost circulation treatment is often iterative. Document all treatments and results for optimization.*
