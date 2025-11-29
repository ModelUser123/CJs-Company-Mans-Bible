# Kick Detection

## Overview

Early kick detection is critical to well control. The sooner a kick is detected, the smaller the influx and the easier the well kill.

---

## Primary Kick Indicators

### Pit Volume Increase (Flow Check)

**Most Reliable Indicator**

**Monitoring Requirements:**
- Active pit volume displayed at all times
- Alarm set for volume change (typically 5-10 bbl)
- Driller must monitor continuously

**Causes of Pit Gain:**
| Cause | Action |
|-------|--------|
| Kick | Shut in, verify |
| Rig pumps off/on | Verify, adjust |
| Transfer between pits | Verify, adjust |
| Rain | Verify, adjust |

### Flow Rate Increase

**Pump Running, Flow Increases**
- Returns greater than pump rate
- Indicates formation influx

**Monitoring:**
- Flow sensor at flowline
- Paddle-type or electromagnetic

### Flow with Pumps Off

**Most Serious Indicator**
- Well is flowing without circulation
- Immediate action required

**Response:**
1. Verify pumps are off
2. Observe flow
3. If flowing, shut in immediately

---

## Secondary Kick Indicators

### Drilling Break

**Definition:** Sudden increase in ROP

**Possible Causes:**
- Drilling into pressure (underbalanced)
- Formation change
- Bit dysfunction

**Response:**
1. Note depth and severity
2. Circulate bottoms up
3. Monitor for flow
4. Evaluate samples

### Pump Pressure Decrease

**Possible Causes:**
- Gas-cut mud (lighter column)
- Washout in string
- Lost nozzle
- Formation breakdown

**Response:**
1. Check for other indicators
2. Evaluate cause
3. Flow check if warranted

### Torque Increase

**Possible Causes:**
- Formation change
- Reactive formation (swelling)
- Underbalanced (formation support lost)

**Response:**
1. Monitor other parameters
2. Evaluate trend
3. Flow check if concerned

### Gas-Cut Mud

**Indicators:**
- Lower mud weight out
- Degasser working
- Gas detector response

**Evaluation:**
- Connection gas vs. formation kick
- Background gas levels
- Trend vs. single occurrence

**Response:**
1. Circulate out
2. Evaluate source
3. Weight up if required (actual influx)

---

## Monitoring Systems

### Pit Volume Totalizer (PVT)

**Purpose:** Track total mud volume in system

**Key Features:**
- Digital display at driller's console
- Alarm for volume change
- Trend recording

**Alarm Settings:**
| Condition | Typical Setting |
|-----------|-----------------|
| Gain | +5 to +10 bbl |
| Loss | -5 to -10 bbl |

### Flow Show Detector

**Types:**
- Paddle type
- Electromagnetic
- Coriolis

**Monitoring:**
- Flow rate trend
- Comparison to pump rate
- Alarm for deviation

### Mud Logging

**Gas Detection:**
- Total gas
- Component analysis (C1, C2, etc.)
- Background vs. connection gas

**Parameter Monitoring:**
- ROP
- Weight on bit
- Torque
- Pump pressure
- Pit volume

---

## Trip Monitoring

### Hole Fill Monitoring

**Critical During Trips**
- Hole must be filled to prevent swab
- Track fill volume vs. calculated

**Expected Fill:**

```
Fill Volume = Pipe Displacement × Stands Pulled

Pipe Displacement (bbl/ft) = (OD² - ID²) / 1029.4
```

### Trip Tank

**Purpose:** Accurate fill tracking

**Operation:**
1. Fill trip tank
2. Track volume used to fill hole
3. Compare to calculated
4. Investigate discrepancies

**Discrepancy Indicators:**
| Situation | Indication |
|-----------|------------|
| Less fill needed | Hole flowing |
| More fill needed | Hole losing |

### Trip Sheet

**Record:**
- Stands pulled
- Expected fill
- Actual fill
- Cumulative difference

```
TRIP SHEET

Well: _____________ Date: _____________
Trip out from: _______ MD

| Stands | Expected (bbl) | Actual (bbl) | Difference |
|--------|----------------|--------------|------------|
| 1-5    |                |              |            |
| 6-10   |                |              |            |
| ...    |                |              |            |

Total: _______ stands
Total Expected: _______ bbl
Total Actual: _______ bbl
Difference: _______ bbl
```

---

## Swab and Surge

### Swab Effects (Pulling Out)

**Reduces Bottom Hole Pressure**
- Can pull formation fluids into wellbore
- Effect increases with trip speed
- Effect increases with tight clearances

**Mitigation:**
- Control pulling speed
- Use trip margin
- Swab calculations before trip

### Surge Effects (Going In)

**Increases Bottom Hole Pressure**
- Can cause formation breakdown
- Can cause lost circulation
- Effect increases with trip speed

**Mitigation:**
- Control running speed
- Calculate surge pressures
- Monitor for losses

### Speed Limits

| Condition | Typical Limit |
|-----------|---------------|
| Open hole, vertical | 3-5 stands/min |
| Open hole, deviated | 2-3 stands/min |
| Tight clearances | 1-2 stands/min |
| Near balance | Minimum speed |

---

## Response to Indicators

### Flow Check Procedure

**When to Perform:**
- Drilling break
- Pit gain alarm
- Any primary indicator
- Any combination of secondary indicators

**Procedure:**
1. Pick up off bottom
2. Stop pumps
3. Observe well (3-5 minutes minimum)
4. Watch for flow at flowline
5. Monitor pit volume

**If Well Flows:**
- Shut in immediately
- Follow shut-in procedure
- Record pressures

**If No Flow:**
- Resume operations
- Document observation
- Heighten awareness

### Quick Response Guide

| Indicator | Immediate Action |
|-----------|------------------|
| Pit gain | Flow check |
| Flow increase | Verify, flow check |
| Flow, pumps off | Shut in immediately |
| Drilling break | Flow check |
| Gas-cut mud | Circulate, evaluate |
| Multiple indicators | Shut in |

---

## Special Situations

### Gas in Mud (While Circulating)

**Connection Gas:**
- Normal amount expected
- Increases with depth
- Evaluate trend

**Trip Gas:**
- Gas pulled in while tripping
- Circulate out before drilling

**Formation Kick:**
- Sustained gas levels
- Pit gain accompanies
- Requires well control action

### Ballooning

**Definition:** Wellbore breathes (takes mud when pumping, returns when stopped)

**Indicators:**
- Mild flow when pumps off
- Slight gains/losses
- Stabilizes without kick behavior

**Verification:**
- Close well on choke
- Monitor for pressure buildup
- True kick will pressure up
- Ballooning will stabilize or decrease

**Management:**
- Reduce ECD
- Adjust mud weight
- Manage LOT/FIT data

---

## Crew Training

### Kick Detection Training

**All Crew Members:**
- Recognize kick indicators
- Know immediate response
- Practice shut-in procedures

**Drillers:**
- Continuous monitoring responsibility
- Alarm response
- Shut-in authority

### Drills

**Weekly requirement:**
- Simulated kick detection
- Shut-in practice
- Response time measurement

---

## Related Documents

- [Well Control Procedures](./well-control-procedures.md)
- [Kill Procedures](./kill-procedures.md)
- [Mud Programs](../02-drilling-operations/mud-programs.md)
- [Emergency Action Plans](../08-emergency-response/emergency-action-plans.md)
