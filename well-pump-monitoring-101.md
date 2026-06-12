# Well Pump Monitoring 101

## Related Videos

📻 **Tug's Garage Radio:** Coming Soon

🎓 **Learning 101 Video:** Coming Soon

---

> **Project Status**
>
> This project is currently in the research and development phase.
>
> Hardware selection, sensor placement, dashboard design, and alert logic are still being evaluated through real-world testing.

## The Problem

Most homeowners have very little visibility into how their well system is operating.

The well pump is one of the most important pieces of equipment in the home, yet many people do not know there is a problem until they lose water completely.

Unlike a freezer, dehumidifier, or sump pump, a well system often provides warning signs before failure occurs.

Some common warning signs include:

- Pressure changes
- Runtime changes
- Short cycling
- Extended run times
- Unexpected power consumption
- Loss of pressure

Many of these symptoms can appear days, weeks, or even months before a major failure.

Most well pump failures are expensive.

Many are preventable.

---

## Project Goal

The goal of this project is not to automate the well pump.

The goal is to better understand how the well system behaves.

By monitoring power, runtime, pressure, and eventually flow, we can establish a normal operating baseline.

Once we understand normal behavior, abnormal behavior becomes easier to recognize.

This project focuses on awareness before failure.

---

## What Can Fail?

Every Tug's Garage monitoring project starts with the same question:

**What can fail?**

A well system may experience problems involving:

- The pump motor
- The pressure tank
- The pressure switch
- The check valve
- Plumbing leaks
- Dry well conditions
- Electrical problems
- Worn mechanical components
- Excessive water demand

Monitoring gives us a way to recognize changes before complete failure occurs.

---

## What Can We Measure?

Several measurements can provide valuable insight into the health of a well system.

These include:

- Pump runtime
- Pump cycle count
- Power consumption
- System pressure
- Pressure recovery time
- Water flow
- Historical trends
- Abnormal operating patterns

One sensor rarely tells the entire story.

Multiple measurements working together provide a much clearer picture of what is happening.

---

## Layered Monitoring Approach

This project is being built in layers.

### Layer 1: Power and Runtime Monitoring

The first layer is simply knowing when the pump runs.

This allows us to monitor:

- Pump runtime
- Cycle frequency
- Short cycling
- Long run times
- General operating patterns

### Layer 2: Pressure Monitoring

The second layer focuses on understanding system pressure.

Pressure monitoring can reveal:

- Pressure tank problems
- Pressure switch issues
- Pressure recovery performance
- Possible plumbing leaks
- Changes in pump performance

### Layer 3: Flow Monitoring

The third layer may include flow monitoring.

Flow monitoring helps answer one important question:

**Where is the water going?**

Flow data may help identify:

- Hidden leaks
- Continuous water usage
- Irrigation demand
- Unexpected consumption patterns

### Layer 4: Historical Trends

The final layer focuses on historical analysis.

Over time, collected data can establish a baseline and help identify subtle changes before they become major failures.

Each layer should provide useful information on its own.

The system should remain valuable even if every sensor has not yet been installed.

---

## Proposed Architecture

The current concept combines several data sources within Home Assistant.

Potential inputs include:

- Power monitoring
- Runtime analysis
- Pressure monitoring
- Flow monitoring
- Historical trend tracking

The goal is not to monitor a single value.

The goal is to understand how the entire well system behaves over time.

As testing continues, the architecture may evolve based on reliability, accuracy, safety, and ease of installation.

## Hardware Under Evaluation

The hardware for this project is still being evaluated.

Possible components include:

### Power Monitoring Hardware

- Current transformers (CTs)
- Energy monitoring boards
- CircuitSetup energy monitors
- ESPHome-compatible monitoring solutions

### Pressure Monitoring Hardware

- Pressure transducers
- Analog monitoring inputs
- Pressure trend logging

### Flow Monitoring Hardware

- Inline flow sensors
- Pulse-output water meters
- Alternative flow measurement methods

### Controller Hardware

- ESP32
- ESPHome
- Home Assistant

The final hardware selection will be determined through testing and real-world evaluation.

---

## Power Monitoring

Power monitoring provides insight into pump operation without modifying the well system itself.

Power data can help identify:

- Pump start events
- Excessive runtime
- Short cycling
- Increased motor load
- Abnormal operating patterns

For many 240-volt well pumps, CT monitoring offers a practical non-invasive monitoring method.

---

## Pressure Monitoring

Pressure is one of the most valuable indicators of well system health.

A properly functioning system should operate within a predictable pressure range.

Pressure monitoring may help identify:

- Pressure tank issues
- Pressure switch problems
- Plumbing leaks
- Poor pressure recovery
- Changes in pump performance

Pressure data provides context that power monitoring alone cannot provide.

---

## Flow Monitoring

Flow monitoring is currently considered a future expansion.

Power monitoring can tell us when the pump is running.

Pressure monitoring can tell us what the system pressure is doing.

Flow monitoring can help determine whether water is actually moving through the system.

This additional information may improve troubleshooting and leak detection capabilities.

---

## Alert Strategy

Monitoring is only useful if it provides actionable information.

Possible alert conditions include:

- Pump running too long
- Excessive cycle frequency
- Short cycling
- Pressure not recovering normally
- Pressure dropping while the pump is off
- Continuous water flow
- Unexpected pump operation
- Abnormal power consumption

The objective is awareness, not alarm fatigue.

---

## Safety Considerations

**Safety matters more than data.**

Well pump monitoring may involve:

- Electrical panels
- 240-volt circuits
- Current transformers
- Pressure plumbing
- Water system components

Homeowners should not work inside electrical panels or install CTs unless they are qualified and understand the hazards involved.

When in doubt, hire a licensed electrician or qualified professional.

This project is intended for education, testing, and documentation.

---

## Future Improvements

Potential future enhancements include:

- Improved pressure trend analysis
- Flow-based diagnostics
- Predictive maintenance alerts
- Water usage tracking
- Leak detection logic
- Dedicated well system dashboards
- Integration with whole-house water monitoring
- Additional failure detection strategies

The system does not need to be perfect on day one.

Each layer adds additional understanding.

---

## Lessons Learned

Monitoring creates awareness.

Awareness creates understanding.

Understanding leads to better decisions.

Most equipment does not fail without warning.

The warning signs are often there.

We simply are not measuring them yet.

At Tug's Garage, the goal is not to automate everything.

The goal is to understand how systems behave, recognize changes early, and solve problems before they become emergencies.

## Awareness Before Automation. Always.
