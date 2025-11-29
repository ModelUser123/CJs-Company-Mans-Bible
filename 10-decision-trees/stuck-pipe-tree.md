# Stuck Pipe Decision Tree

## Initial Detection

```
┌─────────────────────────────────────────────────────────────┐
│              STRING WILL NOT MOVE                           │
│    (Cannot rotate, reciprocate, or both)                   │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│           IMMEDIATE ACTIONS (First 5 minutes)              │
│                                                             │
│    1. Note depth and position                              │
│    2. Note hook load at stuck point                        │
│    3. Note rotary torque at stuck point                    │
│    4. Record time                                          │
│    5. Apply maximum safe overpull IMMEDIATELY              │
│       (Time is critical - don't wait!)                     │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
              ┌───────────────────────────────┐
              │    DID STRING COME FREE?      │
              └───────────────────────────────┘
                     │              │
                 YES │              │ NO
                     ▼              ▼
         ┌───────────────┐   ┌───────────────────────┐
         │ Resume ops    │   │ Begin stuck pipe      │
         │ Investigate   │   │ diagnosis             │
         │ root cause    │   │                       │
         └───────────────┘   └───────────────────────┘
```

## Diagnosis - Determine Sticking Mechanism

```
┌─────────────────────────────────────────────────────────────┐
│               DIAGNOSE STUCK TYPE                           │
│                                                             │
│    Key Questions:                                          │
│    • What was happening when stuck?                        │
│    • Can you rotate?                                       │
│    • Can you circulate?                                    │
│    • Where is the stuck point?                             │
└─────────────────────────────────────────────────────────────┘
                              │
              ┌───────────────┴───────────────┐
              │       WHEN DID IT OCCUR?       │
              └───────────────────────────────┘
         │              │              │              │
         ▼              ▼              ▼              ▼
┌─────────────┐  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐
│ WHILE       │  │ STATIC      │  │ DURING      │  │ DURING      │
│ DRILLING    │  │ (NOT MOVING)│  │ TRIPPING    │  │ REAMING     │
└─────────────┘  └─────────────┘  └─────────────┘  └─────────────┘
      │                │                │                │
      ▼                ▼                ▼                ▼
```

## Type 1: Differential Sticking

```
┌─────────────────────────────────────────────────────────────┐
│              DIFFERENTIAL STICKING                          │
│                                                             │
│  SYMPTOMS:                                                 │
│  • Occurred while stationary (static)                      │
│  • Across permeable zone (sandstone)                       │
│  • High overbalance pressure                               │
│  • CAN circulate                                           │
│  • CAN'T rotate or reciprocate freely                      │
│  • Free point is across permeable interval                 │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│              IMMEDIATE ACTIONS                              │
│                                                             │
│  1. Work string - apply max safe torque and overpull      │
│  2. Jar DOWN (counterintuitive but often more effective)  │
│  3. Apply steady overpull while jarring                   │
│  4. Reduce hydrostatic if possible (still safe)           │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│              SPOTTING FLUID (if working fails)             │
│                                                             │
│  1. Calculate stuck point depth (stretch calculation)      │
│  2. Spot oil-based or water-based spotting fluid          │
│     across stuck zone                                      │
│  3. Allow 4-8 hours soak time                             │
│  4. Work pipe periodically during soak                    │
│  5. If diesel-based: spot diesel/surfactant blend         │
│  6. If water-based: use commercial spotting fluid         │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
              ┌───────────────────────────────┐
              │         PIPE FREE?            │
              └───────────────────────────────┘
                     │              │
                 YES │              │ NO
                     ▼              ▼
         ┌───────────────┐   ┌───────────────────────┐
         │ Resume ops    │   │ Repeat spot & soak    │
         │ Address root  │   │ OR                    │
         │ cause         │   │ Back-off, sidetrack   │
         └───────────────┘   └───────────────────────┘
```

## Type 2: Mechanical Sticking

```
┌─────────────────────────────────────────────────────────────┐
│              MECHANICAL STICKING                            │
│                                                             │
│  CAUSES:                                                   │
│  • Key seat                                                │
│  • Undergauge hole                                         │
│  • Junk in hole                                            │
│  • Ledges/ledging                                          │
│  • Cement restriction                                      │
│  • Wellbore geometry (doglegs)                             │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
```

### Key Seat

```
┌─────────────────────────────────────────────────────────────┐
│                    KEY SEAT                                 │
│                                                             │
│  SYMPTOMS:                                                 │
│  • Stuck while tripping out                                │
│  • Tool joint hangs up at dogleg                           │
│  • Located at abrupt direction change                      │
│  • String will go down but not up                          │
│  • CAN circulate                                           │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│                    ACTIONS                                  │
│                                                             │
│  1. Apply steady overpull with rotation                    │
│  2. Jar UP                                                 │
│  3. Work string up and down                                │
│  4. If jars not available, may need to work back down     │
│     and run key seat wiper/reamer                          │
│  5. Ream through dogleg area on return                     │
└─────────────────────────────────────────────────────────────┘
```

### Undergauge Hole

```
┌─────────────────────────────────────────────────────────────┐
│                 UNDERGAUGE HOLE                             │
│                                                             │
│  SYMPTOMS:                                                 │
│  • Stuck while tripping in or drilling ahead               │
│  • Reactive shales or swelling clays                       │
│  • Salt sections (creeping salt)                           │
│  • Tight spots noted during tripping                       │
│  • Cannot circulate (bit packed off)                       │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│                    ACTIONS                                  │
│                                                             │
│  1. Apply max torque and attempt to ream through           │
│  2. Jar both directions                                    │
│  3. Circulate if possible with max flow rate               │
│  4. Consider spotting oil pill on reactive shales          │
│  5. May need to back-off above stuck point                 │
│  6. Run reamer or hole opener before bit                   │
└─────────────────────────────────────────────────────────────┘
```

### Junk in Hole

```
┌─────────────────────────────────────────────────────────────┐
│                  JUNK IN HOLE                               │
│                                                             │
│  SYMPTOMS:                                                 │
│  • Sudden sticking, no warning                             │
│  • Metal fragments in returns                              │
│  • Known lost equipment in hole                            │
│  • Cannot rotate or reciprocate                            │
│  • Circulation may be blocked                              │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│                    ACTIONS                                  │
│                                                             │
│  1. DO NOT force rotation (can worsen)                     │
│  2. Jar up and down gently                                 │
│  3. Circulate to clear if possible                         │
│  4. May need to back-off and fish                          │
│  5. Junk basket or magnet run may be needed                │
└─────────────────────────────────────────────────────────────┘
```

## Type 3: Pack-Off / Wellbore Instability

```
┌─────────────────────────────────────────────────────────────┐
│              PACK-OFF / HOLE COLLAPSE                       │
│                                                             │
│  SYMPTOMS:                                                 │
│  • Increasing drag and torque before stuck                 │
│  • Cavings in returns (shale, coal)                        │
│  • Bridges forming                                         │
│  • Cannot circulate OR very high pump pressure             │
│  • Often in shale sections or unconsolidated zones         │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│                    ACTIONS                                  │
│                                                             │
│  1. DO NOT pull excessively (can swab more cavings)        │
│  2. Attempt circulation - increase MW if needed            │
│  3. Work pipe gently to maintain movement                  │
│  4. Jar both directions                                    │
│  5. Circulate at max rate to clean hole                    │
│  6. May need to increase mud weight                        │
│  7. Spotting viscous sweeps may help                       │
└─────────────────────────────────────────────────────────────┘
```

## Free Point Calculation

```
┌─────────────────────────────────────────────────────────────┐
│              FREE POINT CALCULATION                         │
│                                                             │
│  Method: Pipe Stretch Measurement                          │
│                                                             │
│  L = (735,294 × E × W) ÷ (P × ΔL)                         │
│                                                             │
│  Where:                                                    │
│  L = Free point depth (ft)                                 │
│  E = Stretch (inches)                                      │
│  W = Weight of pipe (lb/ft)                                │
│  P = Applied overpull (lb)                                 │
│  ΔL = Measured stretch at overpull (inches)                │
│                                                             │
│  SIMPLIFIED: Free Point ≈ Stretch (in) × 1000 × (lb/ft ÷   │
│              Overpull in thousands)                        │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│  EXAMPLE:                                                  │
│  • 5" DP at 19.5 lb/ft                                     │
│  • Applied 50,000 lb overpull                              │
│  • Measured 15 inches of stretch                           │
│                                                             │
│  Free Point ≈ (735,294 × 15 × 19.5) ÷ (50,000 × 15)       │
│             ≈ 2,865 ft                                     │
└─────────────────────────────────────────────────────────────┘
```

## Back-Off Procedure

```
┌─────────────────────────────────────────────────────────────┐
│        WHEN ALL FREEING ATTEMPTS FAIL                       │
│              BACK-OFF PROCEDURE                             │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│ 1. Run free point indicator to confirm stuck depth         │
│    • Electric or mechanical                                │
│    • Correlate with calculated free point                  │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│ 2. Select back-off depth                                   │
│    • Above stuck point in free pipe                        │
│    • At tool joint (easier to back off)                    │
│    • Consider what can be recovered vs abandoned           │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│ 3. Apply left-hand torque                                  │
│    • Apply 75-80% of make-up torque in reverse             │
│    • Hold torque steady                                    │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│ 4. Detonate string shot                                    │
│    • Position prima cord at selected depth                 │
│    • Fire while holding left-hand torque                   │
│    • Connection should unscrew                             │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│ 5. Recover free string                                     │
│    • Pull out of hole with free pipe                       │
│    • Inspect thread condition                              │
│    • Plan fishing operation or sidetrack                   │
└─────────────────────────────────────────────────────────────┘
```

## Decision: Fish or Sidetrack?

```
              ┌───────────────────────────────┐
              │     FISH OR SIDETRACK?        │
              └───────────────────────────────┘
                     │              │
         ┌───────────┘              └───────────┐
         ▼                                      ▼
┌─────────────────────────┐        ┌─────────────────────────┐
│      FISHING            │        │      SIDETRACK          │
│                         │        │                         │
│ Choose if:              │        │ Choose if:              │
│ • Fish is simple shape  │        │ • Fish is complex       │
│ • Fish is in open hole  │        │ • Multiple attempts     │
│ • High chance success   │        │   already failed        │
│ • Hole is stable        │        │ • Hole deteriorating    │
│ • Equipment is available│        │ • Time critical         │
│ • Low cost option       │        │ • Near TD anyway        │
│                         │        │ • Fish has no value     │
└─────────────────────────┘        └─────────────────────────┘
```

## Prevention Summary

```
┌─────────────────────────────────────────────────────────────┐
│              PREVENTION PRACTICES                           │
├─────────────────────────────────────────────────────────────┤
│                                                             │
│ DIFFERENTIAL STICKING:                                      │
│ • Keep pipe moving (rotate/reciprocate)                    │
│ • Minimize static time across permeable zones              │
│ • Maintain good filter cake quality                        │
│ • Minimize overbalance                                     │
│                                                             │
│ KEY SEATS:                                                 │
│ • Control dogleg severity                                  │
│ • Use key seat wipers                                      │
│ • Ream through doglegs                                     │
│                                                             │
│ HOLE INSTABILITY:                                          │
│ • Maintain proper MW for formation                         │
│ • Use inhibitive mud system                                │
│ • Minimize open hole exposure time                         │
│ • Circulate hole clean before trips                        │
│                                                             │
│ GENERAL:                                                   │
│ • Monitor drag trends                                      │
│ • Act quickly when stuck                                   │
│ • Maintain jars in working order                           │
│ • Have contingency plans                                   │
└─────────────────────────────────────────────────────────────┘
```

---

*Quick response is critical with stuck pipe. The longer you wait, the harder it becomes to free.*
