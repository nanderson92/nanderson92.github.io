---
layout: page
title: Process Simulation and Design
category: Process Engineering Case File
subtitle: Flowsheets, balances, thermodynamic reasoning, and simulation-based design decisions.
---

## Summary

This case file collects process-engineering work where a chemical process is converted from a description into a defensible flowsheet, balance structure, and operating decision.

## Problem / motivation

Process design work can look abstract until the assumptions are visible. A credible design needs a process flow diagram, stated thermodynamic reasoning, material and energy balances, and a clear explanation of tradeoffs such as recovery, purity, energy demand, and equipment constraints.

## System schematic

<div class="project-schematic schematic-pfd" aria-label="Representative process flow diagram schematic">
  <div class="pfd-row"><span>FEED</span><i></i><span>MIX</span><i></i><span>SEPARATE</span><i></i><span>PRODUCT</span></div>
  <p>Representative PFD logic for making assumptions, streams, unit operations, and design decisions visible.</p>
</div>

## My role

<div class="role-block">
  <p>Built balance logic, selected appropriate modeling assumptions, organized process inputs/outputs, and translated calculations into design tradeoff summaries.</p>
</div>

## Technical challenge

The core challenge is converting a process objective into quantitative design logic without overclaiming model precision. The project emphasizes balance closure, transparent assumptions, and simulation results that support engineering decisions rather than black-box outputs.

## Variables studied

| Variable | Why it matters |
|---|---|
| Feed composition | Sets material balance basis and separation difficulty. |
| Operating temperature / pressure | Affects phase behavior, energy duty, and equipment feasibility. |
| Recovery / purity targets | Define whether a process alternative is technically acceptable. |
| Recycle or purge logic | Controls yield, accumulation, and steady-state feasibility. |
| Thermodynamic model | Determines whether VLE/separation predictions are physically reasonable. |

## Public artifact set

<div class="matrix">
  <div class="matrix-card"><h3>Process flow diagram</h3><p>Clean PFD with numbered streams and unit-operation logic.</p></div>
  <div class="matrix-card"><h3>Balance table</h3><p>Feed/product/recycle streams with units, assumptions, and closure checks.</p></div>
  <div class="matrix-card"><h3>Design tradeoff summary</h3><p>Short explanation of how operating conditions affect feasibility and performance.</p></div>
</div>

## Methods and tools

<div class="two-col">
  <div class="matrix-card"><h3>Engineering methods</h3><p>PFD construction, material balances, energy balances, thermodynamic reasoning, sensitivity comparisons, and process tradeoff tables.</p></div>
  <div class="matrix-card"><h3>Software / computation</h3><p>Aspen simulations, MATLAB calculations, Excel screening tables, and communication-ready engineering plots.</p></div>
</div>

<div class="badge-row"><span class="badge">Aspen</span><span class="badge">PFDs</span><span class="badge">Balances</span><span class="badge">MATLAB</span><span class="badge">Excel</span></div>

## Engineering interpretation

The value of this project is the ability to make process assumptions visible and turn calculations into clear decisions. That is the core skill behind scale-up, process development, and manufacturing support.

<div class="case-cta-row">
 <a class="button primary" href="{{ '/projects/' | relative_url }}">View all case files</a>
 <a class="button secondary" href="{{ '/assets/files/Nathan_Anderson_Resume.pdf' | relative_url }}" download="Nathan_Anderson_Resume.pdf">Download Resume</a>
 <a class="button tertiary" href="mailto:nanderson92@gatech.edu">Contact</a>
</div>
