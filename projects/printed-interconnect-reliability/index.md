---
layout: page
title: Printed Interconnect & FET Reliability
category: Supporting Case File
tags: Semiconductors · Reliability · Process Control · Manufacturing
subtitle: Turning electrical drift and pass/fail behavior into process-control feedback for printed micromodular circuits.
---

## Summary

This case file focuses on reliability and process control for printed interconnects and device test structures in a micromodular electronics workflow. The project turns electrical measurements into manufacturing decisions: what is stable, what is drifting, what fails, and which process step likely caused it.

<div class="role-block">
 <p class="system-label small">MY ROLE</p>
 <p>Built and used electrical screening workflows, organized resistance/failure data, interpreted stress-response behavior, correlated failures to surface-prep/deposition/cure steps, and framed the results as CTQs, acceptance limits, and process-window feedback.</p>
</div>

<div class="connection-note"><strong>Connection to flagship:</strong> The deposition project asks where devices land. This reliability project asks whether the printed interconnects and device interfaces remain electrically usable after assembly.</div>

## Problem / motivation

Printed interconnects can look acceptable initially but fail later through resistance drift, intermittent opens, weak contacts, surface-prep defects, or stress-induced degradation. A useful manufacturing process needs more than a one-time “works / does not work” check; it needs a measurement loop that makes yield and failure modes visible.

## Where this project fits in the workflow

<figure class="wide-figure">
 <img src="{{ '/assets/images/micromodular-workflow-interconnect-focus.png' | relative_url }}" alt="High-level micromodular electronics workflow with the interconnect subsystem highlighted across analyzing components, planning wiring, and printing wires." loading="lazy">
 <figcaption><strong>Micromodular electronics workflow.</strong> The rounded rectangle highlights the interconnect subsystem: analyzing printed component layouts, planning wiring paths, and printing the interconnects that turn placed components into working circuits.</figcaption>
</figure>

## Representative reliability artifact

<div class="reliability-artifact proof-artifact-card" aria-label="Representative resistance drift and go/no-go threshold artifact">
 <div>
  <p class="system-label small">PUBLIC ARTIFACT FORMAT</p>
  <h3>Resistance drift → threshold decision</h3>
  <p>A sanitized resistance-trace format communicates how raw electrical measurements become process-control feedback.</p>
  <ul>
   <li><strong>Initial R below limit:</strong> pass screen.</li>
   <li><strong>Drift above threshold:</strong> monitor or fail.</li>
   <li><strong>Open circuit:</strong> fail.</li>
   <li><strong>Intermittent behavior:</strong> handling/contact failure candidate.</li>
  </ul>
 </div>
 <div class="resistance-plot" aria-label="Representative resistance versus time plot with thresholds">
  <span class="plot-axis y">R/R₀</span>
  <span class="plot-axis x">stress interval</span>
  <i class="threshold fail"></i>
  <i class="threshold warn"></i>
  <b class="trace stable"></b>
  <b class="trace drift"></b>
  <b class="trace failtrace"></b>
  <em class="label pass">pass</em>
  <em class="label drift-label">drift</em>
  <em class="label fail-label">fail</em>
 </div>
</div>

## Process-control loop

<div class="process-map reliability-loop" aria-label="Printed interconnect reliability process-control loop">
 <div class="process-map-stage"><p>FABRICATE</p><span>surface prep</span><span>print</span><span>cure</span></div>
 <div class="process-map-arrow" aria-hidden="true">→</div>
 <div class="process-map-stage"><p>MEASURE</p><span>initial R</span><span>stress interval</span><span>R drift</span></div>
 <div class="process-map-arrow" aria-hidden="true">→</div>
 <div class="process-map-stage"><p>CLASSIFY</p><span>pass</span><span>drift</span><span>open</span><span>intermittent</span></div>
 <div class="process-map-arrow" aria-hidden="true">→</div>
 <div class="process-map-stage decision-stage"><p>ADJUST</p><span>surface prep / deposition / cure / handling</span></div>
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

## Engineering interpretation

The value of this project is not just plotting resistance. It is building a feedback loop: measure the electrical output, classify the failure mode, identify likely process causes, then tighten the process window.

## Manufacturing relevance

Two CTQs make the reliability loop actionable: initial resistance must pass the first screen, and resistance drift must stay below the chosen failure threshold after stress. Those two outputs turn electrical testing into a process-control signal rather than a one-time pass/fail check.

<div class="case-cta-row">
 <a class="button primary" href="{{ '/projects/micromodular-deposition/' | relative_url }}">Related deposition case file →</a>
 <a class="button secondary" href="{{ '/assets/files/Nathan_Anderson_Resume.pdf' | relative_url }}" download="Nathan_Anderson_Resume.pdf">Download Resume</a>
 <a class="button tertiary" href="mailto:{{ site.email }}">Contact</a>
</div>
