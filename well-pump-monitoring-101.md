# Well Pump Monitoring 101

## The Problem

Most homeowners have very little visibility into how their well system is operating.

The well pump is one of the most important pieces of equipment in the home, yet many people do not know there is a problem until they lose water completely.

Unlike a freezer, dehumidifier, or sump pump, a well system often provides warning signs before failure occurs.

- Pressure changes
- Runtime changes
- Short cycling
- Extended run times
- Unexpected power consumption
- Loss of pressure

Many of these symptoms can appear days, weeks, or even months before complete failure occurs.

Most well pump failures are expensive.

Many are preventable.

The goal of this project is not to automate the well pump.

The goal is to understand its behavior, identify developing problems, and provide early warning before complete failure occurs.

---

## Failure Modes

Every monitoring project begins with the same question:

**What can fail?**

A well system contains several components that can develop problems over time.

Common failure modes include:

- Pressure tank failure
- Waterlogged pressure tank
- Pressure switch failure
- Leaking plumbing
- Stuck check valve
- Pump motor failure
- Worn pump bearings
- Dry well conditions
- Electrical issues
- Pipe leaks

Many of these failures create detectable changes long before complete system failure.

Monitoring allows us to recognize those changes early.

---

## What To Monitor

The first step is deciding what information is useful.

For this project, the primary areas of interest are:

- System pressure
- Pump runtime
- Pump power consumption
- Water flow
- Operating patterns

Individually, these measurements provide information.

Combined, they create awareness.

Over time they establish a baseline that helps identify abnormal behavior.

---

## Proposed Architecture

The exact design of this project is still evolving as testing continues.

The current concept is centered around collecting information from multiple sources and combining that information inside Home Assistant.

Potential monitoring inputs include:

- Pressure transducer
- Power monitoring
- Flow monitoring
- Runtime analysis
- Historical trends

The goal is not to monitor a single value.

The goal is to understand how the entire well system behaves over time.

By combining multiple data sources, abnormal conditions can often be identified before complete failure occurs.

As testing continues, this architecture may evolve based on reliability, accuracy, safety, and ease of implementation.

The final design will prioritize awareness, simplicity, and practical long-term maintenance.

---

## Pressure Monitoring

Pressure is one of the most valuable indicators of system health.

A healthy well system should operate within a predictable pressure range.

Monitoring pressure can help identify:

- Pressure tank issues
- Plumbing leaks
- Pressure switch problems
- Pump performance changes
- Water usage abnormalities

Pressure data often reveals developing issues before they become emergencies.

---

## Current Hardware Candidates

The exact hardware selection for this project is still under evaluation.

The goal is to balance reliability, accuracy, safety, and ease of implementation.

Potential hardware under consideration includes:

### Pressure Monitoring

Current candidate:

- IFM pressure transducer currently available from previous projects

Considerations:

- Pressure range suitability
- Resolution within the operating range of the well system
- Long-term reliability
- Ease of integration with ESPHome and Home Assistant

### Power Monitoring

Current candidates:

- Current Transformers (CTs)
- Alternative non-invasive monitoring methods

Considerations:

- Installation complexity
- Measurement accuracy
- Safety
- Homeowner accessibility

### Flow Monitoring

Potential candidates:

- Inline flow sensors
- Water meter pulse outputs
- Alternative flow measurement solutions

Considerations:

- Accuracy
- Pressure loss
- Installation requirements
- Long-term reliability

### Controller Hardware

Current candidates:

- ESP32
- ESPHome
- Home Assistant

The final hardware selection will be determined through testing and evaluation as the project develops.

---

## Power Monitoring

Power monitoring provides insight into how hard the pump is working.

Changes in power consumption may indicate:

- Increased mechanical load
- Pump wear
- Motor problems
- Changes in water demand
- Developing system issues

Power monitoring also allows runtime tracking.

Runtime trends often reveal problems long before complete failure occurs.

---

## Flow Monitoring

Flow monitoring helps answer an important question:

**Where is the water going?**

Flow information can help identify:

- Hidden leaks
- Continuous water usage
- Irrigation issues
- Abnormal consumption patterns

Flow data provides context that pressure and power monitoring alone cannot provide.

---

## Alert Strategy

Monitoring is only useful if it provides actionable information.

Alerts should focus on abnormal conditions rather than generating constant notifications.

Examples include:

- Pressure outside the normal range
- Excessive pump runtime
- Unusual power consumption
- Continuous flow detection
- Loss of pressure

The objective is awareness, not alarm fatigue.

---

## Power Monitoring Considerations

Power monitoring is one of the most valuable tools available for understanding well pump behavior.

For this project, I am currently evaluating multiple methods of measuring pump operation and electrical load.

One option is the use of current transformers (CTs), which are a proven and widely used method for monitoring electrical equipment.

CTs can provide valuable information including:

- Pump runtime
- Electrical load
- Operating patterns
- Potential signs of mechanical wear
- Changes in system demand

The primary drawback is that CT installation often requires access to electrical panels or conductors, which may not be appropriate for every homeowner.

Because of this, I am also exploring alternative monitoring methods that may provide useful information while reducing installation complexity.

At the time of writing, CT-based monitoring remains the most likely solution for this project.

As the project develops, monitoring methods may change based on testing, accuracy, safety, and ease of implementation.

If homeowners are not comfortable working inside electrical equipment, they should consult a qualified electrician.

---

## Future Improvements

This project will continue to evolve over time.

Potential future additions include:

- Historical pressure trending
- Advanced runtime analysis
- Flow-based diagnostics
- Predictive maintenance alerts
- Additional failure detection methods

The more patterns we understand, the more useful the monitoring system becomes.

---

## Lessons Learned

The most valuable lesson is that monitoring creates awareness.

Awareness creates understanding.

Understanding creates informed decisions.

Most equipment does not fail without warning.

The warning signs are often there.

We simply are not measuring them.

At Tug's Garage, the goal is not to automate everything.

The goal is to understand how systems behave, recognize changes early, and solve problems before they become emergencies.

**Awareness before automation.**

**Always.**
