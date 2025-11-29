# Wellbore Instability Decision Tree

## Instability Detection

```
┌─────────────────────────────────────────────────────────────┐
│           WELLBORE INSTABILITY INDICATORS                   │
│                                                             │
│ Warning Signs:                                             │
│ • Increasing drag/torque trends                            │
│ • Cavings in returns                                       │
│ • Tight spots while tripping                               │
│ • Hole fill after connections                              │
│ • Overpull required to move string                         │
│ • Erratic ROP                                              │
│ • Formation breakdown/mud losses                           │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
              ┌───────────────────────────────┐
              │   IDENTIFY PROBLEM TYPE       │
              └───────────────────────────────┘
    │              │              │              │
    ▼              ▼              ▼              ▼
┌────────────┐ ┌────────────┐ ┌────────────┐ ┌────────────┐
│ SHALE      │ │HOLE        │ │ FORMATION  │ │ UNCONSOLID-│
│ INSTABILITY│ │ COLLAPSE   │ │ BREAKDOWN  │ │ ATED SANDS │
└────────────┘ └────────────┘ └────────────┘ └────────────┘
```

## Shale Instability

```
┌─────────────────────────────────────────────────────────────┐
│                 SHALE INSTABILITY                           │
│                                                             │
│ SYMPTOMS:                                                  │
│ • Splintery, angular cavings                               │
│ • Shale swelling indicators                                │
│ • Increasing torque and drag                               │
│ • Bit balling in gumbo shales                              │
│ • Tight hole conditions                                    │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
              ┌───────────────────────────────┐
              │      WHAT TYPE OF SHALE?      │
              └───────────────────────────────┘
         │                   │                   │
         ▼                   ▼                   ▼
┌───────────────┐   ┌───────────────┐   ┌───────────────┐
│ REACTIVE/     │   │ BRITTLE       │   │ OVERPRESSURED │
│ SWELLING      │   │ (STRESS)      │   │ SHALE         │
└───────────────┘   └───────────────┘   └───────────────┘
         │                   │                   │
         ▼                   ▼                   ▼

REACTIVE/SWELLING SHALE:
┌─────────────────────────────────────────────────────────────┐
│ CAUSE: Clay hydration from water-based mud                │
│                                                             │
│ SOLUTIONS:                                                 │
│ 1. Increase salinity (KCl, NaCl)                          │
│ 2. Add shale inhibitors (glycols, amines)                 │
│ 3. Increase mud weight (adds stress to stabilize)         │
│ 4. Consider converting to OBM/SBM                         │
│ 5. Minimize exposure time                                  │
│ 6. Run casing ASAP                                         │
└─────────────────────────────────────────────────────────────┘

BRITTLE/STRESS SHALE:
┌─────────────────────────────────────────────────────────────┐
│ CAUSE: Mechanical failure due to stress concentration     │
│                                                             │
│ CAVINGS APPEAR: Blocky, angular, splintery                │
│                                                             │
│ SOLUTIONS:                                                 │
│ 1. Increase mud weight (support borehole wall)            │
│ 2. Minimize swab/surge                                     │
│ 3. Reduce doglegs (stress concentration)                  │
│ 4. Optimize well trajectory                                │
│ 5. Time-dependent - run casing before failure             │
└─────────────────────────────────────────────────────────────┘

OVERPRESSURED SHALE:
┌─────────────────────────────────────────────────────────────┐
│ CAUSE: Underbalanced condition in shale                   │
│                                                             │
│ INDICATORS:                                                │
│ • Increasing d-exponent                                    │
│ • Gas shows                                                │
│ • Cavings with fresh appearance                            │
│                                                             │
│ SOLUTIONS:                                                 │
│ 1. Increase mud weight                                     │
│ 2. Monitor pore pressure indicators                        │
│ 3. D-exponent, gas, cuttings analysis                     │
│ 4. May need LOT to verify MW margin                        │
└─────────────────────────────────────────────────────────────┘
```

## Hole Collapse

```
┌─────────────────────────────────────────────────────────────┐
│                    HOLE COLLAPSE                            │
│                                                             │
│ SYMPTOMS:                                                  │
│ • Large volumes of cavings                                 │
│ • Pack-offs                                                │
│ • Cannot reach bottom                                      │
│ • Sudden increases in torque                               │
│ • Well takes weight unexpectedly                           │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│               IMMEDIATE ACTIONS                             │
│                                                             │
│ 1. Pick up off bottom                                      │
│ 2. Increase circulation rate                               │
│ 3. Work pipe to clear annulus                              │
│ 4. Circulate bottoms up - evaluate cavings                │
│ 5. Consider increasing mud weight                          │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│            ANALYZE CAVING TYPE                              │
│                                                             │
│ SPLINTERY/ANGULAR:                                         │
│ → Stress-related failure, increase MW                      │
│                                                             │
│ BLOCKY/TABULAR:                                            │
│ → Bedding plane failure, may need to change trajectory    │
│                                                             │
│ ROUNDED/SOFT:                                              │
│ → Chemical instability, improve inhibition                 │
│                                                             │
│ LARGE CHUNKS:                                              │
│ → Massive failure, may need to set casing                 │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
              ┌───────────────────────────────┐
              │   IS MUD WEIGHT AT MAXIMUM    │
              │   (near frac gradient)?       │
              └───────────────────────────────┘
                     │              │
                 YES │              │ NO
                     ▼              ▼
         ┌───────────────┐   ┌───────────────────────┐
         │ Limited       │   │ Increase MW in small  │
         │ options:      │   │ increments (0.2-0.5   │
         │ • Set casing  │   │ ppg) until stable     │
         │ • Sidetrack   │   │                       │
         │ • Underream   │   │ Monitor frac gradient │
         └───────────────┘   └───────────────────────┘
```

## Formation Breakdown (Induced Fracturing)

```
┌─────────────────────────────────────────────────────────────┐
│               FORMATION BREAKDOWN                           │
│         (Mud Weight Too High / ECD Issues)                 │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│ SYMPTOMS:                                                  │
│ • Lost circulation                                         │
│ • Break in cuttings returns                                │
│ • Decreasing pit volume                                    │
│ • Unable to maintain returns                               │
│ • May have induced kick (lost returns → underbalance)     │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
              ┌───────────────────────────────┐
              │   CAN REDUCE MUD WEIGHT?      │
              │   (Still safe for pore        │
              │    pressure)                  │
              └───────────────────────────────┘
                     │              │
                 YES │              │ NO (narrow MW window)
                     ▼              ▼
         ┌───────────────┐   ┌───────────────────────┐
         │ 1. Reduce MW  │   │ MANAGED PRESSURE      │
         │    to minimum │   │ DRILLING OPTIONS:     │
         │    safe weight│   │ • MPD                 │
         │ 2. Reduce flow│   │ • ECD reduction tools │
         │    rate (ECD) │   │ • Foam/aerated mud    │
         │ 3. Reduce ROP │   │ • Set intermediate    │
         │ 4. Spot LCM   │   │   casing              │
         └───────────────┘   └───────────────────────┘
```

## Unconsolidated Sands

```
┌─────────────────────────────────────────────────────────────┐
│              UNCONSOLIDATED SANDS                           │
│                                                             │
│ SYMPTOMS:                                                  │
│ • Sand production in returns                               │
│ • Hole enlargement (caliper)                               │
│ • Difficulty running casing                                │
│ • Bridges forming                                          │
│ • Borehole sloughing                                       │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│                    SOLUTIONS                                │
│                                                             │
│ 1. Maintain adequate mud weight                            │
│ 2. Avoid swab/surge                                        │
│ 3. Use viscous sweeps to clean                            │
│ 4. Minimize exposure time                                  │
│ 5. Consider cementing/consolidation                        │
│ 6. Run casing as soon as possible                         │
│                                                             │
│ IF SEVERE:                                                 │
│ • Chemical consolidation treatment                         │
│ • Underreaming before casing                              │
│ • Pre-drilled liner                                        │
└─────────────────────────────────────────────────────────────┘
```

## Mud Weight Optimization

```
┌─────────────────────────────────────────────────────────────┐
│            MUD WEIGHT WINDOW MANAGEMENT                     │
│                                                             │
│            Fracture Gradient                                │
│         ══════════════════════                              │
│                    ↑                                        │
│             MW Operating Range                              │
│                    ↓                                        │
│         ══════════════════════                              │
│            Collapse Gradient                                │
│                    ↓                                        │
│            Pore Pressure                                    │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│         OPTIMAL MW POSITIONING                              │
│                                                             │
│ 1. Minimum MW = Pore Pressure + Trip Margin (0.2-0.5 ppg)  │
│                                                             │
│ 2. For shale stability, may need MW closer to collapse    │
│    gradient (higher than minimum)                          │
│                                                             │
│ 3. Maximum MW = Frac Gradient - ECD margin                 │
│                                                             │
│ 4. If window is narrow (<0.5 ppg), consider:              │
│    • Setting intermediate casing                           │
│    • MPD techniques                                        │
│    • Wellbore strengthening                                │
└─────────────────────────────────────────────────────────────┘
```

## ECD Management

```
┌─────────────────────────────────────────────────────────────┐
│           ECD REDUCTION STRATEGIES                          │
│                                                             │
│ When close to frac gradient:                              │
│                                                             │
│ 1. REDUCE FLOW RATE                                        │
│    • Lower circulation rate                                │
│    • Sacrifice hole cleaning efficiency                    │
│    • May need more sweeps                                  │
│                                                             │
│ 2. REDUCE ROTARY SPEED                                     │
│    • Lower RPM reduces annular friction                    │
│    • Balance with hole cleaning needs                      │
│                                                             │
│ 3. MODIFY MUD PROPERTIES                                   │
│    • Reduce PV (plastic viscosity)                         │
│    • Lower solids content                                  │
│    • Thin mud where possible                               │
│                                                             │
│ 4. REDUCE ROP                                              │
│    • Less cuttings = lower ECD                            │
│    • Slower drilling in problem zones                      │
│                                                             │
│ 5. USE ECD REDUCTION TOOLS                                 │
│    • Rotating control devices                              │
│    • CML (continuous mud logging)                          │
└─────────────────────────────────────────────────────────────┘
```

## Troubleshooting Summary Matrix

| Problem | Key Indicator | Primary Solution | Secondary |
|---------|--------------|------------------|-----------|
| Swelling shale | Tight hole, mushy cavings | Inhibition, salinity | OBM conversion |
| Stress shale | Angular cavings | Increase MW | Set casing |
| Overpressured | Gas, fresh cavings | Increase MW | Monitor PP |
| Hole collapse | Volume cavings, pack-off | Increase MW, clean | Set casing |
| Frac induced | Losses | Reduce MW, ECD | LCM, MPD |
| Unconsolidated | Sand in returns | MW, minimize time | Casing |

## Prevention Best Practices

```
┌─────────────────────────────────────────────────────────────┐
│              PREVENTION STRATEGIES                          │
│                                                             │
│ PRE-DRILL:                                                 │
│ • Review offset well data for problem zones                │
│ • Geomechanical modeling for MW window                     │
│ • Select appropriate mud system                            │
│ • Plan casing points for problem intervals                 │
│                                                             │
│ WHILE DRILLING:                                            │
│ • Monitor torque/drag trends continuously                  │
│ • Examine cuttings and cavings                             │
│ • Track pore pressure indicators                           │
│ • Minimize exposure time in unstable zones                 │
│ • Keep hole clean                                          │
│ • Maintain proper mud properties                           │
│                                                             │
│ TRIPPING:                                                  │
│ • Control swab/surge                                       │
│ • Circulate bottoms up before trips                        │
│ • Fill hole on trips out                                   │
│ • Watch for hole fill on trips in                         │
└─────────────────────────────────────────────────────────────┘
```

---

*Wellbore instability is often progressive. Early detection and response prevents major problems.*
