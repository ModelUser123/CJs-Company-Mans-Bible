# Workover Planning

## Pre-Workover Analysis

### Well Data Gathering

```
ESSENTIAL WELL DATA
├── Well Configuration
│   ├── Casing program (sizes, depths, grades)
│   ├── Cement tops (per bond logs)
│   ├── Tubing size, depth, grade
│   ├── Packer type, depth, restrictions
│   ├── Downhole equipment (SCSSV, nipples)
│   └── Artificial lift equipment
├── Pressure Data
│   ├── Current SITP/SICP
│   ├── Bottom hole pressure
│   ├── Formation pressure (original, current)
│   ├── Fracture gradient
│   └── Wellhead rating
├── Production Data
│   ├── Current/historical rates
│   ├── Water cut history
│   ├── GOR history
│   ├── Problems encountered
│   └── Last test results
└── Problem Diagnosis
    ├── Reason for workover
    ├── Suspected failure mode
    ├── Downhole conditions
    └── Surface observations
```

### Kill Fluid Design

```
KILL FLUID REQUIREMENTS
├── Weight Calculation
│   ├── BHP = Formation Pressure + Safety Margin
│   ├── Safety Margin = 100-500 psi typical
│   ├── Kill Weight = BHP ÷ 0.052 ÷ TVD
│   └── Consider depletion
├── Volume Requirements
│   ├── Tubing capacity
│   ├── Casing capacity (below packer)
│   ├── Annulus capacity
│   ├── Excess volume (1.5-2×)
│   └── Reserve for circulation
├── Fluid Type Selection
│   ├── Brine (KCl, NaCl, CaCl₂, CaBr₂)
│   ├── Oil-based (diesel, crude)
│   ├── Completion fluid
│   └── Formation compatibility
└── Treatment
    ├── Oxygen scavenger
    ├── Biocide
    ├── Scale inhibitor
    ├── H2S scavenger (if needed)
    └── Corrosion inhibitor

BRINE WEIGHT RANGES
├── Potassium Chloride: 8.4-9.7 ppg
├── Sodium Chloride: 8.4-10.0 ppg
├── Calcium Chloride: 8.4-11.7 ppg
├── Sodium Bromide: 8.4-12.5 ppg
├── Calcium Bromide: 8.4-15.1 ppg
└── Zinc Bromide: 14.5-19.2 ppg
```

### Equipment Selection

| Operation | Equipment Required | Capacity Check |
|-----------|-------------------|----------------|
| Pull tubing | Pulling unit/rig | String weight + overpull |
| Run tubing | Same | String weight |
| Circulate | Kill pump | Rate and pressure |
| Cement | Cement unit | Volume and rate |
| Fish | Fishing tools | Match to completion |
| Test | Test equipment | Test pressure |

## Workover Procedures

### Well Kill Procedure

```
BULLHEAD KILL
├── When to Use
│   ├── Tubing open to formation
│   ├── No circulation path
│   └── Quick kill needed
├── Procedure
│   ├── Calculate required volume
│   ├── Connect kill line
│   ├── Pump kill fluid slowly
│   ├── Monitor pressure response
│   ├── Continue until stabilized
│   └── Verify kill (flow check)
├── Limitations
│   ├── May damage formation
│   ├── High pressures possible
│   └── May not achieve full kill
└── Rate: 0.5-2 bpm typical

CIRCULATING KILL
├── When to Use
│   ├── Can circulate through tubing
│   ├── Tubing packer not seated
│   └── Preferred method
├── Procedure
│   ├── Pump down tubing
│   ├── Returns up annulus (or reverse)
│   ├── Displace well fluids
│   ├── Monitor returns
│   └── Verify kill
├── Advantages
│   ├── Better fluid placement
│   ├── Lower pressures
│   └── Complete displacement
└── Rate: 1-4 bpm typical
```

### Pulling Completion

```
PULLING TUBING PROCEDURE
├── Pre-Pull Checks
│   ├── Well killed and verified
│   ├── BOPs installed and tested
│   ├── Handling equipment ready
│   ├── Tally known
│   └── Fluids available
├── Initial Steps
│   ├── Bleed off pressure
│   ├── Remove wellhead
│   ├── Install BOPs
│   ├── Space out if needed
│   └── Rig up handling
├── Pulling Operations
│   ├── Pick up slowly
│   ├── Monitor for stuck/tight
│   ├── Fill well as tubing removed
│   ├── Inspect each joint
│   │   ├── Corrosion
│   │   ├── Erosion
│   │   ├── Thread damage
│   │   └── Mechanical damage
│   └── Rack in organized manner
├── Packer Retrieval
│   ├── Follow specific procedure
│   ├── Set down for release
│   ├── Right-hand rotation (typically)
│   ├── Overpull if stuck
│   └── May need to mill
└── Well Bore Access
    ├── Run bit/scraper
    ├── Verify casing condition
    ├── Clean out fill
    └── Ready for next step
```

### Running New Completion

```
RUNNING COMPLETION
├── Preparation
│   ├── All equipment on location
│   ├── Inspected and tested
│   ├── Makeup torques specified
│   ├── Centralizers positioned
│   └── Running speed calculated
├── Running In Hole
│   ├── Fill tubing while running
│   ├── Proper connection makeup
│   ├── Control running speed
│   ├── Watch for resistance
│   └── Space out at surface
├── Packer Setting
│   ├── At correct depth
│   ├── Set per manufacturer
│   ├── Verify set (pickup weight)
│   ├── Test if applicable
│   └── Document setting
├── Final Assembly
│   ├── Tubing hanger
│   ├── Wellhead installation
│   ├── Pressure test
│   │   ├── Tubing
│   │   ├── Annulus
│   │   └── Wellhead
│   └── SCSSV test
└── Well Return to Production
    ├── Unload kill fluid
    ├── Gradual choke opening
    ├── Monitor for problems
    └── Normal operations
```

## Common Workover Operations

### Tubing Replacement

```
TUBING CHANGE-OUT
├── Reasons
│   ├── Leak/failure
│   ├── Corrosion
│   ├── Scale buildup
│   ├── Size change needed
│   └── Grade upgrade
├── Procedure
│   ├── Kill well
│   ├── Pull existing tubing
│   ├── Inspect/clean wellbore
│   ├── Run new tubing
│   └── Test and return to production
├── Considerations
│   ├── Match thread type
│   ├── Consider premium connections
│   ├── Corrosion-resistant if needed
│   └── Properly torque all connections
└── Duration: 2-5 days typical
```

### Packer Replacement

```
PACKER CHANGE-OUT
├── Assessment
│   ├── Packer type (retrievable, permanent)
│   ├── Set depth
│   ├── Condition
│   └── Reason for failure
├── Retrievable Packer
│   ├── Follow release procedure
│   ├── Rotation, weight, or J-slot
│   ├── Pull with tubing
│   └── Inspect on surface
├── Permanent Packer
│   ├── Mill/drill out required
│   ├── Time consuming
│   ├── Debris management
│   └── Verify clean bore
└── New Packer Installation
    ├── Select appropriate type
    ├── Size for casing ID
    ├── Set at correct depth
    ├── Verify set
    └── Test
```

### Artificial Lift Changes

| Lift Type | Typical Workover Activities |
|-----------|----------------------------|
| Rod pump | Replace rods, pump, tubing |
| ESP | Pull/run pump, cable, tubing |
| Gas lift | Pull/run mandrels, valves |
| PCP | Replace rotor, stator, tubing |
| Plunger | Replace plunger, tubing work |

## Troubleshooting Workover Problems

### Stuck Tubing

```
STUCK TUBING RESPONSE
├── Indicators
│   ├── Cannot pick up string
│   ├── Overpull required
│   ├── No movement with jarring
│   └── Torque change if rotating
├── Causes
│   ├── Scale/paraffin buildup
│   ├── Corrosion products
│   ├── Sand fill
│   ├── Key seat
│   ├── Collapsed casing
│   └── Formation movement
├── Initial Response
│   ├── Note depth of stick
│   ├── Apply controlled overpull
│   ├── Work pipe up/down
│   ├── Circulate if possible
│   └── Jar if equipped
├── Remedial Options
│   ├── Soak with solvent
│   ├── Chemical treatment
│   ├── Wash over
│   ├── Cut and fish
│   └── Back off above
└── Prevention
    ├── Regular circulation
    ├── Chemical treatments
    └── Planned maintenance
```

### Lost Circulation During Workover

| Severity | Action |
|----------|--------|
| Seepage | Continue, monitor |
| Partial | LCM treatment |
| Complete | Stop, pump LCM, cement if needed |

### Well Control During Workover

```
WORKOVER WELL CONTROL
├── Prevention
│   ├── Accurate kill weight
│   ├── Maintain hole full
│   ├── Monitor trip tank
│   └── Watch for flow
├── If Kick Occurs
│   ├── Close BOPs
│   ├── Record pressures
│   ├── Calculate kill weight
│   ├── Kill well
│   └── Resume operations
├── Special Considerations
│   ├── Stripped completions
│   ├── Open hole completions
│   ├── Multiple zones
│   └── Depleted reservoirs
└── Documentation
    ├── Record all pressures
    ├── Log all events
    └── Report as required
```

## Post-Workover

### Testing and Startup

```
POST-WORKOVER TESTING
├── Pressure Tests
│   ├── Tubing: To expected operating
│   ├── Annulus: To rating or BOP test
│   ├── SCSSV: Surface and subsurface
│   └── Wellhead: Flange tests
├── Well Tests
│   ├── Production test
│   ├── Build-up test
│   ├── Compare to pre-workover
│   └── Document results
├── Startup Procedure
│   ├── Gradual opening
│   ├── Monitor pressures
│   ├── Watch for problems
│   └── Optimize as needed
└── Documentation
    ├── Completion report
    ├── As-completed diagram
    ├── All test results
    └── Recommendations
```

### Workover Reporting

| Report | Content | Timing |
|--------|---------|--------|
| Daily report | Operations, costs, progress | Daily |
| Final report | Summary, costs, results | Completion |
| Regulatory | As required by state/federal | Per requirements |
| Lessons learned | What worked, problems, fixes | Post-job |

---

*Successful workovers require thorough planning and attention to detail. Expect the unexpected and have contingency plans ready.*
