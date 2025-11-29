# Equipment Failure Decision Tree

## Initial Equipment Failure Response

```
┌─────────────────────────────────────────────────────────────┐
│              EQUIPMENT FAILURE DETECTED                     │
│    (Abnormal operation, alarms, or complete failure)       │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│              IMMEDIATE SAFETY ASSESSMENT                    │
│                                                             │
│    1. Is there immediate danger to personnel?              │
│    2. Is well control at risk?                             │
│    3. Is there environmental hazard?                       │
│                                                             │
│    If YES to any: Initiate emergency response              │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│              IDENTIFY FAILED EQUIPMENT                      │
└─────────────────────────────────────────────────────────────┘
         │          │          │          │          │
         ▼          ▼          ▼          ▼          ▼
    ┌────────┐ ┌────────┐ ┌────────┐ ┌────────┐ ┌────────┐
    │ TOP    │ │ DRAWWORKS│ │ MUD    │ │ ROTARY │ │ POWER  │
    │ DRIVE  │ │        │ │ PUMPS  │ │ TABLE  │ │ SYSTEM │
    └────────┘ └────────┘ └────────┘ └────────┘ └────────┘
         │          │          │          │          │
         ▼          ▼          ▼          ▼          ▼
```

## Top Drive Failure

```
┌─────────────────────────────────────────────────────────────┐
│                  TOP DRIVE FAILURE                          │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
              ┌───────────────────────────────┐
              │     WHAT IS THE SYMPTOM?      │
              └───────────────────────────────┘
         │              │              │              │
         ▼              ▼              ▼              ▼
┌──────────────┐ ┌─────────────┐ ┌─────────────┐ ┌─────────────┐
│ NO ROTATION  │ │ VIBRATION/  │ │ WASHOUT/    │ │ ELECTRICAL  │
│              │ │ NOISE       │ │ LEAK        │ │ FAULT       │
└──────────────┘ └─────────────┘ └─────────────┘ └─────────────┘
      │                │              │                │
      ▼                ▼              ▼                ▼
┌─────────────────────────────────────────────────────────────┐
│ NO ROTATION TROUBLESHOOTING:                               │
│ 1. Check electrical supply (VFD faults, breakers)          │
│ 2. Check hydraulic pressure (if hydraulic drive)           │
│ 3. Verify motor engagement                                 │
│ 4. Check for mechanical binding                            │
│ 5. Inspect gearbox oil level and condition                 │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
              ┌───────────────────────────────┐
              │    CAN ISSUE BE REPAIRED      │
              │    ON LOCATION?               │
              └───────────────────────────────┘
                     │              │
                 YES │              │ NO
                     ▼              ▼
         ┌───────────────┐   ┌───────────────────────┐
         │ Repair and    │   │ OPTIONS:              │
         │ return to     │   │ • Call out service    │
         │ service       │   │ • Install backup unit │
         │               │   │ • Use rotary table    │
         └───────────────┘   │   (if equipped)       │
                             └───────────────────────┘
```

## Drawworks Failure

```
┌─────────────────────────────────────────────────────────────┐
│                 DRAWWORKS FAILURE                           │
│                                                             │
│    CRITICAL: Can you hold/lower pipe safely?               │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
              ┌───────────────────────────────┐
              │     WHAT IS THE SYMPTOM?      │
              └───────────────────────────────┘
         │              │              │              │
         ▼              ▼              ▼              ▼
┌──────────────┐ ┌─────────────┐ ┌─────────────┐ ┌─────────────┐
│ BRAKE        │ │ DRUM DOES   │ │ CLUTCH      │ │ MOTOR/      │
│ FAILURE      │ │ NOT ROTATE  │ │ SLIPPING    │ │ ELECTRICAL  │
└──────────────┘ └─────────────┘ └─────────────┘ └─────────────┘

BRAKE FAILURE - CRITICAL:
┌─────────────────────────────────────────────────────────────┐
│ EMERGENCY ACTIONS:                                         │
│ 1. Engage auxiliary brake IMMEDIATELY                      │
│ 2. Set slips if pipe in hole                               │
│ 3. Lower block to safe position                            │
│ 4. Secure area - no personnel under block                  │
│ 5. Do not operate until repaired                           │
│                                                             │
│ TROUBLESHOOTING:                                           │
│ • Check brake band wear                                    │
│ • Verify hydraulic pressure (if hydro-brake)               │
│ • Check cooling system                                     │
│ • Inspect drum for contamination (oil, water)              │
└─────────────────────────────────────────────────────────────┘

DRUM DOES NOT ROTATE:
┌─────────────────────────────────────────────────────────────┐
│ 1. Verify brake is released                                │
│ 2. Check motor power supply                                │
│ 3. Verify clutch engagement                                │
│ 4. Check for mechanical binding                            │
│ 5. Inspect transmission/gearing                            │
└─────────────────────────────────────────────────────────────┘
```

## Mud Pump Failure

```
┌─────────────────────────────────────────────────────────────┐
│                   MUD PUMP FAILURE                          │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
              ┌───────────────────────────────┐
              │     WHAT IS THE SYMPTOM?      │
              └───────────────────────────────┘
         │              │              │              │
         ▼              ▼              ▼              ▼
┌──────────────┐ ┌─────────────┐ ┌─────────────┐ ┌─────────────┐
│ NO DISCHARGE │ │ LOW         │ │ UNUSUAL     │ │ PUMP        │
│ PRESSURE     │ │ FLOW RATE   │ │ NOISE       │ │ KNOCKING    │
└──────────────┘ └─────────────┘ └─────────────┘ └─────────────┘

NO DISCHARGE PRESSURE:
┌─────────────────────────────────────────────────────────────┐
│ 1. Check suction (air in system, blocked strainer)         │
│ 2. Verify valves and liners for failure                    │
│    • Remove suction valve cover, inspect                   │
│    • Remove discharge valve cover, inspect                 │
│ 3. Check pulsation dampener charge                         │
│ 4. Verify power end operation                              │
│                                                             │
│ TYPICAL CAUSES:                                            │
│ • Washed valve seats (most common)                         │
│ • Cracked liner                                            │
│ • Plugged suction                                          │
│ • Air bound (cavitation)                                   │
└─────────────────────────────────────────────────────────────┘

PUMP KNOCKING:
┌─────────────────────────────────────────────────────────────┐
│ WARNING: Can indicate serious failure imminent             │
│                                                             │
│ 1. STOP PUMP IMMEDIATELY                                   │
│ 2. Check piston rod/crosshead clearance                    │
│ 3. Check main bearings for play                            │
│ 4. Verify pulsation dampener pre-charge                    │
│ 5. Check for cracked liners                                │
│ 6. Do not restart until issue identified                   │
└─────────────────────────────────────────────────────────────┘
```

### Mud Pump Valve Replacement

```
┌─────────────────────────────────────────────────────────────┐
│           VALVE/SEAT REPLACEMENT PROCEDURE                  │
│                                                             │
│ 1. Isolate pump (close suction, bleed pressure)            │
│ 2. Remove valve cover (suction or discharge)               │
│ 3. Remove retaining nut/spring                             │
│ 4. Extract valve and seat                                  │
│ 5. Inspect seat pocket for erosion                         │
│ 6. Install new seat (proper orientation)                   │
│ 7. Install new valve, spring, retainer                     │
│ 8. Replace cover with new gasket                           │
│ 9. Pressure test before returning to service               │
└─────────────────────────────────────────────────────────────┘
```

## Power System Failure

```
┌─────────────────────────────────────────────────────────────┐
│                 POWER SYSTEM FAILURE                        │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
              ┌───────────────────────────────┐
              │   PARTIAL OR TOTAL BLACKOUT?  │
              └───────────────────────────────┘
                     │              │
           PARTIAL   │              │ TOTAL
                     ▼              ▼
         ┌───────────────┐   ┌───────────────────────┐
         │ Single gen-   │   │ TOTAL BLACKOUT        │
         │ set failure   │   │ CRITICAL ACTIONS:     │
         │               │   │ 1. Engage emergency   │
         │ • Isolate     │   │    power/UPS          │
         │   failed unit │   │ 2. Verify well control│
         │ • Redistribute│   │    (accumulators)     │
         │   load        │   │ 3. Account for all    │
         │ • Troubleshoot│   │    personnel          │
         │   offline     │   │ 4. Secure any         │
         └───────────────┘   │    hazardous ops      │
                             └───────────────────────┘
                              │
                              ▼
GENERATOR TROUBLESHOOTING:
┌─────────────────────────────────────────────────────────────┐
│ 1. Check fuel supply and fuel filters                      │
│ 2. Verify oil pressure and level                           │
│ 3. Check coolant level and temperature                     │
│ 4. Inspect air filters                                     │
│ 5. Check electrical connections                            │
│ 6. Verify governor/AVR operation                           │
│ 7. Check for fault codes (electronic engines)              │
│                                                             │
│ COMMON ISSUES:                                             │
│ • Fuel starvation (filters, air in lines)                  │
│ • Overheating (coolant, fan, thermostat)                   │
│ • Electrical faults (breakers, connections)                │
│ • Governor malfunction                                     │
└─────────────────────────────────────────────────────────────┘
```

## BOP Equipment Failure

```
┌─────────────────────────────────────────────────────────────┐
│                   BOP FAILURE                               │
│              CRITICAL WELL CONTROL ISSUE                    │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
              ┌───────────────────────────────┐
              │     IS THE WELL FLOWING?      │
              └───────────────────────────────┘
                     │              │
                 YES │              │ NO
                     ▼              ▼
┌───────────────────────────────┐ ┌───────────────────────────┐
│ IMMEDIATE ACTIONS:            │ │ Troubleshoot but do NOT   │
│ 1. Close alternate preventer  │ │ resume operations until   │
│    (use secondary barrier)    │ │ BOP fully functional      │
│ 2. Activate accumulator       │ │                           │
│ 3. Notify supervision         │ │ • Run function tests      │
│ 4. Follow well control        │ │ • Pressure test as needed │
│    procedures                 │ │ • May need to POOH to     │
│                               │ │   inspect/repair          │
└───────────────────────────────┘ └───────────────────────────┘

BOP TROUBLESHOOTING:
┌─────────────────────────────────────────────────────────────┐
│                                                             │
│ WON'T CLOSE:                                               │
│ • Check accumulator pressure (minimum 1200 psi typical)    │
│ • Verify manifold position (correct valve open)            │
│ • Check for blocked control lines                          │
│ • Verify rams are correct size for pipe in hole            │
│ • Check control panel electrical/air supply                │
│                                                             │
│ WON'T OPEN:                                                │
│ • Check return line (pressure trapped)                     │
│ • Verify hydraulic supply                                  │
│ • May need to release pressure manually                    │
│                                                             │
│ LEAKING WHEN CLOSED:                                       │
│ • Ram elements may be damaged                              │
│ • Incorrect ram size for pipe                              │
│ • Debris preventing seal                                   │
│ • May need to pull to inspect (kill well first)            │
└─────────────────────────────────────────────────────────────┘
```

## Quick Troubleshooting Reference

| Equipment | Common Failure | First Check | Backup Plan |
|-----------|---------------|-------------|-------------|
| Top Drive | No rotation | VFD/electrical | Use rotary table |
| Drawworks | Brake slip | Band adjustment | Aux brake |
| Mud Pump | No pressure | Valves/seats | Standby pump |
| Generator | No power | Fuel supply | Other gen-sets |
| BOP | Won't close | Accumulator pressure | Secondary preventer |
| Air System | Low pressure | Compressor, leaks | Emergency start |

## Documentation Requirements

After any equipment failure:

```
┌─────────────────────────────────────────────────────────────┐
│               FAILURE DOCUMENTATION                         │
│                                                             │
│ 1. Time and date of failure                                │
│ 2. Equipment identification (serial numbers)               │
│ 3. Operations in progress when failed                      │
│ 4. Symptoms observed                                       │
│ 5. Troubleshooting steps taken                             │
│ 6. Root cause (if determined)                              │
│ 7. Parts replaced                                          │
│ 8. Repair performed by whom                                │
│ 9. Return to service time                                  │
│ 10. Any well control implications                          │
│ 11. Downtime cost estimate                                 │
└─────────────────────────────────────────────────────────────┘
```

---

*Never bypass safety systems during equipment repair. Use proper lockout/tagout procedures.*
