---
layout: page
title: Thermocycler Process Automation
category: Supporting Case File
tags: Automation · Controls · Diagnostics · Hardware
subtitle: PID-controlled thermal cycling hardware for rapid molecular-diagnostics workflows.
---

## Summary

This case file presents a thermocycler automation project focused on building repeatable thermal control for RT-qPCR-style workflows. The engineering challenge is turning a biological protocol into a controllable temperature-time process.

<div class="buildout-note">artifact buildout — add control-loop diagram, thermal-profile plot, and prototype notes as artifacts.</div>

<div class="role-block">
 <p class="system-label small">MY ROLE</p>
 <p>Prototyped an embedded-controller thermocycler, integrated heating/cooling and sensor feedback, tuned PID behavior, and evaluated ramp rate and steady-state temperature stability.</p>
</div>

<div class="connection-note"><strong>Connection to flagship:</strong> This project extends the same process-control mindset into automation: define the controlled variable, measure dynamic response, tune the system, and quantify repeatability.</div>

## Problem / motivation

PCR thermal cycling depends on repeatable heating and cooling between temperature setpoints. Poor thermal control creates inconsistent amplification conditions, slower workflows, and unreliable diagnostic performance.

## Control-loop schematic

<div class="project-schematic schematic-pfd" aria-label="Representative PID thermal control schematic">
 <div class="pfd-row"><span>SETPOINT</span><i></i><span>PID</span><i></i><span>HEATER / FAN</span><i></i><span>SENSOR</span></div>
 <p>Representative feedback-control loop for thermal cycling.</p>
</div>

## Engineering framing

<div class="matrix">
 <div class="matrix-card"><h3>Controlled variable</h3><p>Reaction-zone temperature over time during denaturation, annealing, and extension steps.</p></div>
 <div class="matrix-card"><h3>Manipulated variables</h3><p>Heater power, cooling fan behavior, dwell time, ramp profile, and controller tuning.</p></div>
 <div class="matrix-card"><h3>Performance metrics</h3><p>Ramp rate, overshoot, settling time, steady-state error, repeatability, and run-to-run stability.</p></div>
</div>

## Variables studied

| Variable | Why it matters |
|---|---|
| Ramp rate | Determines total cycle time and diagnostic speed. |
| Steady-state error | Determines whether the sample experiences the intended temperature. |
| Overshoot / undershoot | Can damage assay performance or reduce repeatability. |
| Sensor placement | Affects whether measured temperature represents sample temperature. |
| Controller gains | Determine stability, responsiveness, and oscillation behavior. |
| Heating/cooling balance | Sets whether the device can transition quickly without excessive lag. |

## Methods and tools

<div class="two-col">
 <div class="matrix-card"><h3>Hardware / control</h3><p>Embedded controller, temperature sensor feedback, heater/fan actuation, PID tuning, and thermal cycling scripts.</p></div>
 <div class="matrix-card"><h3>Validation</h3><p>Thermal profile logging, ramp-rate calculation, hold stability checks, repeatability checks, and protocol comparison.</p></div>
</div>

<div class="badge-row"><span class="badge">ESP32</span><span class="badge">Arduino</span><span class="badge">PID Control</span><span class="badge">Sensors</span><span class="badge">RT-qPCR</span><span class="badge">Automation</span></div>

## Portfolio artifacts to add

<div class="matrix">
 <div class="matrix-card"><h3>Thermal profile</h3><p>Temperature vs. time plot with setpoints, ramps, and hold stability.</p></div>
 <div class="matrix-card"><h3>Control-loop diagram</h3><p>Setpoint, controller, actuator, chamber, and sensor feedback.</p></div>
 <div class="matrix-card"><h3>Prototype summary</h3><p>Ramp rate, steady-state stability, constraints, and next design changes.</p></div>
</div>

## Engineering interpretation

This project shows automation as process engineering: define the required state trajectory, build the feedback loop, measure performance, and tune the system until the physical process follows the protocol.

## Ongoing development

Add a thermal-profile plot, describe controller tuning constraints, and include a concise bill-of-system diagram for the prototype.

<div class="case-cta-row">
 <a class="button primary" href="{{ '/projects/' | relative_url }}">View all case files</a>
 <a class="button secondary" href="{{ '/assets/files/Nathan_Anderson_Resume.pdf' | relative_url }}" download="Nathan_Anderson_Resume.pdf">Download Resume</a>
 <a class="button tertiary" href="mailto:{{ site.email }}">Contact</a>
</div>
