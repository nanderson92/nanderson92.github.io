---
layout: page
title: Stem-Cell Microencapsulation
category: Mayo Clinic · microfluidic process development
tags: Microfluidics · Process Development · Biomedical Manufacturing
subtitle: "I built a microfluidic system for making core-shell hydrogel capsules that hold stem cells, and tuned it from a fragile demo into a process that runs 20× faster with roughly half the failure rate."
---

<p class="credential-line"><strong>Affiliation:</strong> Mayo Clinic Engineering Intern · alginate-core microcapsules for encapsulation and 3D culture of ARPE-19 cells</p>

<div class="selected-outcomes micro-stats-hero">
 <div class="metric-strip stat-strip">
  <span class="stat-primary"><strong>20×</strong><em>throughput increase</em></span>
  <span class="stat-primary"><strong>~50%</strong><em>yield improvement</em></span>
  <span class="stat-primary"><strong>Lower</strong><em>coalescence frequency</em></span>
  <span class="stat-primary"><strong>QC</strong><em>microscopy workflow</em></span>
 </div>
 <p class="metric-method-note">Measurement note: throughput and yield improvements compare the tuned process to the initial low-throughput workflow after changes to flow ratios, tooling/crosslinking automation, and microscopy-supported QC.</p>
</div>

<figure class="poster-proof-card project-photo-card">
 <img src="{{ '/assets/images/nathan-anderson-poster.jpg' | relative_url }}" alt="Nathan Anderson presenting alginate-core microcapsule research at Mayo Clinic." loading="eager">
 <figcaption>Public research artifact: Mayo Clinic poster presentation on alginate-core microcapsules for encapsulation and 3D culture of ARPE-19 cells.</figcaption>
</figure>

## Summary

Developed and tuned a flow-focused microfluidic encapsulation process for core–shell hydrogel capsules, connecting flow ratio, crosslinking dwell time, and microscopy QC to capsule throughput, coalescence, and usable yield.

<div class="role-block">
 <p class="system-label small">MY ROLE</p>
 <p>Fabricated PEG/alginate core–shell microcapsules, tuned flow and crosslinking conditions, reduced coalescence, and connected microscopy observations to encapsulation yield and process stability.</p>
</div>

## Problem / motivation

Microencapsulation is valuable because hydrogel capsules can provide a controlled microenvironment while allowing transport of nutrients and metabolites. The hard part was balancing capsule complexity, throughput, uniformity, and cell compatibility without turning the process into a fragile one-off demonstration.

## Process schematic

<figure class="microfluidic-visual-card">
 <img src="{{ '/assets/images/microfluidic-flow-schematic.svg' | relative_url }}" alt="Flow-focused microencapsulation process schematic with three input streams, junction, dwell region, collection, and microscopy QC." loading="lazy">
 <figcaption>Public process schematic: streams converge, capsules form, crosslinking stabilizes the shell, and microscopy closes the QC loop.</figcaption>
</figure>

## What did not work at first

Higher throughput was not automatically better. When flow and crosslinking conditions were not matched, faster production increased coalescence and reduced the fraction of usable capsules. That pivot made the project less about “make more capsules” and more about finding the operating window where throughput and capsule quality improved together.

## Process knobs

| Knob | Mechanism | Output affected |
|---|---|---|
| Continuous/dispersed flow ratio | Shear and droplet breakup | Capsule size, throughput, coalescence |
| Crosslink dwell time | Shell formation | Stability, handling, yield |
| Collection condition | Post-formation environment | Aggregation, coalescence |
| Cell suspension handling | Biological compatibility | Viability/usefulness |

## Methods and tools

<div class="two-col">
 <div class="matrix-card"><h3>Process methods</h3><p>Flow-focused microfluidics, capsule generation, crosslinking control, flow-ratio tuning, and yield/coalescence observation.</p></div>
 <div class="matrix-card"><h3>Measurement methods</h3><p>Microscopy inspection, capsule counting, defect classification, and process-condition comparison.</p></div>
</div>

<div class="badge-row"><span class="badge">Mayo Clinic</span><span class="badge">Microfluidics</span><span class="badge">PEG/Alginate</span><span class="badge">Cell Culture</span><span class="badge">Microscopy</span><span class="badge">Process Development</span></div>

## What I’d do next

If I were building the next version, I would separate the process into two controls: one loop for capsule formation at the nozzle and one loop for post-formation stabilization. The current workflow treats collection and crosslinking as downstream handling steps, but at scale they become part of the process window.

<div class="case-cta-row">
 <a class="button primary" href="{{ '/projects/' | relative_url }}">View all projects</a>
 <a class="button secondary" href="{{ '/assets/files/Nathan_Anderson_Resume.pdf' | relative_url }}" download="Nathan_Anderson_Resume.pdf">Download Resume</a>
 <a class="button tertiary" href="mailto:{{ site.email }}">Contact</a>
</div>
