# Zipper Frac Operations

## Concept and Benefits

### What is Zipper Fracturing?

```
ZIPPER FRAC DEFINITION
├── Simultaneous completion of 2+ wells
├── Alternate pumping between wells
├── While one well pumps, other preps
├── Continuous pumping operations
└── Maximizes equipment utilization

OPERATIONAL SEQUENCE (2 Well)
├── Well A: Pump Stage 1
│   └── Well B: Prep Stage 1 (wireline)
├── Well B: Pump Stage 1
│   └── Well A: Prep Stage 2 (wireline)
├── Well A: Pump Stage 2
│   └── Well B: Prep Stage 2 (wireline)
└── Continue alternating...
```

### Benefits of Zipper Operations

| Benefit | Description | Impact |
|---------|-------------|--------|
| Efficiency | Continuous pumping | 20-40% time reduction |
| Cost | Less standby time | 15-25% cost reduction |
| Stress shadow | Enhanced fracture complexity | Better SRV |
| Equipment | Higher utilization | Lower cost per stage |
| Personnel | Optimized crew allocation | Reduced labor cost |

### Stress Shadow Effect

```
STRESS SHADOW MECHANISM
├── First Frac Creates Stress Change
│   ├── Compressional stress perpendicular
│   ├── Affects adjacent wells
│   └── Can enhance complexity
├── Timing Critical
│   ├── Must pump while stress still altered
│   ├── Typically within 2-4 hours
│   └── Pressure dependent
└── Benefits
    ├── More complex fracture network
    ├── Better near-wellbore geometry
    └── Enhanced SRV

OPTIMAL SPACING FOR STRESS SHADOW
├── Too Close: Frac hits (communication)
├── Too Far: No stress shadow benefit
├── Optimal: 400-800 ft typically
└── Formation dependent
```

## Zipper Configurations

### Standard 2-Well Zipper

```
2-WELL ZIPPER LAYOUT

Well A ←─── Pump ───→ Stages 1,3,5,7...
              ↕
          Manifold
              ↕
Well B ←─── Pump ───→ Stages 2,4,6,8...

SEQUENCE
├── Time 0-2 hrs: Well A Stage 1
├── Time 2-4 hrs: Well B Stage 1
├── Time 4-6 hrs: Well A Stage 2
├── Time 6-8 hrs: Well B Stage 2
└── Continue...

EFFICIENCY GAIN
├── Sequential: 4 hrs/stage × 80 stages = 320 hrs
├── Zipper: 2 hrs pumping × 80 = 160 hrs + prep
└── Net Savings: ~30-40%
```

### 3-Well Zipper

```
3-WELL ZIPPER SEQUENCE

Well A: Pump → Prep → Wait → Pump → Prep → Wait...
Well B: Wait → Pump → Prep → Wait → Pump → Prep...
Well C: Prep → Wait → Pump → Prep → Wait → Pump...

TIME ALLOCATION (Example)
├── Pump: 1.5-2 hours
├── Prep: 1.5-2 hours
├── Wait: 1.5-2 hours (pressure monitoring)
└── Cycle: ~6 hours total per well

ADVANTAGES
├── Higher equipment utilization
├── More stress shadow benefit
└── Larger economy of scale

CHALLENGES
├── More complex logistics
├── Greater coordination required
└── More surface equipment
```

### Simul-Frac Operations

```
SIMUL-FRAC (SIMULTANEOUS FRAC)
├── Definition
│   ├── Pump same stage on 2+ wells
│   ├── True simultaneous operations
│   └── Different from zipper
├── Requirements
│   ├── Double pumping capacity
│   ├── Dual blender/hydration
│   ├── Parallel treating lines
│   └── Coordinated wellheads
├── Advantages
│   ├── Maximum stress shadow benefit
│   ├── Fastest completion time
│   └── Lowest cost per stage
└── Challenges
    ├── Double equipment requirement
    ├── Complex real-time monitoring
    └── Well interaction concerns

HYBRID APPROACHES
├── Zipper + Simul-frac
├── Start zipper, switch to simul
└── Depends on formation response
```

## Surface Equipment Configuration

### Zipper Manifold System

```
ZIPPER MANIFOLD LAYOUT

                    ┌──────────────┐
   From Pumps ─────→│   MISSILE    │
                    │  (Manifold)  │
                    └──────┬───────┘
                           │
              ┌────────────┼────────────┐
              ↓            ↓            ↓
        ┌─────────┐  ┌─────────┐  ┌─────────┐
        │ Valve A │  │ Valve B │  │ Valve C │
        └────┬────┘  └────┬────┘  └────┬────┘
             │            │            │
             ↓            ↓            ↓
          Well A       Well B       Well C

MANIFOLD SPECIFICATIONS
├── Pressure Rating: Match well requirement
├── Connections: Quick connect/disconnect
├── Isolation: Each well independently valved
├── Safety: Multiple barrier philosophy
└── Monitoring: Pressure gauges each leg
```

### Equipment Requirements

| Equipment | 2-Well Zipper | 3-Well Zipper | Simul-Frac |
|-----------|--------------|---------------|------------|
| Blender | 1 | 1 | 2 |
| Hydration | 1 | 1 | 2 |
| Pump spread | 1 | 1 | 2 |
| Wireline units | 2 | 3 | 2 |
| Data vans | 2 | 3 | 2-3 |
| Manifold | 1 (zipper) | 1 (zipper) | 2 |

### Wireline Considerations

```
WIRELINE OPERATIONS IN ZIPPER
├── Multiple Units Required
│   ├── One per active well
│   ├── Prep while pumping adjacent
│   └── Coordinate timing
├── Staging
│   ├── Pre-load plugs and guns
│   ├── Minimize changeover time
│   └── Just-in-time delivery
├── Communication
│   ├── Radio channels assigned
│   ├── Clear protocols
│   └── Coordination with frac crew
└── Safety
    ├── Simultaneous operations awareness
    ├── Well-specific barriers
    └── SIMOPS procedures
```

## Operational Procedures

### Pre-Job Planning

```
ZIPPER PLANNING CHECKLIST
├── Well Spacing Verification
│   ├── Distance between wellheads
│   ├── Downhole lateral spacing
│   └── Stage alignment (offset or aligned)
├── Stage Design
│   ├── Number of stages per well
│   ├── Stage lengths
│   └── Proppant/fluid per stage
├── Schedule Development
│   ├── Cycle time calculations
│   ├── Resource allocation
│   └── Contingency planning
├── Equipment Layout
│   ├── Manifold placement
│   ├── Treating line routing
│   └── Wireline positioning
└── Communication Plan
    ├── Radio channels
    ├── Decision authority
    └── Emergency protocols
```

### Timing and Coordination

```
CYCLE TIME MANAGEMENT

CRITICAL TIMING ELEMENTS
├── Pump Time: 1.5-2.5 hours/stage
├── Wireline Time: 1.5-2.0 hours/stage
├── Valve Switching: 10-15 minutes
├── Pressure Test: 5-10 minutes
└── Buffer Time: 15-30 minutes

IDEAL SCENARIO
├── Wireline prep completes as pumping ends
├── Immediate switch to next well
├── No equipment standby
└── Continuous operations

COORDINATION TRIGGERS
├── "15 minutes to flush" call
├── "5 minutes to done" call
├── "Ready for you" confirmation
└── "Pressure up" verification
```

### Stage-to-Stage Transitions

| Step | Action | Responsible | Duration |
|------|--------|-------------|----------|
| 1 | Call "flushing" | Frac coordinator | N/A |
| 2 | Verify wireline ready | Wireline supervisor | N/A |
| 3 | Close completing well | Operator | 2 min |
| 4 | Open new well valve | Operator | 2 min |
| 5 | Pressure test lines | Frac crew | 5 min |
| 6 | Begin pumping | Frac coordinator | N/A |

## Monitoring and Control

### Real-Time Data Management

```
DATA DISPLAY REQUIREMENTS
├── Each Well Stream
│   ├── Treating pressure
│   ├── Rate
│   ├── Proppant concentration
│   ├── Volume pumped
│   └── ISIP tracking
├── Comparative Views
│   ├── Well-to-well comparison
│   ├── Stage-to-stage trending
│   └── Anomaly detection
└── System Status
    ├── Valve positions
    ├── Equipment status
    └── Personnel locations

ALARM SETTINGS
├── Pressure high: Individual well limits
├── Rate variance: >10% from design
├── Communication: Between wells
└── Equipment: Pump/blender failures
```

### Inter-Well Communication Detection

```
COMMUNICATION INDICATORS
├── Pressure Response on Adjacent Well
│   ├── Immediate: Direct communication
│   ├── Delayed: Indirect connection
│   └── None: No communication
├── Fluid/Proppant Detection
│   ├── Returns at offset well
│   ├── Flow at closed well
│   └── Fluid chemistry changes
└── Microseismic Evidence
    ├── Event location
    ├── Fracture propagation direction
    └── Stage-to-stage interaction

RESPONSE TO COMMUNICATION
├── Mild: Monitor and continue
├── Moderate: Adjust stage design
├── Severe: Consider skipping stages
└── Critical: Stop operations, evaluate
```

## Troubleshooting

### Common Zipper Issues

| Issue | Indication | Response |
|-------|------------|----------|
| Timing mismatch | Waiting between stages | Optimize prep sequence |
| Valve failure | Can't switch wells | Repair/replace, continue other well |
| Wireline delay | Pump waiting on perf | Expedite or batch operations |
| Inter-well communication | Pressure response offset | Adjust spacing, evaluate |
| Manifold leak | Pressure loss, flow | Isolate, repair, test |
| Screenout | Pressure out on stage | Evaluate, adjust design |

### Contingency Planning

```
CONTINGENCY SCENARIOS
├── Equipment Failure
│   ├── Pump: Use redundancy
│   ├── Blender: Pause operations
│   ├── Wireline: Delay stages
│   └── Manifold: Repair or bypass
├── Well Issues
│   ├── Screenout: Move to other well
│   ├── Ball stuck: Retrieve, continue
│   ├── Casing issue: Evaluate, decide
│   └── High pressure: Adjust design
├── Environmental
│   ├── Weather: Secure operations
│   ├── Spill: Stop, contain, clean
│   └── Noise complaint: Address
└── Personnel
    ├── Injury: Response plan, continue
    ├── Crew fatigue: Rotate crews
    └── Communication failure: Backup systems
```

## Safety Considerations

### SIMOPS Hazards

```
SIMULTANEOUS OPERATIONS RISKS
├── Multiple Active Wellheads
│   ├── High pressure at multiple locations
│   ├── Clear zoning required
│   └── Access control
├── Surface Equipment
│   ├── High pressure treating lines
│   ├── Moving equipment
│   └── Chemical handling
├── Personnel Coordination
│   ├── Multiple crews working
│   ├── Radio traffic management
│   └── Clear assignments
└── Emergency Response
    ├── Which well is active?
    ├── Isolation procedures
    └── Evacuation routes

SAFETY BARRIERS
├── Physical: Valve isolations, barriers
├── Procedural: Clear protocols, permits
├── Technical: Alarms, interlocks
└── Administrative: Training, supervision
```

### Safety Protocols

| Activity | Requirement |
|----------|-------------|
| Well switching | Verbal confirmation both ends |
| Pressure testing | All personnel clear |
| Wireline operations | Lubricator safety zone |
| Equipment movement | Spotter required |
| Night operations | Enhanced lighting |
| Shift change | Formal handover |

## Performance Metrics

### Efficiency Tracking

```
ZIPPER EFFICIENCY METRICS
├── Stage Per Day
│   ├── Target: 6-10 stages/day (2 well)
│   ├── Good: >8 stages/day
│   └── Excellent: >10 stages/day
├── NPT (Non-Productive Time)
│   ├── Target: <10%
│   ├── Track by cause
│   └── Continuous improvement
├── Equipment Utilization
│   ├── Pump hours vs available
│   ├── Wireline efficiency
│   └── Blender utilization
└── Cost Per Stage
    ├── Track all costs
    ├── Compare to budget
    └── Benchmark vs industry
```

### Cost Analysis

| Cost Element | Sequential | Zipper | Savings |
|--------------|-----------|--------|---------|
| Pump spread | Base | -25% | Equipment sharing |
| Fluid | Same | Same | None |
| Proppant | Same | Same | None |
| Wireline | Base | +10% | Multiple units |
| Labor | Base | -20% | Fewer days |
| **Total** | Base | **-15-25%** | Overall |

---

*Zipper frac operations require excellent coordination and planning. Success depends on timing precision, communication, and contingency preparation.*
