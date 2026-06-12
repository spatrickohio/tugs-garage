# Well Pump Monitoring 101

## Related Videos

**Tug's Garage Radio:** Coming Soon

**Learning 101 Video:** Coming Soon

---

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

Many of these symptoms can appear days, weeks, or even months before a major failure.

Most well pump failures are expensive.

Many are preventable.

---

## Project Goal

The goal of this project is not to automate the well pump.

The goal is to understand how the well system behaves.

By monitoring power, runtime, pressure, and eventually flow, we can start building a normal baseline.

Once we understand normal behavior, abnormal behavior becomes easier to recognize.

This project is about awareness before failure.

---

## What Can Fail?

Every Tug's Garage monitoring project starts with the same question:

**What can fail?**

A well system may have issues with:

- The pump motor
- The pressure tank
- The pressure switch
- The check valve
- Plumbing leaks
- Dry well conditions
- Electrical problems
- Worn mechanical parts
- Water usage patterns

Monitoring gives us a way to see changes before the system completely fails.

---

## What Can We Measure?

A well pump monitoring system can collect several useful pieces of information.

- Pump runtime
- Pump cycle count
- Power consumption
- System pressure
- Pressure recovery time
- Flow rate
- Water usage history
- Abnormal operating patterns

One sensor may not tell the whole story.

Several measurements together can give a much better picture of what is happening.

---

## Layered Monitoring Approach

This project is being built in layers.

### Layer 1: Power and Runtime Monitoring

The first layer is knowing when the pump runs.

This allows us to track:

- How often the pump starts
- How long the pump runs
- Whether the pump is short cycling
- Whether the pump is running longer than normal

### Layer 2: Pressure Monitoring

The second layer is monitoring system pressure.

Pressure monitoring can help show:

- Normal cut-in pressure
- Normal cut-out pressure
- Pressure recovery time
- Pressure drop when the pump is off
- Possible pressure tank issues
- Possible leaks

### Layer 3: Flow Monitoring

The third layer may include flow monitoring.

Flow monitoring helps answer one important question:

**Where is the water going?**

Flow monitoring may help detect:

- Hidden leaks
- Unexpected water usage
- Continuous flow
- Abnormal water demand
- Irrigation or outside water use

### Layer 4: Predictive Trends

The final layer is using history and trends.

Once the system has enough data, we can begin comparing current behavior to normal behavior.

This could help detect problems before they become emergencies.

---

## Hardware Under Evaluation

The hardware for this project is still being evaluated.

Possible hardware includes:

- CT-based power monitoring
- ESP32
- ESPHome
- Home Assistant
- Pressure transducer
- Flow sensor
- Energy monitoring board

The final hardware choice will depend on reliability, safety, accuracy, and how practical it is to install.

---

## Power Monitoring

Power monitoring tells us when the pump is running.

It may also help show how the pump is behaving electrically.

Power monitoring may help identify:

- Pump start events
- Long run times
- Short cycling
- Increased motor load
- Abnormal power usage
- Possible pump wear

For a 240-volt well pump, CT monitoring is usually a better option than a smart plug.

---

## Pressure Monitoring

Pressure monitoring is one of the most valuable parts of this project.

A healthy well system should operate within a predictable pressure range.

Pressure monitoring may help detect:

- Pressure tank problems
- Pressure switch problems
- Leaks
- Poor pressure recovery
- Pump performance changes
- Loss of pressure

Pressure data gives context that power monitoring alone cannot provide.

---

## Flow Monitoring

Flow monitoring is a future expansion for this project.

Power monitoring can tell us that the pump is running.

Pressure monitoring can tell us what the system pressure is doing.

Flow monitoring can help tell us whether water is actually moving.

That matters because a pump running with no useful water movement could indicate a serious problem.

---

## Alert Strategy

The purpose of alerts is not to create noise.

The purpose is to provide useful information when something changes.

Possible alerts include:

- Pump running too long
- Pump short cycling
- Pressure not recovering normally
- Pressure dropping while pump is off
- Pump running unexpectedly
- Continuous water flow
- Loss of pressure
- Abnormal power usage

The goal is awareness, not alarm fatigue.

---

## Safety Considerations

**Safety matters more than data.**

Well pump monitoring may involve:

- 240-volt circuits
- Electrical panels
- Current transformers
- Pressure plumbing
- Water system components

Homeowners should not open electrical panels or install CTs unless they are qualified and understand the hazards involved.

When in doubt, hire a licensed electrician or qualified professional.

This project is for education, testing, and documentation.

---

## Future Improvements

Possible future improvements include:

- Better pressure trend tracking
- Flow-based diagnostics
- Predictive maintenance alerts
- Water usage history
- Leak detection logic
- Well pump dashboard
- Integration with whole-house water monitoring
- Possible shutdown or interlock concepts

The system does not need to be perfect on day one.

Each layer adds more useful information.

---

## Lessons Learned

Monitoring creates awareness.

Awareness creates understanding.

Understanding leads to better decisions.

Most equipment does not fail without warning.

The warning signs are usually there.

We just are not measuring them yet.

At Tug's Garage, the goal is not to automate everything.

The goal is to understand how systems behave, recognize changes early, and solve problems before they become emergencies.

## Awareness Before Automation. Always.
