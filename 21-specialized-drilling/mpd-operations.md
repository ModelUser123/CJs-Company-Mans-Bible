# Managed Pressure Drilling (MPD)

## MPD Fundamentals

### What is MPD?

```
MPD DEFINITION
├── Precise Control of BHP
│   ├── Mud weight + surface backpressure
│   ├── Maintains BHP within window
│   ├── Constant or variable BHP
│   └── Closed loop system
├── Key Principle
│   ├── MW set below pore pressure
│   ├── Surface pressure applied
│   ├── BHP = Hydrostatic + Surface Pressure
│   └── Adjustable in real-time
├── Benefits
│   ├── Drill narrow windows
│   ├── Reduce losses
│   ├── Faster kick detection
│   ├── Minimize NPT
│   └── Protect formations
└── When to Use
    ├── Narrow PP/FG window
    ├── Depleted zones
    ├── Fractured reservoirs
    ├── Uncertain pressures
    └── Historical lost circulation
```

### MPD Methods

| Method | Description | Application |
|--------|-------------|-------------|
| Constant BHP | Surface pressure varies | Connections, trips |
| Pressurized Mud Cap | Heavy mud cap, drill underbalanced | Severe losses |
| Dual Gradient | Variable density annulus | Deepwater |
| Returns Flow Control | Choke maintains BHP | All MPD |

## Equipment Requirements

### Surface Equipment

```
MPD SURFACE EQUIPMENT
├── Rotating Control Device (RCD)
│   ├── Seals around drill pipe
│   ├── Diverts returns through choke
│   ├── Allows rotation and pressure
│   ├── 2500-5000 psi typical
│   └── Critical barrier element
├── MPD Choke Manifold
│   ├── Automated choke
│   ├── Precise pressure control
│   ├── Fast response time
│   ├── Redundancy (multiple chokes)
│   └── Manual backup
├── Flow Measurement
│   ├── Coriolis meter (accurate)
│   ├── Flow in measurement
│   ├── Flow out measurement
│   ├── Delta flow calculation
│   └── Real-time display
├── Pressure Management System
│   ├── Control computer
│   ├── Automatic adjustments
│   ├── Alarms and limits
│   ├── Data recording
│   └── Interface with rig
└── Separation System
    ├── Handle returns at pressure
    ├── Gas handling
    ├── Solids control
    └── Fluid measurement
```

### Downhole Equipment

```
DOWNHOLE MPD COMPONENTS
├── Non-Return Valve (NRV)
│   ├── Prevents backflow up string
│   ├── Float type or flapper
│   ├── Critical for connections
│   └── Positioned above bit
├── PWD (Pressure While Drilling)
│   ├── Real-time BHP measurement
│   ├── Critical for MPD
│   ├── ECD monitoring
│   └── Kick/loss detection
├── Downhole Deployment Valve (DDV)
│   ├── Optional for some methods
│   ├── Isolates string on connections
│   └── Advanced MPD operations
└── ECD Reduction Tools
    ├── If ECD is primary issue
    ├── Reduce annular friction
    └── Various technologies
```

## MPD Procedures

### Startup Procedure

```
MPD STARTUP SEQUENCE
├── Pre-MPD Checks
│   ├── RCD installed and tested
│   ├── Choke system tested
│   ├── Flow meters calibrated
│   ├── BOP tested
│   ├── Control system functional
│   └── All personnel trained
├── Transition to MPD
│   ├── May start conventionally
│   ├── Confirm stable conditions
│   ├── Close flow diversion
│   ├── Establish choke control
│   ├── Verify BHP
│   └── Begin MPD operations
├── Operating Mode
│   ├── Set target BHP
│   ├── Monitor continuously
│   ├── Choke adjusts automatically
│   ├── Respond to changes
│   └── Document everything
└── Normal Operations
    ├── Drilling: Choke maintains BHP
    ├── Connections: Add pressure for ECD
    ├── Trips: Special procedures
    └── Logging: May need adjustments
```

### Connection Procedure

```
MPD CONNECTION PROCEDURE
├── Conventional Issue
│   ├── Pump off → ECD drops
│   ├── BHP decreases
│   ├── May induce kick
│   └── MPD compensates
├── MPD Compensation
│   ├── Stop pumps
│   ├── Increase surface pressure
│   ├── Amount = ECD equivalent
│   ├── Maintain constant BHP
│   └── Make connection
├── Typical Sequence
│   ├── Slow pumps to minimum
│   ├── Close NRV (trap pressure)
│   ├── Stop pumps
│   ├── Apply surface pressure
│   ├── Break connection
│   ├── Make up new joint
│   ├── Restart pumps
│   ├── Bleed surface pressure
│   └── Resume drilling
└── Key Points
    ├── Timing critical
    ├── Automated helps
    ├── Monitor BHP throughout
    └── Practice procedures
```

### Trip Procedures

```
MPD TRIPPING
├── Challenge
│   ├── Cannot maintain pressure
│   ├── Swab/surge concerns
│   ├── RCD not rated for tripping
│   └── Need alternative method
├── Options
│   ├── Trip with mud cap
│   │   ├── Set weighted mud
│   │   ├── Provides overbalance
│   │   └── Monitor carefully
│   ├── Continuous circulation
│   │   ├── Special sub
│   │   ├── Maintains BHP
│   │   └── Complex equipment
│   ├── Trip margin
│   │   ├── Weight up mud
│   │   ├── Provide margin
│   │   └── Trip conventionally
│   └── Snubbing
│       ├── Under pressure
│       ├── Specialized equipment
│       └── Slow process
└── Procedure Selection
    ├── Based on conditions
    ├── Risk assessment
    ├── Equipment available
    └── Operator preference
```

## Kick/Loss Detection

### Enhanced Detection

```
MPD KICK DETECTION
├── Faster Detection
│   ├── Closed system visibility
│   ├── Coriolis flow measurement
│   ├── Small changes detectable
│   └── Typical: 1-3 bbl accuracy
├── Delta Flow
│   ├── Flow In - Flow Out
│   ├── Continuous calculation
│   ├── Alarm on deviation
│   └── Real-time display
├── Pressure Response
│   ├── PWD shows BHP change
│   ├── Surface pressure change
│   ├── Combined with flow data
│   └── Confirms influx/loss
└── Response
    ├── Influx: Increase choke pressure
    ├── Loss: Decrease choke pressure
    ├── Record data
    └── Evaluate response

DETECTION SENSITIVITY
├── Conventional: 10-20 bbl typical
├── MPD: 1-5 bbl possible
├── Enables earlier response
└── Smaller kicks to handle
```

### Well Control Transition

```
MPD TO WELL CONTROL
├── When Kick Detected
│   ├── Increase surface pressure
│   ├── Attempt to balance
│   ├── If successful, continue
│   └── If not, transition
├── Transition to BOP
│   ├── Close BOP (rams)
│   ├── RCD remains closed
│   ├── Route through choke
│   ├── Standard kill procedures
│   └── MPD choke can assist
├── Kill Operation
│   ├── Standard driller's/W&W
│   ├── Use MPD equipment
│   ├── Or conventional choke
│   ├── Enhanced monitoring
│   └── Resume MPD after kill
└── Documentation
    ├── Record entire event
    ├── Analyze response
    └── Adjust procedures
```

## Operational Considerations

### ECD Management

```
ECD WITH MPD
├── ECD Components
│   ├── Hydrostatic
│   ├── Annular friction
│   ├── Cuttings load
│   └── Surface backpressure
├── ECD Control Methods
│   ├── Reduce MW (add SP)
│   ├── Optimize rheology
│   ├── Control ROP (cuttings)
│   ├── Flow rate management
│   └── Continuous circulation
└── Benefits
    ├── Drill otherwise impossible wells
    ├── Reduce losses
    ├── Protect formations
    └── Maintain hole stability
```

### Troubleshooting

| Problem | Cause | Solution |
|---------|-------|----------|
| RCD leak | Wear, damage | Replace element |
| Erratic pressure | Choke issue | Check/repair choke |
| Inaccurate flow | Meter issue | Calibrate |
| Excessive SP | Too low MW | Adjust MW |
| BHP fluctuation | Control issue | Tune system |

---

*MPD is a powerful technique that requires specialized equipment, training, and procedures. Proper implementation significantly expands drilling capability.*
