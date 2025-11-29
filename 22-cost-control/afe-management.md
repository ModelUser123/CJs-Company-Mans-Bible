# AFE Management

## Understanding the AFE

### AFE Components

```
AFE STRUCTURE
├── Header Information
│   ├── Well name and location
│   ├── API number
│   ├── AFE number
│   ├── Working interest owners
│   ├── Approval date
│   └── Estimated duration
├── Intangible Costs
│   ├── Drilling contractor
│   ├── Fuel and water
│   ├── Drilling fluids
│   ├── Directional services
│   ├── Cementing
│   ├── Logging
│   ├── Rentals
│   ├── Transportation
│   ├── Supervision
│   └── Other services
├── Tangible Costs
│   ├── Casing and tubing
│   ├── Wellhead equipment
│   ├── Completion equipment
│   ├── Production equipment
│   └── Pumping equipment
├── Completion Costs
│   ├── Perforating
│   ├── Stimulation
│   ├── Testing
│   └── Flowback
└── Contingency
    ├── Typically 10-15%
    ├── For unexpected events
    └── May require approval to use
```

### Budget Line Items

| Category | Typical % | Key Items |
|----------|-----------|-----------|
| Drilling rig | 25-35% | Day rate, personnel, fuel |
| Mud/fluids | 8-12% | Products, engineering, disposal |
| Directional | 10-15% | MWD/LWD, motors, surveys |
| Cementing | 3-6% | Primary and remedial |
| Logging | 2-4% | Wireline, LWD data |
| Casing/tubing | 15-20% | Pipe, accessories, running |
| Rentals | 3-5% | BOP, tools, equipment |
| Completion | 10-20% | Perforating, stimulation |
| Other | 5-10% | Fuel, trucking, supervision |
| Contingency | 10-15% | Unexpected events |

## AFE Tracking

### Daily Tracking Process

```
DAILY AFE TRACKING
├── Input Daily Costs
│   ├── From field tickets
│   ├── From daily cost sheet
│   ├── Categorize correctly
│   └── Running cumulative total
├── Compare to Budget
│   ├── Line item actual vs budget
│   ├── Category actual vs budget
│   ├── Total actual vs budget
│   └── Calculate variance
├── Calculate Metrics
│   ├── % of budget spent
│   ├── % of well complete
│   ├── Cost per foot
│   ├── Days vs estimate
│   └── Projected final cost
├── Identify Issues
│   ├── Line items over budget
│   ├── Categories trending over
│   ├── Unexpected costs
│   └── NPT impact
└── Report Status
    ├── To management
    ├── Highlight variances
    ├── Explain causes
    └── Forecast final
```

### AFE Tracking Template

```
AFE TRACKING SPREADSHEET
═══════════════════════════════════════════════════
Well: _____________ AFE#: _________ Date: _________
══════════════════════════════════════════════════

                           AFE      ACTUAL   VARIANCE
                          BUDGET
─────────────────────────────────────────────────────
INTANGIBLE DRILLING
├── Rig contract        $______   $______   $______
├── Fuel                $______   $______   $______
├── Mud services        $______   $______   $______
├── Directional         $______   $______   $______
├── Cementing           $______   $______   $______
├── Logging             $______   $______   $______
├── Rentals             $______   $______   $______
├── Transportation      $______   $______   $______
├── Supervision         $______   $______   $______
└── Other services      $______   $______   $______
─────────────────────────────────────────────────────
INTANGIBLE SUBTOTAL     $______   $______   $______

TANGIBLE
├── Casing              $______   $______   $______
├── Tubing              $______   $______   $______
├── Wellhead            $______   $______   $______
└── Other equipment     $______   $______   $______
─────────────────────────────────────────────────────
TANGIBLE SUBTOTAL       $______   $______   $______

COMPLETION
├── Perforating         $______   $______   $______
├── Stimulation         $______   $______   $______
├── Testing             $______   $______   $______
└── Flowback            $______   $______   $______
─────────────────────────────────────────────────────
COMPLETION SUBTOTAL     $______   $______   $______

CONTINGENCY             $______   $______   $______
─────────────────────────────────────────────────────
TOTAL                   $______   $______   $______

SUMMARY:
├── % of AFE spent: ______%
├── % of well complete: ______%
├── Days elapsed: ___ of ___ budgeted
├── Projected total: $______
└── Status: On Track / Over / Under
═══════════════════════════════════════════════════
```

## Variance Analysis

### Calculating Variance

```
VARIANCE CALCULATIONS
├── Dollar Variance
│   Variance ($) = Actual - Budget
│   ├── Positive = Over budget
│   └── Negative = Under budget
│
├── Percentage Variance
│   Variance (%) = (Actual - Budget) / Budget × 100
│   ├── Positive = Over budget
│   └── Negative = Under budget
│
├── Earned Value Analysis
│   ├── BCWS = Budgeted cost of work scheduled
│   ├── BCWP = Budgeted cost of work performed
│   ├── ACWP = Actual cost of work performed
│   ├── SV = BCWP - BCWS (Schedule variance)
│   └── CV = BCWP - ACWP (Cost variance)
│
└── Forecast at Completion
    ├── EAC = ACWP + (Budget - BCWP)
    ├── Assumes future as planned
    └── Or adjust for trends
```

### Common Variance Causes

| Category | Over Budget Causes | Under Budget Causes |
|----------|-------------------|---------------------|
| Rig | NPT, slow ROP, extended ops | Fast drilling, efficiency |
| Mud | Losses, problems, expensive products | Lower usage, good hole |
| Directional | Surveys, motor problems, slides | Fast curve, RSS |
| Cement | Remedial work, squeeze | Clean cement jobs |
| Casing | Extra joints, problems | Efficient running |
| Logging | Additional runs, problems | Logs as planned |

### Variance Reporting

```
VARIANCE REPORT FORMAT
═══════════════════════════════════════════════════
AFE VARIANCE REPORT
Well: _____________ Date: _________
══════════════════════════════════════════════════

CURRENT STATUS:
├── Well progress: __% complete
├── Budget spent: __% ($_____ of $_____)
├── Overall variance: $_____ (__%)
└── Trend: Improving / Stable / Worsening

SIGNIFICANT VARIANCES:
┌────────────┬─────────┬─────────┬─────────┐
│ Category   │ Budget  │ Actual  │ Variance│
├────────────┼─────────┼─────────┼─────────┤
│ _________  │ $______ │ $______ │ $______ │
│ _________  │ $______ │ $______ │ $______ │
│ _________  │ $______ │ $______ │ $______ │
└────────────┴─────────┴─────────┴─────────┘

VARIANCE EXPLANATIONS:
├── _______________: ____________________________
├── _______________: ____________________________
└── _______________: ____________________________

CORRECTIVE ACTIONS:
├── _____________________________________________
├── _____________________________________________
└── _____________________________________________

FORECAST:
├── Projected final cost: $_____
├── Variance from AFE: $_____ (__%)
├── Contingency required: $_____ of $_____
└── Supplement needed: Yes / No

RECOMMENDATIONS:
_________________________________________________
_________________________________________________
═══════════════════════════════════════════════════
```

## AFE Supplement Process

### When Supplement Required

```
AFE SUPPLEMENT TRIGGERS
├── Automatic Triggers
│   ├── Expenditure will exceed AFE
│   ├── Scope change required
│   ├── Major unplanned operations
│   └── Per company policy threshold
├── Timing
│   ├── Request BEFORE exceeding AFE
│   ├── Allow time for approval
│   ├── Document need thoroughly
│   └── Continued operations may need interim approval
├── Documentation Needed
│   ├── Current AFE summary
│   ├── Detailed variance analysis
│   ├── Cause of overrun
│   ├── Proposed additional cost
│   ├── Total revised estimate
│   └── Justification
└── Approval Process
    ├── Submit to management
    ├── Partner notification (if JV)
    ├── Approval at appropriate level
    ├── Revised AFE issued
    └── Update tracking
```

### Supplement Request Format

```
AFE SUPPLEMENT REQUEST
═══════════════════════════════════════════════════
Date: _________
Well: _____________ AFE#: _________
══════════════════════════════════════════════════

CURRENT AFE STATUS:
├── Original AFE: $_________
├── Current expenditure: $_________
├── Remaining AFE: $_________
└── Estimated cost to complete: $_________

SUPPLEMENT REQUESTED: $_________
REVISED TOTAL AFE: $_________

REASON FOR SUPPLEMENT:
_________________________________________________
_________________________________________________
_________________________________________________

DETAILED BREAKDOWN:
┌────────────────┬───────────┬────────────┐
│ Item           │ Original  │ Revised    │
├────────────────┼───────────┼────────────┤
│ ______________ │ $________ │ $_________ │
│ ______________ │ $________ │ $_________ │
│ ______________ │ $________ │ $_________ │
└────────────────┴───────────┴────────────┘

ALTERNATIVES CONSIDERED:
_________________________________________________

RECOMMENDATION:
_________________________________________________

REQUESTED BY: _____________ DATE: _________
APPROVED BY:  _____________ DATE: _________
═══════════════════════════════════════════════════
```

## Post-Well Analysis

### Well Cost Summary

```
POST-WELL COST ANALYSIS
├── Final Cost Summary
│   ├── Total well cost
│   ├── Cost per foot
│   ├── Cost per day
│   ├── Comparison to AFE
│   └── Comparison to offsets
├── Category Analysis
│   ├── Each category actual vs budget
│   ├── Identify major variances
│   ├── Document causes
│   └── Lessons for future
├── Time Analysis
│   ├── Total days
│   ├── Drilling days
│   ├── Completion days
│   ├── NPT days and cost
│   └── Comparison to plan
├── Efficiency Metrics
│   ├── Drilling footage/day
│   ├── ROP by section
│   ├── Trip speed
│   └── Connection time
└── Recommendations
    ├── Future AFE improvements
    ├── Vendor performance
    ├── Process improvements
    └── Cost saving opportunities
```

---

*Effective AFE management requires continuous tracking, early identification of variances, and proactive communication with management.*
