# Rig Components Specifications

## Drawworks

### Classification and Ratings

| Component | Light Duty | Medium | Heavy Duty | Ultra HD |
|-----------|-----------|--------|------------|----------|
| Input HP | 750-1000 | 1500-2000 | 2500-3000 | 3000-4000 |
| Max Line Pull (lb) | 50,000 | 75,000 | 100,000 | 125,000+ |
| Line Speed (ft/min) | 0-1500 | 0-1800 | 0-2000 | 0-2200 |
| Drum Capacity (ft) | 3000-4000 | 4000-5000 | 5000-6000 | 6000+ |
| Brake Rating (HP) | 1000 | 2000 | 3000 | 4000 |

### Drawworks Components

```
POWER SYSTEM
├── Prime Mover Connection
│   ├── Mechanical (compound)
│   ├── Electric (DC/AC)
│   └── Hydraulic (rare)
├── Transmission
│   ├── Chain drive
│   ├── Direct drive
│   └── Gear reduction
└── Clutch System
    ├── Air actuated
    └── Hydraulic

DRUM ASSEMBLY
├── Main Drum
│   ├── Grooved for wire rope
│   ├── Flanges for line containment
│   └── Spooling device
├── Cathead Shafts
│   ├── Friction cathead (makeup)
│   └── Mechanical cathead (breakout)
└── Sandline Drum (optional)

BRAKING SYSTEM
├── Primary Brake
│   ├── Band brake (most common)
│   ├── Disc brake
│   └── Eddy current (auxiliary)
├── Auxiliary Brake
│   ├── Hydromatic
│   ├── Elmagco
│   └── Baylor
└── Emergency Systems
    ├── Automatic setback
    └── Crown-o-matic
```

### Drawworks Inspection Points

| Inspection | Frequency | Accept/Reject Criteria |
|------------|-----------|----------------------|
| Brake band lining | Daily | >¼" remaining |
| Brake drum surface | Weekly | No scoring >1/16" |
| Clutch facing | Weekly | >¼" remaining |
| Chain tension | Weekly | ½"-1" deflection |
| Oil level | Daily | In sight glass |
| Drum flanges | Weekly | No cracks, chips |
| Wire rope condition | Each trip | Per API RP 9B |

---

## Top Drive

### Top Drive Classifications

| Type | Torque (ft-lb) | Speed (RPM) | Weight (lb) |
|------|---------------|-------------|-------------|
| Light | 15,000-25,000 | 0-250 | 20,000-25,000 |
| Medium | 25,000-40,000 | 0-220 | 30,000-40,000 |
| Heavy | 40,000-60,000 | 0-200 | 45,000-55,000 |
| Ultra Heavy | 60,000-85,000 | 0-180 | 55,000-70,000 |

### Top Drive Components

```
DRIVE SYSTEM
├── Electric Motor(s)
│   ├── AC (most common modern)
│   ├── DC (legacy)
│   └── Dual motor configuration
├── Gearbox
│   ├── Planetary reduction
│   ├── Helical gears
│   └── Lubrication system
└── Rotating Head
    ├── Main shaft
    ├── Bearings (thrust & radial)
    └── Seals

PIPE HANDLING
├── IBOP (Upper)
│   ├── Full-open valve
│   └── Remote operated
├── Saver Sub
│   ├── Protects main shaft
│   └── Replaceable connection
├── Elevator Links
│   ├── Fixed or retractable
│   └── Multiple lengths available
└── Torque Wrench
    ├── Makeup & breakout
    ├── Spinner
    └── Clamp system

GUIDE SYSTEM
├── Dolly Assembly
│   ├── Guide rails
│   └── Rollers
├── Counterbalance
│   ├── Cylinder or spring
│   └── Adjustable
└── Swivel/Wash Pipe
    ├── Mud path
    └── Rotating seal
```

### Top Drive Maintenance

| Component | Interval | Action |
|-----------|----------|--------|
| Gearbox oil | 500 hrs / Monthly | Check level, sample |
| Motor brushes | 1000 hrs | Inspect, measure |
| IBOP | Each well | Function test |
| Torque wrench | Weekly | Calibration check |
| Guide rollers | Weekly | Inspect, lubricate |
| Swivel packing | As needed | Replace when leaking |
| Main bearings | Annual | Inspect, measure play |

---

## Mast/Derrick

### Mast Types and Ratings

| Type | Height (ft) | Hook Load (lb) | Wind Rating |
|------|-------------|----------------|-------------|
| Portable Mast | 84-96 | 200,000-350,000 | 70 mph |
| Telescoping | 120-140 | 350,000-500,000 | 80 mph |
| Standard Derrick | 140-147 | 500,000-750,000 | 100 mph |
| Enhanced Derrick | 160-180 | 750,000-1,500,000 | 115 mph |

### Structural Components

```
MAST STRUCTURE
├── Legs (4)
│   ├── Main chords
│   ├── Lacing/bracing
│   └── Leg connections
├── Girts (horizontal)
│   ├── V-door girt
│   ├── Intermediate girts
│   └── Crown section
├── Bracing
│   ├── Diagonal bracing
│   ├── X-bracing
│   └── Portal bracing
└── Crown Assembly
    ├── Crown block
    ├── Fast line sheave
    ├── Deadline anchor
    └── Crown platform

SUBSTRUCTURE
├── Rotary Beams
│   ├── Support rotary table
│   └── Setback area
├── Setback Structure
│   ├── Pipe setback area
│   ├── Fingerboard
│   └── Racking capacity
└── Cellar
    ├── BOP access
    └── Flow line connection

AUXILIARY STRUCTURES
├── Monkey Board
│   ├── Derrickman platform
│   └── Safety harness anchor
├── Stabbing Board
│   ├── Casing running
│   └── Adjustable height
└── Escape Systems
    ├── Geronimo line
    └── Emergency ladder
```

### Mast Inspection Requirements

| Inspection Type | Frequency | Key Points |
|----------------|-----------|------------|
| Visual | Daily | Obvious damage, alignment |
| Guy wire tension | Weekly | Proper tension per specs |
| Pin connections | Monthly | Wear, cracks, corrosion |
| Structural NDT | Annual | Welds, stress points |
| Load test | 5 years | Proof load per API |

### Wind Loading Criteria

| Condition | Wind Speed | Action Required |
|-----------|-----------|-----------------|
| Normal Operations | <35 mph | No restrictions |
| Caution | 35-50 mph | Monitor, secure loose items |
| Restricted | 50-70 mph | Stop crane, secure equipment |
| Suspend | >70 mph | Suspend all operations |
| Lay Down | >100 mph | Lay down mast if time permits |

---

## Rotary Table

### Rotary Table Specifications

| Size (in) | Opening (in) | Static Load (lb) | RPM Range | Torque (ft-lb) |
|-----------|-------------|-----------------|-----------|----------------|
| 17½ | 17½ | 500,000 | 0-200 | 10,000 |
| 20½ | 20½ | 750,000 | 0-200 | 15,000 |
| 27½ | 27½ | 1,000,000 | 0-150 | 25,000 |
| 37½ | 37½ | 1,500,000 | 0-120 | 40,000 |
| 49½ | 49½ | 2,000,000 | 0-100 | 60,000 |

### Rotary Components

```
MAIN ASSEMBLY
├── Turntable
│   ├── Master bushing receiver
│   ├── Slips pocket
│   └── Lock mechanism
├── Sprocket Drive
│   ├── Drive sprocket
│   ├── Chain drive
│   └── Clutch engagement
├── Main Bearing
│   ├── Thrust bearing
│   ├── Radial bearing
│   └── Seal system
└── Housing
    ├── Support structure
    └── Oil reservoir

AUXILIARY EQUIPMENT
├── Kelly Bushing
│   ├── Square drive (4/6 pin)
│   ├── Roller type
│   └── Split for removal
├── Master Bushing
│   ├── Bowl receiver
│   ├── Locking dogs
│   └── Various sizes
└── Slips
    ├── Rotary slips
    ├── Drill collar slips
    └── Casing slips
```

### Rotary Table Maintenance

| Item | Frequency | Specification |
|------|-----------|---------------|
| Oil level | Daily | Maintain at mark |
| Oil change | 500 hrs | Per OEM spec |
| Bearing play | Monthly | Max per OEM |
| Sprocket wear | Monthly | Replace at 25% wear |
| Lock mechanism | Weekly | Function test |
| Turntable surface | Weekly | Check for wear/damage |

---

## Crown Block

### Crown Block Specifications

| Rating (tons) | Sheave Qty | Sheave Dia (in) | Line Size (in) |
|--------------|------------|-----------------|----------------|
| 150 | 4-5 | 36-42 | 1-1⅛ |
| 250 | 5-6 | 42-48 | 1⅛-1¼ |
| 350 | 6-7 | 48-54 | 1¼-1⅜ |
| 500 | 7-8 | 54-60 | 1⅜-1½ |
| 750 | 8-10 | 60-72 | 1½-1⅝ |

### Crown Block Components

```
SHEAVE ASSEMBLY
├── Sheaves
│   ├── Groove profile (per rope size)
│   ├── Hardened surface
│   └── Balanced for high speed
├── Bearings
│   ├── Roller or sleeve
│   ├── Sealed or open
│   └── Grease or oil lubricated
├── Shaft
│   ├── Stationary or rotating
│   └── Keyed to frame
└── Guards
    ├── Sheave guards
    └── Rope guides

FRAME
├── Side Plates
│   ├── Structural members
│   └── Shaft supports
├── Bumper
│   ├── Crown saver (limit)
│   └── Emergency stop
└── Dead Line Anchor
    ├── Sheave
    └── Anchor point
```

---

## Traveling Block

### Traveling Block Specifications

| Rating (tons) | Sheave Qty | Weight (lb) | Line Size (in) |
|--------------|------------|-------------|----------------|
| 150 | 4 | 6,000-8,000 | 1-1⅛ |
| 250 | 5 | 10,000-14,000 | 1⅛-1¼ |
| 350 | 6 | 16,000-22,000 | 1¼-1⅜ |
| 500 | 7 | 25,000-35,000 | 1⅜-1½ |
| 750 | 8 | 40,000-50,000 | 1½-1⅝ |

### Traveling Block Inspection

| Component | Inspection Point | Reject Criteria |
|-----------|-----------------|-----------------|
| Sheaves | Groove wear | >1/32" wear |
| Sheaves | Cracks | Any visible crack |
| Bearings | Play | Excessive play |
| Side plates | Cracks | Any visible crack |
| Becket | Wear, cracks | Visual defects |
| Safety latch | Function | Does not engage |

---

## Quick Reference - Rig Equipment Ratings

### Rig Component Compatibility

| Rig Class | Drawworks | Top Drive | Mast | Rotary |
|-----------|-----------|-----------|------|--------|
| 250 | 1000 HP | 25,000 ft-lb | 350k | 17½" |
| 350 | 1500 HP | 37,500 ft-lb | 500k | 20½" |
| 500 | 2000 HP | 50,000 ft-lb | 750k | 27½" |
| 750 | 3000 HP | 65,000 ft-lb | 1000k | 37½" |
| 1000 | 4000 HP | 80,000 ft-lb | 1500k | 49½" |

---

*Always verify equipment ratings with manufacturer data plates and current certifications.*
