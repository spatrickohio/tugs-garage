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

## Why I Am Not Using CTs

Many monitoring projects use current transformers (CTs) to measure electrical load.

CTs are a proven and effective method for monitoring equipment power consumption.

As an electrician, I have no issue using CTs when the application calls for them.

However, installing CTs often requires opening electrical panels and working around energized conductors.

For many homeowners, that is not practical and may not be safe.

For this version of the project, I am exploring monitoring methods that provide useful information while minimizing electrical exposure and installation complexity.

The goal is to create solutions that more homeowners can realistically implement and maintain.

Future versions of this project may include CT-based monitoring if additional information or accuracy justifies the added complexity.

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
