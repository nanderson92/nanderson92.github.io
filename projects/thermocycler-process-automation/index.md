---
layout: page
title: Thermocycler Process Automation
category: Supporting Case File
tags: Automation · Controls · Diagnostics · Hardware
subtitle: PID-controlled thermal cycling hardware for rapid molecular-diagnostics workflows.
---

## Summary

This case file presents a thermocycler automation project focused on building repeatable thermal control for RT-qPCR-style workflows. The engineering challenge is turning a biological protocol into a controllable temperature-time process.

<div class="role-block">
 <p class="system-label small">MY ROLE</p>
 <p>Prototyped an embedded-controller thermocycler, integrated heating/cooling and sensor feedback, tuned PID behavior, and evaluated ramp rate, overshoot, settling time, and steady-state temperature stability.</p>
</div>

<div class="connection-note"><strong>Connection to flagship:</strong> This project extends the same measurement-to-control mindset into automation: define the controlled variable, measure dynamic response, tune the system, and quantify repeatability.</div>

## Problem / motivation

PCR thermal cycling depends on repeatable heating and cooling between temperature setpoints. Poor thermal control creates inconsistent amplification conditions, slower workflows, and unreliable diagnostic performance.

## Representative control artifact

<div class="thermal-artifact proof-artifact-card" aria-label="Temperature versus time profile for thermocycler control">
 <div>
  <p class="system-label small">CONTROL PERFORMANCE VIEW</p>
  <h3>Setpoint tracking and thermal lag</h3>
  <p>The representative setpoint-vs-time plot emphasizes the engineering constraints that separate a prototype from a controlled thermal process: sensor placement, ramp-rate limits, overshoot/undershoot, settling time, hold stability, and repeatability across cycles.</p>
 </div>
 <div class="thermal-plot" aria-label="Representative thermal profile with setpoint and measured temperature">
  <span class="plot-axis y">temperature</span>
  <span class="plot-axis x">time</span>
  <b class="setpoint-line"></b>
  <b class="measured-line"></b>
  <em class="annot ramp">ramp rate</em>
  <em class="annot overshoot">overshoot</em>
  <em class="annot hold">hold stability</em>
 </div>
</div>

<div class="hardware-interface-card proof-artifact-card" aria-label="Representative thermocycler hardware interface map">
 <div>
  <p class="system-label small">HARDWARE INTERFACE VIEW</p>
  <h3>Controller → actuator → thermal mass → sensor</h3>
  <p>A representative hardware map makes the control problem concrete: the controller changes actuator output, the thermal block responds with lag, and the sensor closes the loop with imperfect knowledge of actual sample temperature.</p>
 </div>
 <div class="hardware-map" aria-label="Embedded controller thermocycler interface diagram">
  <span>ESP32 / Arduino</span><i></i><span>heater + fan</span><i></i><span>thermal block</span><i></i><span>temperature sensor</span>
 </div>
</div>

## Control-loop schematic

<div class="process-map control-loop-map" aria-label="Representative PID thermal control schematic">
 <div class="process-map-stage"><p>SETPOINT</p><span>denaturation</span><span>annealing</span><span>extension</span></div>
 <div class="process-map-arrow" aria-hidden="true">→</div>
 <div class="process-map-stage"><p>PID</p><span>error</span><span>gain tuning</span></div>
 <div class="process-map-arrow" aria-hidden="true">→</div>
 <div class="process-map-stage"><p>ACTUATION</p><span>heater</span><span>cooling fan</span></div>
 <div class="process-map-arrow" aria-hidden="true">→</div>
 <div class="process-map-stage decision-stage"><p>FEEDBACK</p><span>sensor signal vs. sample temperature estimate</span></div>
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

## Engineering interpretation

This project shows automation as process engineering: define the required state trajectory, build the feedback loop, measure performance, and tune the system until the physical process follows the protocol.

<div class="case-cta-row">
 <a class="button primary" href="{{ '/projects/' | relative_url }}">View all case files</a>
 <a class="button secondary" href="{{ '/assets/files/Nathan_Anderson_Resume.pdf' | relative_url }}" download="Nathan_Anderson_Resume.pdf">Download Resume</a>
 <a class="button tertiary" href="mailto:{{ site.email }}">Contact</a>
</div>
