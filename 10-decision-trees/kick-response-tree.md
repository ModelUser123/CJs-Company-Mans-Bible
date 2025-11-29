# Kick Response Decision Tree

## Initial Kick Detection

```
┌─────────────────────────────────────────────────────────────┐
│                    PIT GAIN DETECTED                        │
│         (or flow with pumps off, drilling break)            │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│              STOP ALL OPERATIONS IMMEDIATELY                │
│    • Stop drilling/tripping                                 │
│    • Pick up off bottom (if drilling)                       │
│    • Space out tool joint from BOP                          │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│                 SHUT IN THE WELL                            │
│    • Close annular or pipe rams                             │
│    • Record shut-in time                                    │
│    • Open HCR line to choke manifold                        │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│              RECORD INITIAL PRESSURES                       │
│    • SIDPP (Shut-In Drill Pipe Pressure)                    │
│    • SICP (Shut-In Casing Pressure)                         │
│    • Pit gain volume                                        │
│    • Time to stabilize                                      │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
                    ┌─────────────────┐
                    │ SIDPP = SICP?   │
                    └─────────────────┘
                     │              │
                 YES │              │ NO
                     ▼              ▼
        ┌──────────────────┐  ┌──────────────────┐
        │ Possible causes: │  │ Normal kick      │
        │ • Plugged bit    │  │ SICP > SIDPP     │
        │ • Underground    │  │ indicates gas    │
        │   blowout        │  │ in annulus       │
        │ • Float failure  │  │                  │
        └──────────────────┘  └──────────────────┘
                              │
                              ▼
```

## Kill Method Selection

```
┌─────────────────────────────────────────────────────────────┐
│              CALCULATE KILL PARAMETERS                      │
│    • Kill Mud Weight = Current MW + (SIDPP ÷ 0.052 ÷ TVD)  │
│    • Initial Circulating Pressure (ICP)                     │
│    • Final Circulating Pressure (FCP)                       │
│    • Strokes to bit, strokes to surface                     │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
              ┌───────────────────────────────┐
              │ CAN YOU CIRCULATE?            │
              │ (Pumps working, no washout,   │
              │  bit not plugged)             │
              └───────────────────────────────┘
                     │              │
                 YES │              │ NO
                     ▼              ▼
         ┌───────────────┐   ┌───────────────────────┐
         │ SELECT KILL   │   │ VOLUMETRIC METHOD     │
         │ METHOD        │   │ or BULLHEADING        │
         └───────────────┘   │ See below             │
                │            └───────────────────────┘
                ▼
    ┌───────────────────────────────────────┐
    │ IS KICK SIZE < 20 BBL AND            │
    │ FORMATION RELATIVELY COMPETENT?       │
    └───────────────────────────────────────┘
           │                    │
       YES │                    │ NO
           ▼                    ▼
┌─────────────────────┐  ┌─────────────────────┐
│ DRILLER'S METHOD    │  │ WAIT & WEIGHT       │
│ (Two circulation)   │  │ (Engineer's Method) │
│                     │  │ (One circulation)   │
│ • Simpler           │  │                     │
│ • More time         │  │ • More complex      │
│ • Higher pressures  │  │ • Less time         │
│                     │  │ • Lower pressures   │
└─────────────────────┘  └─────────────────────┘
```

## Driller's Method Procedure

```
┌─────────────────────────────────────────────────────────────┐
│                 DRILLER'S METHOD                            │
│                First Circulation                            │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│ 1. Bring pump up to kill rate speed slowly                 │
│    • Hold casing pressure constant while bringing up       │
│    • Record circulating pressure at kill rate              │
│    • This should equal ICP (SIDPP + SCR pressure)          │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│ 2. Circulate maintaining CONSTANT DRILL PIPE PRESSURE      │
│    • DPP = ICP throughout first circulation                │
│    • Adjust choke to maintain DPP                          │
│    • Watch for gas expansion near surface                  │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│ 3. Continue until influx is circulated out                 │
│    • Returns at normal mud weight                          │
│    • Casing pressure = SIDPP (approximately)               │
│    • Pit level stabilized                                  │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│ 4. Shut in and verify                                      │
│    • SIDPP should equal original SIDPP                     │
│    • If SIDPP = 0, well may be dead (verify carefully)     │
│    • If SIDPP unchanged, weight up mud and repeat          │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│                Second Circulation                           │
│    • Weight up mud to kill weight                          │
│    • Circulate kill mud, holding DPP = ICP until           │
│      kill mud reaches bit                                  │
│    • Then hold DPP = FCP until returns are kill weight     │
│    • Shut in and verify SIDPP = SICP = 0                   │
└─────────────────────────────────────────────────────────────┘
```

## Wait & Weight Method

```
┌─────────────────────────────────────────────────────────────┐
│              WAIT & WEIGHT METHOD                           │
│            (Single Circulation)                             │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│ 1. Weight up mud to kill weight while shut in              │
│    • Calculate kill mud weight                             │
│    • Mix kill mud in pits                                  │
│    • Prepare kill sheet with step-down schedule            │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│ 2. Bring pump up slowly, holding casing pressure constant  │
│    • Record ICP when at kill rate                          │
│    • Begin pumping kill mud                                │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│ 3. Follow step-down schedule as kill mud goes down         │
│    • DPP decreases linearly from ICP to FCP                │
│    • Adjust choke to maintain scheduled DPP                │
│    • Kill mud reaches bit when DPP = FCP                   │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│ 4. Hold FCP constant until kill mud reaches surface        │
│    • Continue adjusting choke                              │
│    • Watch for gas expansion                               │
│    • Returns should be kill weight mud                     │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│ 5. Shut in and verify well is dead                         │
│    • SIDPP = 0                                             │
│    • SICP = 0                                              │
│    • No flow with pumps off                                │
└─────────────────────────────────────────────────────────────┘
```

## Volumetric Method (When Circulation Not Possible)

```
┌─────────────────────────────────────────────────────────────┐
│              VOLUMETRIC METHOD                              │
│    (For stripping, waiting on equipment, etc.)             │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│ Purpose: Allow gas to migrate while maintaining constant   │
│          bottomhole pressure                               │
│                                                            │
│ Key Principle:                                             │
│ As gas rises, it expands. Must bleed mud to prevent       │
│ excessive pressure buildup while maintaining BHP.          │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│ 1. Calculate pressure increment                            │
│    • Typically 50-100 psi                                  │
│    • Lower increment = more work but safer                 │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│ 2. Allow pressure to build by one increment                │
│    • Gas migrating causes pressure rise                    │
│    • Monitor SICP increase                                 │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│ 3. Bleed mud volume to drop pressure by one increment      │
│    • Volume = (Pressure increment × Annular capacity) ÷    │
│               (0.052 × Mud weight)                         │
│    • Example: 50 psi, 0.05 bbl/ft, 12 ppg mud             │
│      Volume = (50 × 0.05) ÷ (0.052 × 12) = 4 bbl/100 ft   │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│ 4. Repeat until gas is at surface                          │
│    • Continue build-bleed cycles                           │
│    • Net effect: gas moves up, pressure remains safe       │
└─────────────────────────────────────────────────────────────┘
```

## Special Situations

### Underground Blowout Suspected
```
Signs:
• SIDPP = SICP (or very close)
• Continuous pit loss
• No surface flow

Action:
1. DO NOT attempt conventional kill
2. Evaluate pressure data carefully
3. Consider bullheading if reservoir can take it
4. May need relief well planning
5. Consult well control specialists immediately
```

### Plugged Bit/String
```
Signs:
• Cannot establish circulation
• Pressure spikes when attempting to pump
• SIDPP building when pumping into closed system

Action:
1. Attempt to break loose with controlled pressure
2. Try spotting acid/solvent if LCM plugging
3. Use volumetric method while troubleshooting
4. May need to strip out and re-run
```

### Shallow Gas (Conductor/Surface Hole)
```
Signs:
• Flow during drilling shallow hole
• No casing set for BOP closure

Action:
1. EVACUATE NON-ESSENTIAL PERSONNEL
2. Divert flow away from rig if diverter installed
3. Keep pumping to maintain hydrostatic
4. Monitor for H2S
5. Never shut in on shallow gas without casing
```

## Key Formulas Quick Reference

| Parameter | Formula |
|-----------|---------|
| Kill Mud Weight | KMW = OMW + (SIDPP ÷ 0.052 ÷ TVD) |
| ICP | ICP = SIDPP + SCR Pressure |
| FCP | FCP = SCR × (KMW ÷ OMW) |
| MAASP | MAASP = (Frac Gradient - MW) × 0.052 × Shoe TVD |
| Hydrostatic | P = 0.052 × MW × TVD |

## Documentation Requirements

After every well control event, document:
- [ ] Time of kick detection
- [ ] Initial SIDPP and SICP
- [ ] Pit gain volume
- [ ] Kill parameters calculated
- [ ] Kill method used
- [ ] Circulation pressures throughout
- [ ] Total time to kill
- [ ] Root cause analysis
- [ ] Lessons learned

---

*This decision tree is a guide. Always follow company well control procedures and consult with specialists for complex situations.*
