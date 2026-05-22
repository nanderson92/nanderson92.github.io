---
layout: page
title: Printed Interconnect & FET Reliability
category: Flagship Case Study
tags: Semiconductors · Reliability · Process Control · Manufacturing
subtitle: Electrical test, resistance drift, yield visibility, and process-control loops for micromodular electronics.
---

## Summary

This case file focuses on reliability and process control for printed interconnects and device test structures in a micromodular electronics workflow. The project turns electrical measurements into manufacturing decisions: what is stable, what is drifting, what fails, and which process step likely caused it.

<div class="buildout-note">Case study buildout in progress — public-safe plots, simplified device schematics, and threshold logic will be added as artifacts.</div>

<div class="role-block">
  <p class="system-label small">MY ROLE</p>
  <p>Built and used electrical screening workflows, organized resistance/failure data, interpreted stress-response behavior, correlated failures to surface-prep/deposition/cure steps, and framed the results as CTQs, acceptance limits, and process-window feedback.</p>
</div>

## Problem / motivation

Printed interconnects can look acceptable initially but fail later through resistance drift, intermittent opens, weak contacts, surface-prep defects, or stress-induced degradation. A useful manufacturing process needs more than a one-time “works / does not work” check; it needs a measurement loop that makes yield and failure modes visible.

## Micromodular electronics roadmap

This figure shows where the reliability and interconnect work fits inside the overall micromodular electronics workflow. The highlighted subsystem covers the circuit-assembly side of the process: printing around deposited devices, planning the wiring path, and validating whether the printed interconnect network stays electrically stable.

<figure class="roadmap-figure">
  <img src="{{ '/assets/images/micromodular-roadmap-interconnect.svg' | relative_url }}" alt="High-level micromodular electronics roadmap with the interconnect subsystem highlighted." />
  <figcaption>High-level manufacturing roadmap. This project focuses on the interconnect subsystem: component printing, wiring strategy, and printed-wire reliability.</figcaption>
</figure>

## Engineering framing

<div class="matrix">
  <div class="matrix-card"><h3>Process variables</h3><p>Surface preparation, primer/film chemistry, deposition conditions, curing history, geometry, and handling.</p></div>
  <div class="matrix-card"><h3>Measured signals</h3><p>Initial resistance, drift, intermittent opens, pass/fail yield, stress response, and device-to-device variation.</p></div>
  <div class="matrix-card"><h3>Control response</h3><p>Acceptance thresholds, rework rules, failure-mode notes, and process-window adjustments.</p></div>
</div>

## Variables studied

| Variable | Why it matters |
|---|---|
| Initial resistance | Baseline for drift, failure, and coupon-to-coupon variation. |
| Resistance drift | Indicates degradation, unstable interfaces, or weak process control. |
| Intermittent opens | Suggests contact, cracking, adhesion, or handling-related failure. |
| Temperature / humidity stress | Accelerates reliability issues and reveals process weaknesses. |
| Surface-prep and cure history | Often determines contact quality and conductivity stability. |
| Threshold / compliance limits | Converts measurement into a go/no-go manufacturing decision. |

## Methods and tools

<div class="two-col">
  <div class="matrix-card"><h3>Experimental methods</h3><p>Electrical probing, resistance tracking, stress-condition comparison, pass/fail screening, and failure interval framing.</p></div>
  <div class="matrix-card"><h3>Data methods</h3><p>Automated logging, summary statistics, JMP comparisons, drift plots, threshold logic, and process-step correlation.</p></div>
</div>

<div class="badge-row">
  <span class="badge">Keithley</span>
  <span class="badge">Python</span>
  <span class="badge">JMP</span>
  <span class="badge">Excel</span>
  <span class="badge">Reliability</span>
  <span class="badge">CTQs</span>
</div>

## Outputs to add

<div class="matrix">
  <div class="matrix-card"><h3>Resistance vs. time</h3><p>Public-safe plot showing drift, stabilization, or failure behavior.</p></div>
  <div class="matrix-card"><h3>Go/no-go screen</h3><p>Threshold logic for turning raw readings into pass/fail and rework decisions.</p></div>
  <div class="matrix-card"><h3>Process-control loop</h3><p>Diagram linking electrical signatures back to surface prep, deposition, cure, and handling steps.</p></div>
</div>

## Engineering interpretation

The value of this project is not just plotting resistance. It is building a feedback loop: measure the electrical output, classify the failure mode, identify likely process causes, then tighten the process window.

## Manufacturing relevance

This is the language of process engineering inside semiconductor-adjacent R&amp;D: CTQs, screening, yield visibility, reliability, acceptance limits, failure mechanisms, and standardization.

## Next steps

Add a public-safe resistance drift plot, define failure/drift thresholds, and include one simplified process-control diagram that shows how test data feeds back into process changes.
