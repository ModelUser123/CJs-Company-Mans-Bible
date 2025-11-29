# Daily Drilling Reports (DDR)

## Overview

The Daily Drilling Report is the official record of drilling operations. It serves as the primary communication tool, cost tracking document, and legal record of operations.

---

## Report Requirements

### Mandatory Information

**Header:**
- Well name and number
- API/UWI number
- Operator name
- Report date and number
- Spud date
- Current depth (MD/TVD)
- Days since spud

**Depth Information:**
- Previous depth (MD/TVD)
- Present depth (MD/TVD)
- Footage drilled
- Casing depth
- Liner depth (if applicable)

**Time Breakdown:**
- Drilling hours
- Tripping hours
- Circulating hours
- Reaming hours
- Casing/cementing hours
- Logging hours
- NPT hours (detailed)
- Other operations

**Drilling Parameters:**
- Weight on bit (WOB)
- Rotary speed (RPM)
- Flow rate (GPM)
- Pump pressure (psi)
- Torque (ft-lbs)
- ROP (ft/hr)

**Mud Properties:**
- Mud weight (ppg)
- Viscosity (sec/qt)
- Plastic viscosity (cP)
- Yield point (lb/100ft²)
- Gel strength (10 sec/10 min)
- Fluid loss (ml/30 min)
- pH
- Chlorides (ppm)

**BHA Information:**
- Bit type and size
- Bit hours and footage
- BHA description
- Survey data (if applicable)

---

## Time Codes

### Standard IADC Time Codes

| Code | Description |
|------|-------------|
| 1 | Rigging up/down |
| 2 | Drilling |
| 3 | Coring |
| 4 | Conditioning mud |
| 5 | Circulating |
| 6 | Tripping |
| 7 | Reaming/back reaming |
| 8 | Casing/tubing |
| 9 | Fishing |
| 10 | DST |
| 11 | Completion |
| 12 | Wireline |
| 13 | Stuck pipe |
| 14 | Lost circulation |
| 15 | Deviation survey |
| 16 | Logging |
| 17 | Well control |
| 18 | Wait on weather |
| 19 | Wait on orders |
| 20 | Other (specify) |

### NPT Codes (Detailed)

| Code | Description |
|------|-------------|
| N1 | Equipment failure - rig |
| N2 | Equipment failure - service |
| N3 | Stuck pipe |
| N4 | Lost circulation |
| N5 | Well control |
| N6 | Weather |
| N7 | Waiting - third party |
| N8 | Waiting - operator |
| N9 | Hole problems |
| N10 | Other NPT |

---

## Reporting Best Practices

### Narrative Section

**DO Include:**
- Sequential description of all operations
- Times for each operation
- Depths for depth-related activities
- Volumes (mud, cement, pills)
- Personnel and equipment involved
- Problems encountered and solutions
- Decisions made and rationale
- Key observations

**Example Good Narrative:**
```
0600-0730: Circulated and conditioned mud. Mud weight 10.2 ppg, 
vis 38 sec. Pumped 50 bbl hi-vis sweep.

0730-0800: POOH from 8,500' to surface. No drag or tight spots 
noted. Pulled wet.

0800-0900: Laid down bit #3, 8.5" PDC Smith MDi519, 74 hrs, 
2,156'. Dull grade: 2-2-WT-A-X-I-NO-TD. Replaced with bit #4, 
same type. Made up BHA per program.

0900-1000: RIH to 8,500'. Tagged bottom at 8,498', 2' fill. 
Circulated clean.

1000-1800: Drilled 8,500'-9,200' (700' in 8 hrs, avg ROP 87.5 ft/hr). 
WOB 15-20K, RPM 120, 850 GPM, 2,800 psi. Good drilling, no problems.
```

### Cost Tracking Section

**Daily Costs:**
- Rig (operating, standby)
- Mud and chemicals
- Rental tools
- Services (directional, mud logging, etc.)
- Fuel
- Water
- Miscellaneous

**Cumulative Tracking:**
| Category | Daily | Cumulative | AFE | Variance |
|----------|-------|------------|-----|----------|
| Rig | | | | |
| Services | | | | |
| Materials | | | | |
| Total | | | | |

---

## Survey Reporting

### Survey Data Requirements

| Field | Description |
|-------|-------------|
| Depth (MD) | Measured depth of survey |
| Inclination | Degrees from vertical |
| Azimuth | Compass direction |
| TVD | True vertical depth |
| VS | Vertical section |
| NS | North-South coordinate |
| EW | East-West coordinate |
| DLS | Dogleg severity |

### Survey Table Format

| MD | Inc | Azi | TVD | VS | DLS |
|----|-----|-----|-----|----|----|
| | | | | | |

---

## Safety and Environmental

### Daily Safety Section

```
□ Safety meeting held (topic: _________)
□ JSAs reviewed for planned work
□ BOP drill conducted (if applicable)
□ Incidents: None / See incident report
□ Near misses: None / Description
□ Safety observations: Number submitted
□ Visitors on location: List names
```

### Environmental Section

```
□ Spills: None / See spill report
□ Waste volumes: Oil___ Water___ Solids___
□ Air emissions: Normal / Issues
□ Wildlife observations: None / Description
□ Weather: Conditions
```

---

## Report Distribution

### Standard Distribution List

| Recipient | Method | Timing |
|-----------|--------|--------|
| Operations Manager | Email | By 0700 |
| Drilling Engineer | Email | By 0700 |
| Geologist | Email | By 0700 |
| Partners | Email | By 0800 |
| Regulatory (if required) | Portal | Per regulation |
| Contractor | Email | By 0800 |

### Report Timing

- **End of day report**: Within 2 hours of midnight
- **Morning report**: By 0800 local
- **Interim updates**: As required for significant events

---

## Quality Control

### Report Review Checklist

```
□ All times account for 24 hours
□ Depths accurate and consistent
□ Survey data included (if taken)
□ Mud properties complete
□ Costs accurate
□ Narrative sequential and clear
□ NPT properly coded and explained
□ Safety section complete
□ All required signatures
```

### Common Errors to Avoid

1. **Time gaps**: All 24 hours must be accounted for
2. **Depth discrepancies**: MD/TVD must be consistent
3. **Vague narrative**: Include specific details
4. **Missing costs**: All daily costs must be captured
5. **NPT attribution**: Clearly identify cause
6. **Late distribution**: Reports must be timely

---

## Electronic Reporting Systems

### Common Platforms

- WellView
- OpenWells
- Pason
- Erdos Miller
- Landmark

### System Requirements

```
□ Data entry complete by end of tour
□ Supervisory review and approval
□ Electronic signature/authorization
□ Distribution automated
□ Archive maintained
```

---

## Report Templates

### 24-Hour Operations Summary

```
DAILY DRILLING REPORT #___

Well: _________________ Date: _____________
Operator: _____________ Spud Date: ________

DEPTH SUMMARY:
Previous Depth: _______ MD / _______ TVD
Present Depth:  _______ MD / _______ TVD
Footage:        _______
Progress:       On Schedule / Behind / Ahead

TIME BREAKDOWN (24 hours):
Drilling:        ___ hrs
Tripping:        ___ hrs  
Circulating:     ___ hrs
Casing/Cement:   ___ hrs
Logging:         ___ hrs
NPT:             ___ hrs (Reason: _________)
Other:           ___ hrs

OPERATIONS NARRATIVE:
_________________________________________________
_________________________________________________
_________________________________________________

PLANNED OPERATIONS (Next 24 hrs):
_________________________________________________

COST SUMMARY:
Daily:      $___________
Cumulative: $___________
AFE:        $___________
Variance:   ____%

Reported by: _________________ Time: _______
```

---

## Related Documents

- [Cost Tracking](../07-cost-vendor-management/cost-tracking.md)
- [Drilling Parameters](./drilling-parameters.md)
- [Incident Reporting](../06-hse-compliance/incident-reporting.md)
