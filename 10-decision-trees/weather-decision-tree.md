# Weather Decision Tree

## Weather Monitoring

```
┌─────────────────────────────────────────────────────────────┐
│              CONTINUOUS WEATHER MONITORING                  │
│                                                             │
│    Sources:                                                │
│    • National Weather Service                              │
│    • Commercial weather services                           │
│    • Rig weather station                                   │
│    • Visual observation                                    │
│    • Marine forecasts (offshore)                           │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
              ┌───────────────────────────────┐
              │   HAZARDOUS WEATHER           │
              │   DETECTED/FORECAST?          │
              └───────────────────────────────┘
                     │              │
                 YES │              │ NO
                     ▼              ▼
         ┌───────────────┐   ┌───────────────┐
         │ Determine     │   │ Continue      │
         │ weather type  │   │ monitoring    │
         │ and severity  │   │               │
         └───────────────┘   └───────────────┘
                │
    ┌───────────┼───────────┬───────────┬───────────┐
    ▼           ▼           ▼           ▼           ▼
┌────────┐ ┌────────┐ ┌────────┐ ┌────────┐ ┌────────┐
│LIGHTNING│ │ HIGH   │ │TORNADO/│ │TROPICAL│ │EXTREME │
│        │ │ WIND   │ │SEVERE  │ │ STORM  │ │ TEMP   │
└────────┘ └────────┘ └────────┘ └────────┘ └────────┘
```

## Lightning Decision Tree

```
┌─────────────────────────────────────────────────────────────┐
│                    LIGHTNING                                │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
              ┌───────────────────────────────┐
              │   LIGHTNING DETECTION         │
              │   (Within 10 miles)           │
              └───────────────────────────────┘
                     │              │
         30-SECOND   │              │ FLASH-BANG
         RULE        │              │ <30 SECONDS
                     ▼              ▼
┌───────────────────────────────────────────────────────────┐
│              IMMEDIATE ACTIONS                             │
│                                                            │
│ 1. SUSPEND outdoor operations                              │
│ 2. Personnel to safe shelter                               │
│ 3. Secure crane operations                                 │
│ 4. Secure derrick work                                     │
│ 5. Halt perforating/explosives operations                  │
│ 6. Disconnect non-essential electrical                     │
└───────────────────────────────────────────────────────────┘
                              │
                              ▼
┌───────────────────────────────────────────────────────────┐
│              OPERATIONS THAT CAN CONTINUE                  │
│                                                            │
│ • Drilling (in derrick enclosure)                         │
│ • Circulation                                              │
│ • Monitoring (in doghouse/control room)                   │
│                                                            │
│              MUST STOP:                                    │
│ • Crane operations                                         │
│ • Derrick board work                                       │
│ • Any outdoor work                                         │
│ • Loading/unloading                                        │
│ • Explosives handling                                      │
│ • Wireline with explosives                                 │
└───────────────────────────────────────────────────────────┘
                              │
                              ▼
┌───────────────────────────────────────────────────────────┐
│              RESUME OPERATIONS                             │
│                                                            │
│ Wait 30 minutes after last lightning/thunder              │
│ before resuming outdoor operations                        │
└───────────────────────────────────────────────────────────┘
```

## High Wind Decision Tree

```
┌─────────────────────────────────────────────────────────────┐
│                    HIGH WIND                                │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
              ┌───────────────────────────────┐
              │      WIND SPEED?              │
              └───────────────────────────────┘
         │          │          │          │
    <20 MPH    20-35 MPH   35-50 MPH    >50 MPH
         │          │          │          │
         ▼          ▼          ▼          ▼
    ┌─────────┐ ┌─────────┐ ┌─────────┐ ┌─────────┐
    │ NORMAL  │ │CAUTION  │ │RESTRICT │ │ SHUT    │
    │ OPS     │ │         │ │ OPS     │ │ DOWN    │
    └─────────┘ └─────────┘ └─────────┘ └─────────┘
         │          │          │          │
         ▼          ▼          ▼          ▼

20-35 MPH (CAUTION):
┌─────────────────────────────────────────────────────────────┐
│ • Heightened awareness for crane operations               │
│ • Secure loose materials                                   │
│ • Monitor for gusts                                        │
│ • Review lift plans for wind limits                        │
│ • Prepare for escalation                                   │
└─────────────────────────────────────────────────────────────┘

35-50 MPH (RESTRICTED OPERATIONS):
┌─────────────────────────────────────────────────────────────┐
│ STOP:                                                      │
│ • Crane operations                                         │
│ • Man-riding operations                                    │
│ • Derrick work above monkey board                         │
│ • Rig-up/rig-down operations                              │
│                                                            │
│ CONTINUE WITH CAUTION:                                     │
│ • Drilling operations                                      │
│ • Essential circulation                                    │
│                                                            │
│ PREPARE:                                                   │
│ • Secure all loose equipment                              │
│ • Position emergency equipment                             │
│ • Review shutdown procedures                               │
└─────────────────────────────────────────────────────────────┘

>50 MPH (SHUTDOWN):
┌─────────────────────────────────────────────────────────────┐
│ • Suspend ALL operations                                   │
│ • Secure well (safe position)                             │
│ • All personnel to shelter                                 │
│ • Lower cranes and secure                                  │
│ • Secure all loose items                                   │
│ • Continuous monitoring                                    │
│ • Prepare for evacuation if conditions worsen             │
└─────────────────────────────────────────────────────────────┘
```

## Tornado/Severe Thunderstorm

```
┌─────────────────────────────────────────────────────────────┐
│                TORNADO WARNING                              │
│           (Tornado sighted or indicated)                   │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│              IMMEDIATE ACTIONS                              │
│                                                             │
│ 1. SOUND ALARM - three long blasts                        │
│ 2. ALL personnel evacuate derrick immediately             │
│ 3. Seek shelter in designated tornado shelter             │
│    or lowest interior room                                 │
│ 4. If no shelter: lie flat in ditch/low area             │
│ 5. Stay away from windows, vehicles, equipment            │
│ 6. DO NOT stay in trailers                                │
│ 7. Account for all personnel                              │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│              WELL OPERATIONS                                │
│                                                             │
│ If time permits (tornado >15 min away):                   │
│ • Set pipe on slips                                        │
│ • Close BOPs                                               │
│ • Shut down pumps                                          │
│ • Evacuate floor                                           │
│                                                             │
│ If imminent: EVACUATE IMMEDIATELY                         │
│ Personnel safety takes priority over equipment            │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│              AFTER TORNADO PASSES                          │
│                                                             │
│ 1. Wait for all-clear                                      │
│ 2. Account for all personnel                              │
│ 3. Check for injuries - provide first aid                 │
│ 4. Assess damage before resuming                          │
│ 5. Check well integrity                                    │
│ 6. Inspect all equipment before use                       │
│ 7. Report damage to supervision                           │
└─────────────────────────────────────────────────────────────┘
```

## Tropical Storm/Hurricane (Offshore)

```
┌─────────────────────────────────────────────────────────────┐
│          TROPICAL STORM/HURRICANE APPROACHING              │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
              ┌───────────────────────────────┐
              │   DISTANCE/TIME TO IMPACT?    │
              └───────────────────────────────┘
    │              │              │              │
    ▼              ▼              ▼              ▼
┌────────────┐┌────────────┐┌────────────┐┌────────────┐
│ 120+ HRS   ││ 72 HRS     ││ 48 HRS     ││ 24 HRS     │
│ MONITOR    ││ PREPARE    ││ SECURE     ││ EVACUATE   │
└────────────┘└────────────┘└────────────┘└────────────┘
      │              │              │              │
      ▼              ▼              ▼              ▼

120+ HOURS (MONITOR):
┌─────────────────────────────────────────────────────────────┐
│ • Track storm path every 6 hours                          │
│ • Review hurricane procedures                              │
│ • Inventory emergency supplies                             │
│ • Verify POB (personnel on board) list                    │
│ • Coordinate with logistics                                │
└─────────────────────────────────────────────────────────────┘

72 HOURS (PREPARE):
┌─────────────────────────────────────────────────────────────┐
│ • Begin well securing preparations                         │
│ • Prioritize completion of critical operations            │
│ • Arrange evacuation transportation                        │
│ • Reduce non-essential POB                                 │
│ • Top off fuel and water                                   │
│ • Prepare to run hurricane hanger                         │
│ • Inform shore base of status                              │
└─────────────────────────────────────────────────────────────┘

48 HOURS (SECURE):
┌─────────────────────────────────────────────────────────────┐
│ • Complete well operations to safe point                  │
│ • Run hurricane hanger (subsea)                           │
│ • Displace to weighted mud                                 │
│ • Secure all loose equipment                               │
│ • Begin non-essential personnel evacuation                │
│ • Crane to park position                                   │
│ • Prepare production system shutdown (if producing)       │
└─────────────────────────────────────────────────────────────┘

24 HOURS (EVACUATE):
┌─────────────────────────────────────────────────────────────┐
│ • EVACUATE ALL PERSONNEL                                   │
│ • Final well status verification                           │
│ • Confirm all safety systems armed                         │
│ • Final equipment securing                                 │
│ • Document final rig condition                             │
│ • Last helicopter/boat departure                           │
│ • Activate emergency beacons                               │
└─────────────────────────────────────────────────────────────┘
```

## Extreme Temperature

### Extreme Cold
```
┌─────────────────────────────────────────────────────────────┐
│              EXTREME COLD (<32°F / 0°C)                    │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│              EQUIPMENT PROTECTION                           │
│                                                             │
│ • Keep all fluid systems circulating                       │
│ • Heat trace freeze-prone lines                            │
│ • Protect BOP hydraulic system                             │
│ • Monitor mud weight (temperature effects)                 │
│ • Keep water-based systems moving                          │
│ • Drain unused lines                                       │
│ • Add antifreeze to wash water systems                     │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│              PERSONNEL PROTECTION                           │
│                                                             │
│ • Mandatory cold weather PPE                               │
│ • Rotate outdoor work exposure                             │
│ • Provide warming shelters                                 │
│ • Monitor for hypothermia/frostbite                        │
│ • Increase break frequency                                 │
│ • Hot drinks available                                     │
└─────────────────────────────────────────────────────────────┘
```

### Extreme Heat
```
┌─────────────────────────────────────────────────────────────┐
│              EXTREME HEAT (>95°F / 35°C)                   │
│              OR HIGH HEAT INDEX                             │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│              PERSONNEL PROTECTION                           │
│                                                             │
│ • Mandatory hydration program                              │
│ • Schedule heavy work for cooler hours                     │
│ • Provide shade/cooling stations                           │
│ • Rotate crews frequently                                  │
│ • Monitor for heat stress symptoms                         │
│ • Use buddy system                                         │
│ • Acclimatization for new workers                          │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
              ┌───────────────────────────────┐
              │   HEAT INDEX >103°F?          │
              └───────────────────────────────┘
                     │              │
                 YES │              │ NO
                     ▼              ▼
┌─────────────────────────────────────────────────────────────┐
│ ADDITIONAL MEASURES:                                       │
│ • Stop non-essential outdoor work                         │
│ • Mandatory rest breaks every 30-45 min                   │
│ • First aid trained personnel on alert                    │
│ • Consider postponing heavy operations                    │
└─────────────────────────────────────────────────────────────┘
```

## Weather Decision Matrix

| Condition | Trigger | Restricted Ops | Suspend All |
|-----------|---------|----------------|-------------|
| Lightning | Within 10 mi | Outdoor work | Explosives |
| Wind | 20-35 mph | Crane limits | >50 mph |
| Tornado | Warning issued | All outdoor | Immediate |
| Hurricane | 48 hrs out | Begin securing | 24 hrs out |
| Cold | <32°F | Monitor personnel | <-20°F w/wind |
| Heat | >95°F | Heavy labor | Heat index >115°F |
| Heavy Rain | Visibility <¼ mi | Crane, heights | Flash flood |
| Fog | Visibility <500 ft | Crane, helicopter | <100 ft |

## Documentation

```
┌─────────────────────────────────────────────────────────────┐
│           WEATHER EVENT DOCUMENTATION                       │
│                                                             │
│ For any weather-related operational change:                │
│                                                             │
│ 1. Date and time of decision                               │
│ 2. Weather conditions (specific measurements)             │
│ 3. Operations suspended or modified                        │
│ 4. Personnel actions taken                                 │
│ 5. Duration of restriction                                 │
│ 6. Conditions at resumption                                │
│ 7. Any incidents or damage                                 │
│                                                             │
│ Record in:                                                 │
│ • Daily drilling report                                    │
│ • Tour sheet                                               │
│ • IADC report                                              │
└─────────────────────────────────────────────────────────────┘
```

---

*When in doubt about weather conditions, err on the side of caution. No operation is worth risking personnel safety.*
