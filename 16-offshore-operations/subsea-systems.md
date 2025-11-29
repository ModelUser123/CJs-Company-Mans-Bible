# Subsea Systems

## Subsea Wellhead Systems

### Wellhead Components

```
HIGH-PRESSURE HOUSING
├── Size: 18¾" or 13⅝"
├── Pressure: 10,000-20,000 psi
├── Functions
│   ├── BOP connection
│   ├── Casing hanger support
│   └── Pressure barrier
└── Lockdown
    ├── Mechanical or hydraulic
    └── Tested after installation

LOW-PRESSURE HOUSING
├── Size: 30" or 36"
├── Functions
│   ├── Conductor hanger
│   ├── Structural support
│   └── Foundation
└── Installation
    ├── Jetted or drilled
    └── Cemented in place

CASING HANGERS
├── Types
│   ├── Mandrel (slip-lock)
│   ├── Tubing spool
│   └── Compact (integral)
├── Seals
│   ├── Metal-to-metal
│   └── Elastomer backup
└── Test
    ├── Inflow test
    └── Pressure test
```

### Subsea Wellhead Sequence

| Step | Component | Depth | Function |
|------|-----------|-------|----------|
| 1 | 30"/36" Housing | 200-500 ft | Foundation |
| 2 | Conductor | 500-1500 ft | Structural |
| 3 | 18¾" Housing | Surface | BOP landing |
| 4 | Surface casing | 2000-5000 ft | Pressure isolation |
| 5 | Intermediate | As needed | Transition |
| 6 | Production | TD | Production |
| 7 | Tree | Final | Production control |

---

## Subsea BOP Stack

### Stack Configuration

```
LOWER MARINE RISER PACKAGE (LMRP)
├── Components
│   ├── Annular preventer (2)
│   ├── LMRP connector
│   ├── Flex joint
│   └── Control pods
├── Function
│   ├── Emergency disconnect
│   ├── Quick reconnect
│   └── Upper stack containment
└── Weight: 100,000-200,000 lb

BOP STACK
├── Ram Preventers
│   ├── Blind shear rams
│   ├── Casing shear rams
│   ├── Pipe rams (2-3)
│   ├── Variable bore rams
│   └── Test rams
├── Wellhead Connector
│   ├── 18¾" typical
│   ├── Hydraulic lock
│   └── ROV overrideable
├── Choke & Kill
│   ├── Internal lines
│   ├── External pods
│   └── Fail-safe valves
└── Weight: 300,000-500,000 lb

CONTROL SYSTEM
├── Multiplex (MUX)
│   ├── Electrical signals
│   ├── Fiber optic
│   └── Pilot hydraulic
├── Backup Systems
│   ├── Acoustic (2 systems)
│   ├── ROV intervention
│   ├── Autoshear
│   └── Deadman
└── Pods
    ├── Dual redundant
    ├── Retrievable
    └── Hot-swappable
```

### Subsea BOP Testing

| Test | Frequency | Pressure | Duration |
|------|-----------|----------|----------|
| Initial | Before use | Full WP | 30 min |
| Periodic | 14 days | 70% WP | 5 min |
| After repair | Each time | 70% WP | 5 min |
| Function | 7 days | Operating | Full cycle |
| Accumulator | 7 days | Close all + reserve | N/A |

### Emergency Systems

```
EMERGENCY DISCONNECT SEQUENCE (EDS)
├── Activation
│   ├── Surface command
│   ├── Acoustic command
│   └── Automatic (deadman)
├── Sequence
│   1. Close BSR
│   2. Seal wellbore
│   3. Unlock LMRP connector
│   4. Unlatch connector
│   5. Lift LMRP clear
└── Time: <60 seconds

AUTOSHEAR
├── Trigger: Unexpected disconnect
├── Function: Shear and seal
└── Independent of control

DEADMAN
├── Trigger: Loss of communication
├── Timer: 24-72 hours typically
├── Function: Automatic EDS
└── Fail-safe design
```

---

## Marine Riser System

### Riser Components

```
RISER JOINTS
├── Standard
│   ├── 75-90 ft lengths
│   ├── 21" bore typical
│   └── Buoyancy equipped
├── Pup Joints
│   ├── Various lengths
│   ├── Space-out adjustment
│   └── Same specifications
└── Connections
    ├── Flanged
    ├── Quick-connect
    └── Stress joint rated

AUXILIARY LINES
├── Choke Line
│   ├── 4-6" bore
│   ├── 15,000 psi
│   └── Internal or external
├── Kill Line
│   ├── 4-6" bore
│   ├── 15,000 psi
│   └── Internal or external
├── Booster Line
│   ├── 6-8" bore
│   ├── Mud boost circulation
│   └── ECD management
└── Hydraulic Lines
    ├── BOP control
    └── Multiple bundles

BUOYANCY MODULES
├── Syntactic foam
├── Depth rated
├── Reduce riser weight
└── 60-80% weight reduction

TENSIONER SYSTEM
├── Hydro-pneumatic
├── Capacity: 1-3 million lb
├── Stroke: 50-80 ft
└── Maintains constant tension
```

### Riser Management

| Parameter | Normal | Warning | Critical |
|-----------|--------|---------|----------|
| Tension | 100% design | <85% | <70% |
| Angle | <2° | 2-4° | >4° |
| VIV | Minimal | Moderate | Severe |
| Flex joint | <4° | 4-6° | >6° |

### Riser Operating Limits

```
CONNECTED LIMITS
├── Vessel Offset: <5-8% of water depth
├── Current: <2-3 knots typically
├── Heave: <15 ft (varies by system)
└── Riser Angle: <4° typically

DISCONNECT CRITERIA
├── Vessel offset approaching limit
├── Tensioner stroke limit
├── Emergency on vessel
├── Loss of position
└── Weather exceeding limits

RECONNECTION REQUIREMENTS
├── Weather within limits
├── Well secured
├── BOP tested
└── Riser inspected
```

---

## Dynamic Positioning (DP)

### DP Classification

| Class | Requirement | Application |
|-------|-------------|-------------|
| DP-1 | Single system | Light duty |
| DP-2 | Redundant systems | Standard drilling |
| DP-3 | Triple redundant | Critical ops, HPHT |

### DP System Components

```
POSITION REFERENCE SYSTEMS
├── DGPS (differential GPS)
├── Acoustics (HPR, LBL, USBL)
├── Taut Wire
├── Laser/radar
└── Gyrocompass

THRUSTERS
├── Main propulsion
├── Tunnel thrusters
├── Azimuth thrusters
├── Retractable thrusters
└── Power: 2,000-10,000 HP each

POWER SYSTEM
├── Main generators (4-6)
├── Redundant buses
├── Automatic load sharing
└── Blackout recovery

CONTROL SYSTEM
├── Triple-redundant computers
├── Joystick/auto control
├── Consequence analysis
├── Alert management
└── DP operator interface
```

### DP Operations

```
WATCH CIRCLES
├── Green Zone
│   ├── Normal operations
│   └── Offset <3% WD
├── Yellow Zone (Advisory)
│   ├── Enhanced monitoring
│   ├── Prepare for disconnect
│   └── Offset 3-5% WD
├── Red Zone (Emergency)
│   ├── Initiate EDS
│   └── Offset >5% WD
└── Factors
    ├── Water depth
    ├── Current/wind
    ├── Riser limits
    └── Vessel capability

DP WATCHES
├── DP Operator: 4-hour max
├── Relief: Overlap handover
├── Documentation: Every event
└── DPO Certification: Required
```

### Failure Mode Analysis

| Failure | Effect | Response |
|---------|--------|----------|
| Single thruster | Reduced capability | Monitor closely |
| Single generator | Load redistribution | Continue ops |
| Single ref system | Backup active | Verify backup |
| Single computer | Redundant takes over | Investigate |
| Drive-off | Vessel moves off position | EDS if needed |
| Drift-off | Vessel drifts off position | EDS if needed |

---

## ROV Operations

### ROV Capabilities

```
OBSERVATION CLASS
├── Depth: 3,000-10,000 ft
├── Functions
│   ├── Visual inspection
│   ├── Light manipulation
│   └── Basic tooling
└── Size: Small, portable

WORK CLASS
├── Depth: 10,000-15,000 ft
├── Functions
│   ├── Heavy manipulation
│   ├── Intervention
│   ├── Construction support
│   └── BOP operations
├── Tooling
│   ├── Torque tools
│   ├── Hot stabs
│   ├── Cutting/grinding
│   └── Cleaning
└── Power: Electric/hydraulic
```

### ROV BOP Interface

| Function | Method | Capability |
|----------|--------|------------|
| Ram override | Hot stab | Open/close |
| LMRP unlatch | Override | Disconnect |
| Wellhead unlock | Torque tool | Release hanger |
| Connector unlock | Override | Release BOP |
| Valve operation | Panel interface | Choke/kill valves |
| Visual inspection | Camera | All components |

---

*Subsea systems require specialized training and certification. Operations should be conducted by qualified personnel only.*
