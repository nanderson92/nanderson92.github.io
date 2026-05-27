---
layout: page
title: Stem-Cell Microencapsulation
category: Microfluidics · Mayo Clinic · Rochester, MN
date_range: Summer 2025
metric_chips: '<span><strong>20×</strong> throughput increase</span><span><strong>~50%</strong> usable-yield improvement</span>'
description: Microfluidic stem-cell microencapsulation case file showing 20× throughput and ~50% usable-yield improvement through flow and tooling changes.
subtitle: Microfluidic capsule-generation work that made throughput useful by keeping yield and handling stability inside the operating window.
body_class: case-file-page
---

<section class="artifact-panel setup-snapshot">
 <h2>The setup</h2>
 <ul class="snapshot-list">
  <li><strong>System:</strong> flow-focusing microfluidic alginate-core / PEG-shell capsule generation for ARPE-19 cell culture.</li>
  <li><strong>Inputs adjusted:</strong> flow ratio, tooling geometry, shielding/crosslinking conditions, and collection workflow.</li>
  <li><strong>Measured outputs:</strong> capsule-generation rate, microscopy-counted usable yield, coalescence, shell integrity, and handling stability.</li>
  <li><strong>Result:</strong> increased capsule-generation throughput by 20× and improved microscopy-counted usable encapsulation yield by ~50% after flow-ratio, tooling, and crosslinking adjustments.</li>
 </ul>
</section>
<section class="acronym-legend">
 <strong>Notation:</strong> <span><abbr title="Critical-to-Quality">CTQ</abbr> = measurable requirement the workflow has to deliver.</span> <span><abbr title="Design of Experiments">DOE</abbr> = structured run plan.</span> <span><abbr title="Failure Mode and Effects Analysis">FMEA</abbr> = failure-mode map used to prioritize checks.</span>
</section>

<section class="artifact-stack" aria-label="Microencapsulation artifacts">
 <article class="artifact-card artifact-card-hero">
  <span class="artifact-label">Microscopy · Figure 1</span>
  <div class="artifact-image-wrap microscopy-wrap"><img class="artifact-image" src="{{ '/assets/images/artifacts/microcapsule-microscopy.jpg' | relative_url }}" alt="Representative hydrogel microcapsules from microfluidic encapsulation workflow" loading="lazy"></div>
  <p class="artifact-caption"><strong>Figure 1. Representative hydrogel microcapsules from the microfluidic encapsulation workflow.</strong> This image shows real capsule morphology, visual process output, and the type of microscopy evidence used for yield/quality assessment.</p>
  <p class="artifact-limitation"><strong>Publication cleanup:</strong> Add final scale bar, condition, flow rate, CaCl₂ concentration, and run ID before public publication if not already embedded.</p>
 </article>
 <div class="artifact-grid two-col-artifacts">
  <article class="artifact-card">
   <span class="artifact-label">Quantitative artifact · Figure 2</span>
   <div class="artifact-image-wrap chart-wrap"><img class="artifact-image" src="{{ '/assets/images/artifacts/peg-shell-thickness-flowrate.png' | relative_url }}" alt="PEG shell thickness versus shell flow rate chart" loading="lazy"></div>
   <p class="artifact-caption"><strong>Figure 2. PEG shell thickness as a function of shell flow rate.</strong> Use this chart as quantitative evidence that process inputs shift capsule structure, but revise the final version with n, error-bar definition, p-value threshold, and clear legend labels.</p>
  </article>
  <article class="artifact-card">
   <span class="artifact-label">Mechanism schematic · Figure 3</span>
   <div class="artifact-image-wrap schematic-wrap"><img class="artifact-image" src="{{ '/assets/images/artifacts/alginate-hardening-concept.png' | relative_url }}" alt="Alginate core hardening concept schematic" loading="lazy"></div>
   <p class="artifact-caption"><strong>Figure 3. Alginate-core hardening concept.</strong> Calcium-mediated crosslinking converts a liquid alginate core into a mechanically stabilized hydrogel core.</p>
  </article>
 </div>
 <article class="artifact-card">
  <span class="artifact-label">Site-native process schematic</span>
  <div class="artifact-image-wrap schematic-wrap"><img class="artifact-image" src="{{ '/assets/images/artifacts/microencapsulation-flow-native.svg' | relative_url }}" alt="Site-native schematic of microfluidic encapsulation streams" loading="lazy"></div>
  <p class="artifact-caption"><strong>Microfluidic encapsulation flow logic.</strong> Recreated as a site-native schematic instead of embedding an ownership-unclear reference image. It shows core, shell, oil, and crosslinker inputs as process levers for capsule formation.</p>
 </article>
</section>

<section class="insight-block tone-dark"><p>Faster capsule generation was only useful when flow ratio, droplet formation, crosslink timing, and collection stayed inside a usable operating window.</p></section>

<section class="mini-flow-card"><h2>Capsule workflow</h2><div class="mini-flow"><span>Set flow ratio</span><b>→</b><span>Generate capsules</span><b>→</b><span>Crosslink</span><b>→</b><span>Microscopy QC</span><b>→</b><span>Classify usable yield</span></div></section>

## What I'd do next

<div class="next-iteration-callout">
 <p>The next iteration should convert yield categories into a simple control plan: acceptable capsule morphology, coalescence limit, collection timing, and microscopy sampling cadence. The engineering decision is whether a faster run stays inside the usable-yield window without hiding new defect classes.</p>
</div>

## Before / after metric table

<div class="artifact-table-wrap"><table class="artifact-table"><thead><tr><th>Metric</th><th>Baseline</th><th>Improved</th><th>Decision use</th></tr></thead><tbody>
<tr><td>Capsule generation rate</td><td>to be filled</td><td>20× baseline</td><td>Shows whether tooling and flow changes made the workflow meaningfully faster.</td></tr>
<tr><td>Usable yield</td><td>to be filled</td><td>~50% relative improvement</td><td>Checks that speed did not hide unacceptable morphology or handling failures.</td></tr>
<tr><td>Main process levers</td><td>flow ratio, tooling, crosslinking, handling/QC</td><td>flow ratio, tooling, crosslinking, handling/QC</td><td>Defines which inputs belong in the next control plan.</td></tr>
<tr><td>Defect classes</td><td>coalesced, unstable, malformed, handling-damaged</td><td>coalesced, unstable, malformed, handling-damaged</td><td>Keeps the throughput claim tied to usable capsules instead of total capsules.</td></tr>
</tbody></table></div>

## Process levers

<div class="artifact-table-wrap"><table class="artifact-table"><thead><tr><th>Process change</th><th>Failure mode addressed</th><th>Metric affected</th><th>Result</th></tr></thead><tbody>
<tr><td>Flow-ratio tuning</td><td>Unstable capsule formation / coalescence</td><td>Usable yield</td><td>~50% improvement</td></tr>
<tr><td>Tooling redesign</td><td>Low generation rate</td><td>Throughput</td><td>20× increase</td></tr>
<tr><td>Crosslink timing adjustment</td><td>Fragile shells / post-formation instability</td><td>Handling stability</td><td>Improved usable capsule fraction</td></tr>
<tr><td>Microscopy QC</td><td>Unclassified defects</td><td>Yield interpretation</td><td>Defect classes became visible</td></tr>
</tbody></table></div>
<p class="method-note"><strong>Yield definition:</strong> percent usable capsules after excluding coalesced, visibly defective, or handling-unstable capsules during microscopy QC.</p>

## The insight

Faster throughput was not automatically better. Speed only mattered when flow ratio, droplet formation, crosslink timing, and collection conditions stayed inside a usable operating window.

## What this shifted

<div class="what-changed-block changed-panel">
 <p>The project moved from trying to make capsules faster to defining which flow and crosslinking conditions made faster capsule generation usable.</p>
</div>

<div class="case-cta-row two-button-cta">
 <a class="button primary" href="{{ '/projects/printed-interconnect-reliability/' | relative_url }}">Next: Printed Interconnect Reliability →</a>
 <a class="button secondary email-button" href="mailto:{{ site.email }}">Email Nathan</a>
</div>
