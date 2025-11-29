# CT Fundamentals

## Coiled Tubing Equipment Details

### Reel and Tubing

```
CT REEL SPECIFICATIONS
├── Reel Capacity
│   ├── Based on CT size
│   ├── Core diameter critical
│   ├── Flange diameter limits
│   └── Weight capacity
├── Typical Capacities
│   ├── 1.5" CT: 25,000-35,000 ft
│   ├── 2.0" CT: 18,000-25,000 ft
│   ├── 2.375" CT: 12,000-18,000 ft
│   └── 2.875" CT: 8,000-12,000 ft
├── Drive System
│   ├── Hydraulic motor
│   ├── Torque control
│   ├── Variable speed
│   └── Braking system
└── Level Wind
    ├── Ensures even wrap
    ├── Prevents damage
    └── Automatic tracking

CT PROPERTIES BY SIZE
┌──────────┬─────────┬────────┬─────────┬──────────┐
│ OD (in)  │ Wall    │ ID     │ Wt/ft   │ Capacity │
│          │ (in)    │ (in)   │ (lb)    │ (bbl/ft) │
├──────────┼─────────┼────────┼─────────┼──────────┤
│ 1.25     │ 0.125   │ 1.000  │ 1.30    │ 0.00097  │
│ 1.50     │ 0.156   │ 1.188  │ 1.94    │ 0.00137  │
│ 1.75     │ 0.175   │ 1.400  │ 2.55    │ 0.00190  │
│ 2.00     │ 0.175   │ 1.650  │ 2.95    │ 0.00264  │
│ 2.375    │ 0.190   │ 1.995  │ 3.83    │ 0.00387  │
│ 2.875    │ 0.203   │ 2.469  │ 5.02    │ 0.00592  │
└──────────┴─────────┴────────┴─────────┴──────────┘
```

### Injector Head

```
INJECTOR HEAD COMPONENTS
├── Drive System
│   ├── Chain Type
│   │   ├── Most common
│   │   ├── High grip force
│   │   └── Long service life
│   ├── Tire Type
│   │   ├── Gentler on tubing
│   │   ├── Lower grip capacity
│   │   └── Faster wear
│   └── Hybrid designs available
├── Key Specifications
│   ├── Injection force: 20,000-60,000 lb
│   ├── Speed: 0-200+ ft/min
│   ├── CT size range
│   └── Weight indicator
├── Weight Measurement
│   ├── Load cells in system
│   ├── Tension monitoring
│   ├── Snub force display
│   └── Critical for operations
└── Safety Features
    ├── Hydraulic overpull protection
    ├── Emergency stops
    ├── Chain/tire monitors
    └── Slip detection
```

### BOP Stack Configuration

```
CT BOP STACK (Bottom to Top)
├── Wellhead Adapter
│   ├── Connects to existing wellhead
│   └── Appropriate flange size
├── Slip Rams
│   ├── Hold CT in place
│   ├── Emergency support
│   └── Sized for CT OD
├── Blind Rams
│   ├── Close on open hole
│   ├── Full seal capability
│   └── Secondary barrier
├── Shear Rams
│   ├── Cut CT in emergency
│   ├── Must seal after cut
│   ├── Rated for CT wall
│   └── Last resort
├── Stripper/Packer
│   ├── Primary seal around CT
│   ├── Dynamic seal while moving
│   ├── Rubber element
│   └── Pressure rated
└── Quick Connector
    ├── Allows BHA changes
    ├── Quick disconnect
    └── Pressure rated

PRESSURE RATINGS
├── Match to well conditions
├── Typical: 5,000-15,000 psi
├── Test before operations
└── Document all tests
```

## CT Operations Fundamentals

### Running In Hole

```
RIH PROCEDURE
├── Pre-Run Checks
│   ├── BOP tested
│   ├── CT inspected
│   ├── BHA function tested
│   ├── Fluids ready
│   └── Communications checked
├── Initial Entry
│   ├── Engage stripper
│   ├── Pressurize as needed
│   ├── Start slow
│   └── Monitor weight
├── Running Speed
│   ├── Typical: 50-100 ft/min
│   ├── Slow in curves/restrictions
│   ├── Watch for tags
│   └── Adjust for conditions
├── Monitoring
│   ├── Weight/drag
│   ├── Depth
│   ├── Pressure
│   └── Returns
└── At Target Depth
    ├── Confirm depth
    ├── Circulate if applicable
    ├── Begin job
    └── Monitor continuously
```

### Pulling Out of Hole

```
POOH PROCEDURE
├── Preparation
│   ├── Complete job operations
│   ├── Circulate clean if applicable
│   ├── Prepare for any pressure
│   └── Ready stripper
├── Pulling Speed
│   ├── Similar to RIH
│   ├── Watch for stuck
│   ├── Monitor stripping pressure
│   └── Control speed
├── At Surface
│   ├── Stop before BHA at stripper
│   ├── Bleed pressure if needed
│   ├── Extract BHA
│   └── Secure well
└── Post-Job
    ├── BOP test if required
    ├── Inspect CT
    ├── Document operations
    └── Rig down
```

### Circulating Operations

```
CT CIRCULATION
├── Pump Capabilities
│   ├── Rate: 0.5-5 bpm typical
│   ├── Pressure: Up to 10,000+ psi
│   ├── Continuous or batch
│   └── Multiple fluid capability
├── Annular Returns
│   ├── Up annulus between CT and tubing
│   ├── Or CT and casing
│   ├── Must have flow path
│   └── Monitor for issues
├── Circulation Calculations
│   ├── Annular velocity
│   ├── Pressure drops
│   ├── Volumes
│   └── Time to circulate
└── Common Issues
    ├── Bridging (debris)
    ├── Lost returns
    ├── Pressure limits
    └── Rate limitations
```

## CT Depth and Weight

### Depth Tracking

```
CT DEPTH MEASUREMENT
├── Methods
│   ├── Wheel/encoder on reel
│   ├── Encoder on injector
│   ├── Magnetic marks on CT
│   └── Combination systems
├── Accuracy Factors
│   ├── CT stretch under load
│   ├── Temperature effects
│   ├── Pressure effects
│   └── Measurement calibration
├── Stretch Correction
│   ├── Calculate based on load
│   ├── E = 30 × 10⁶ psi for steel
│   ├── Stretch = (Load × Length) / (E × Area)
│   └── Apply correction
└── Verification
    ├── Compare to known depths
    ├── Correlation with logs
    ├── Tag known points
    └── Calibrate regularly
```

### Weight Interpretation

```
CT WEIGHT INDICATORS
├── Running In (Slack Off)
│   ├── String weight decreases
│   ├── CT pushing into well
│   ├── May enter buckling
│   └── Watch for lockup
├── Picking Up (Overpull)
│   ├── String weight increases
│   ├── Indicates drag/stuck
│   ├── May indicate problem
│   └── Know limits
├── Normal Signatures
│   ├── Gradual increase RIH (friction)
│   ├── Gradual increase POOH (friction)
│   ├── Tags at restrictions
│   └── Response at depths
└── Abnormal Signatures
    ├── Sudden change (stuck, tag)
    ├── Excessive drag (problem)
    ├── No weight (parting)
    └── Investigate anomalies
```

## CT Material and Fatigue

### CT Material Properties

```
CT STEEL GRADES
├── Standard CT70
│   ├── Yield: 70,000 psi
│   ├── Most common
│   ├── Good fatigue life
│   └── Adequate for most jobs
├── High Strength CT80
│   ├── Yield: 80,000 psi
│   ├── Higher pressure rating
│   ├── Reduced fatigue life
│   └── Deep wells
├── CT90 and CT100
│   ├── Yield: 90,000-100,000 psi
│   ├── Extreme conditions
│   ├── Limited fatigue
│   └── Specialty applications
└── Corrosion Resistant
    ├── 13Cr or higher
    ├── H2S/CO2 service
    ├── Higher cost
    └── Extended life
```

### Fatigue Life Management

```
FATIGUE TRACKING SYSTEM
├── Cycle Counting
│   ├── One trip = one cycle minimum
│   ├── Bending over gooseneck
│   ├── Through injector
│   ├── Both in and out
│   └── Tracked by depth
├── Life Calculation
│   ├── Cycles consumed
│   ├── Remaining cycles
│   ├── Pressure effects
│   ├── Temperature effects
│   └── Software tracking
├── Inspection Requirements
│   ├── Visual each job
│   ├── Diameter measurement
│   ├── Wall thickness
│   ├── UT inspection (periodic)
│   └── Track all data
├── Retirement Criteria
│   ├── Calculated life exceeded
│   ├── Diameter growth >5%
│   ├── Wall thinning detected
│   ├── Visible damage
│   └── Operator discretion
└── Documentation
    ├── Complete records
    ├── Job history
    ├── Inspection results
    └── Audit trail
```

## CT Calculations

### Common CT Calculations

```
VOLUME CALCULATIONS
├── CT Capacity
│   Capacity (bbl/ft) = ID² / 1029.4
│
├── Annular Capacity (CT in tubing)
│   Cap (bbl/ft) = (Tubing ID² - CT OD²) / 1029.4
│
├── Volume in CT String
│   Volume (bbl) = Capacity × Depth
│
└── Strokes to Displace
    Strokes = Volume / Pump Output

PRESSURE CALCULATIONS
├── Friction Pressure
│   ΔP = f × (L/D) × (ρV²/2)
│   (Use friction factor charts)
│
├── Burst Pressure
│   P = (2 × t × S) / OD
│   Where: t = wall, S = yield
│
└── Hydrostatic
    HP = MW × 0.052 × TVD
```

### CT Hydraulics

| CT Size | ID | Flow Rate Range | Typical ΔP/1000 ft |
|---------|-----|-----------------|-------------------|
| 1.50" | 1.19" | 0.3-1.0 bpm | 200-800 psi |
| 2.00" | 1.65" | 0.5-2.0 bpm | 100-400 psi |
| 2.375" | 1.99" | 1.0-3.0 bpm | 50-200 psi |
| 2.875" | 2.47" | 1.5-5.0 bpm | 30-100 psi |

---

*Understanding CT fundamentals is essential for safe and effective operations. Always verify equipment specifications for your specific application.*
