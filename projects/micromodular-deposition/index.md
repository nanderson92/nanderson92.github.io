---
layout: page
title: Micromodular Electronics Deposition
category: Edge crowding → interconnect-accessible placement
date_range: 2025–present
affiliation: Filler Lab, Georgia Institute of Technology
tags: Semiconductors · Process Development · Interfacial Transport · Automation & Data
subtitle: "Substrate/backing screening for IPA droplet deposition of suspended microdevices before downstream printed interconnect routing."
---

<figure class="flagship-page-visual">
 <img src="{{ '/assets/images/micromodular-workflow-deposition-focus.png' | relative_url }}" alt="Micromodular electronics workflow with the deposition subsystem highlighted." loading="eager">
 <figcaption>System view: deposition sits between fabricated components and printable circuit assembly. If placement is unusable, the downstream wiring problem gets harder.</figcaption>
</figure>

<div class="thesis-box promoted-thesis-box">
 <h2>Useful placement is a process variable, not a final-photo aesthetic.</h2>
 <p>I built the screening workflow for identifying substrate/backing conditions that reduce edge crowding while preserving interconnect-accessible placement.</p>
</div>

<blockquote class="ownership-callout">I designed the experiments from scratch: chose the substrates, set up both top-view and side-view video capture, wrote the Python/OpenCV and ImageJ pipelines to extract contact-line metrics, and used those metrics to identify which substrate/backing conditions produce useful placement.</blockquote>

<section class="artifact-panel public-safe-snapshot" aria-label="Public-safe experiment snapshot">
 <h2>Public-safe experiment snapshot</h2>
 <ul class="snapshot-list">
  <li><strong>System:</strong> IPA droplet deposition of suspended microdevices on substrate/backing candidates.</li>
  <li><strong>Inputs varied:</strong> substrate, backing condition, droplet volume, particle/device loading state.</li>
  <li><strong>Metrics extracted:</strong> r(t)/r₀, contact-line regime, edge/center device ratio, qualitative repeatability, final deposition pattern.</li>
  <li><strong>Current decision:</strong> prioritize porous AAO-like drainage conditions over glass-like evaporation controls.</li>
  <li><strong>Next threshold needed:</strong> replicate-backed edge/center ratio and density-uniformity target before interconnect printing.</li>
 </ul>
</section>

## Why this matters

Suspended microdevices can raft, crowd, pin near the contact line, and accumulate nonuniformly as the carrier liquid spreads, evaporates, and/or imbibes into the substrate. The practical question is not “which surface looks clean?” It is: **which substrate/backing state leaves enough devices in wireable positions after the liquid exits?**

The working answer is that porous AAO-like drainage behavior is more promising than glass-like low-uptake behavior. That decision is based on video-derived contact-line history and final placement metrics rather than final stain appearance alone.

## Defining useful placement

<div class="artifact-table-wrap">
<table class="artifact-table">
<thead><tr><th>Criterion</th><th>Operational definition</th><th>Why it matters downstream</th></tr></thead>
<tbody>
<tr><td>Lower edge crowding</td><td>Reduced concentration of devices at the outer ring relative to the field.</td><td>Prevents routing from becoming an edge-only wiring problem.</td></tr>
<tr><td>Better center/field distribution</td><td>More usable devices away from the contact-line perimeter.</td><td>Creates more candidate sites for printed interconnects.</td></tr>
<tr><td>Interconnect-accessible density</td><td>High enough local device density without rafted or overlapped clusters.</td><td>Maintains enough targets while preserving line-of-sight for Ag nanoparticle interconnects.</td></tr>
<tr><td>Repeatable final pattern</td><td>Similar deposit morphology across replicate droplets under the same condition.</td><td>Separates process behavior from a one-off visual result.</td></tr>
<tr><td>Scale-compatible surface</td><td>Substrate or coating can plausibly move beyond brittle AAO-only handling.</td><td>Turns a lab observation into a manufacturing candidate.</td></tr>
</tbody>
</table>
</div>

## Process map

<div class="process-map central-process-map" aria-label="Process input to engineering decision map">
 <div class="process-map-stage"><p>INPUTS</p><span>droplet volume</span><span>solvent</span><span>device loading</span><span>substrate</span><span>backing layer</span></div>
 <div class="process-map-arrow" aria-hidden="true">→</div>
 <div class="process-map-stage"><p>TRANSPORT</p><span>spreading</span><span>imbibition</span><span>evaporation</span><span>pinning</span><span>rafting/crowding</span></div>
 <div class="process-map-arrow" aria-hidden="true">→</div>
 <div class="process-map-stage"><p>CTQs</p><span>r(t)/r₀</span><span>θ(t)</span><span>edge/center ratio</span><span>density map</span><span>repeatability</span></div>
 <div class="process-map-arrow" aria-hidden="true">→</div>
 <div class="process-map-stage decision-stage"><p>DECISION</p><span>accept / reject / redesign candidate surface</span></div>
</div>

## Decision framework

<div class="decision-grid">
 <article class="decision-card pass-card">
  <h3>Candidate passes early screen if</h3>
  <ol>
   <li>Contact-line history can be classified from video, not inferred only from final stain.</li>
   <li>Edge/center device ratio improves relative to glass-like evaporation control.</li>
   <li>Device density remains high enough for downstream interconnect routing.</li>
   <li>Pattern is repeatable across replicate droplets.</li>
   <li>Substrate/backing condition is physically scalable beyond brittle AAO.</li>
  </ol>
 </article>
 <article class="decision-card fail-card">
  <h3>Candidate fails if</h3>
  <ul>
   <li>Fast liquid removal still creates edge-heavy crowding.</li>
   <li>Droplet footprint becomes too small or irregular for routing.</li>
   <li>Device rafts or pins unpredictably.</li>
   <li>Metric extraction cannot distinguish mechanism from artifact.</li>
  </ul>
 </article>
</div>

## My role

<div class="artifact-table-wrap">
<table class="artifact-table role-table">
<thead><tr><th>Area</th><th>Contribution</th></tr></thead>
<tbody>
<tr><td>Experimental design</td><td>Substrate/backing comparisons, droplet setup, substrate preparation, primer/film application, and run-to-run comparison.</td></tr>
<tr><td>Imaging</td><td>Top-view and side-view capture; microscopy-based process observation.</td></tr>
<tr><td>Analysis</td><td>Python/OpenCV and ImageJ extraction of contact-line, microdevice velocity, acceleration, radial drift, and deposition metrics.</td></tr>
<tr><td>Decision output</td><td>Screening logic for substrate candidates before interconnect printing.</td></tr>
</tbody>
</table>
</div>

## Process knobs

| Knob | Why it matters | What I varied / compared |
|---|---|---|
| Substrate porosity / permeability | Controls liquid uptake and vertical drain rate. | Porous membranes versus low-uptake controls. |
| Backing condition | Changes whether the porous substrate behaves like a drain, membrane, or supported surface. | Glass, air gap, absorbent backing, and support conditions. |
| Contact angle / wetting | Sets footprint size, spreading dynamics, and transport length scale. | Contact-line behavior across substrate/backing states. |
| Contact-line pinning | Influences ring accumulation and edge crowding. | Pinned, receding, and mixed regimes from video. |
| Evaporation vs. imbibition | Determines whether flow is dominated by drying or liquid uptake. | Glass-like evaporation baseline versus porous uptake behavior. |
| Device loading | Affects crowding, raft interactions, and useful areal density. | Qualitative loading/crowding state during deposition. |

## Measurement pipeline

<div class="process-map compact-flow-map measurement-pipeline-map" aria-label="Image analysis workflow schematic">
 <div class="process-map-stage"><p>VIDEO</p><span>top view</span><span>side view</span></div>
 <div class="process-map-arrow" aria-hidden="true">→</div>
 <div class="process-map-stage"><p>SEGMENT</p><span>droplet edge</span><span>device field</span></div>
 <div class="process-map-arrow" aria-hidden="true">→</div>
 <div class="process-map-stage"><p>CALIBRATE</p><span>pixel scale</span><span>frame timing</span></div>
 <div class="process-map-arrow" aria-hidden="true">→</div>
 <div class="process-map-stage decision-stage"><p>OUTPUTS</p><span>r(t), density, edge/center ratio, microdevice radial drift</span></div>
</div>

## Methods and tools

<div class="two-col">
 <div class="matrix-card"><h3>Experimental methods</h3><p>Sessile droplet deposition, AAO/substrate comparisons, backing-layer studies, optical microscopy, top-view videos, side-view videos, and process observation.</p></div>
 <div class="matrix-card"><h3>Analysis methods</h3><p>Droplet-radius extraction, contact-line tracking, deposition-pattern quantification, radial density maps, edge/center ratio, DOE / response-surface planning, and statistical comparison.</p></div>
</div>

<div class="badge-row">
 <span class="badge">Keyence</span><span class="badge">Rame-Hart</span><span class="badge">Python/OpenCV</span><span class="badge">ImageJ/Fiji</span><span class="badge">JMP</span><span class="badge">Optical Microscopy</span>
</div>

## Public-safe outputs

<div class="text-output-grid">
 <article><h3>Contact-line dynamics</h3><p><strong>Metric:</strong> normalized radius, r(t)/r₀. <strong>Use:</strong> separates spreading, pinning, recession, and substrate drainage behavior.</p></article>
 <article><h3>Deposition uniformity</h3><p><strong>Metric:</strong> edge/center ratio. <strong>Use:</strong> compares edge crowding against useful central-device placement.</p></article>
 <article><h3>Substrate decision</h3><p><strong>Metric set:</strong> liquid removal behavior, contact-line behavior, deposition output, and repeatability. <strong>Use:</strong> screen substrate/backing combinations before printing interconnects.</p></article>
</div>

<div class="placeholder-figure-grid deposition-output-grid">
 <figure class="data-placeholder-figure wide-placeholder">
  <img src="{{ '/assets/images/placeholder-deposition-comparison.svg' | relative_url }}" alt="Substrate/backing deposition microscopy comparison panel." loading="lazy">
  <figcaption>Substrate/backing comparison panel for microscopy outputs, condition labels, and replicate organization.</figcaption>
 </figure>
 <figure class="data-placeholder-figure">
  <img src="{{ '/assets/images/placeholder-radius-trace.svg' | relative_url }}" alt="Normalized r(t)/r0 contact-line trace panel." loading="lazy">
  <figcaption>Contact-line dynamics across substrate/backing conditions.</figcaption>
 </figure>
 <figure class="data-placeholder-figure">
  <img src="{{ '/assets/images/placeholder-edge-center-ratio.svg' | relative_url }}" alt="Edge-to-center deposition ratio comparison panel." loading="lazy">
  <figcaption>Edge/center ratio comparison across substrate/backing conditions.</figcaption>
 </figure>
</div>

<div class="what-changed-block">
 <h2>What changed because of this</h2>
 <p>This work shifted the project from judging substrates by final visual stains to screening them by video-derived contact-line behavior, drainage/evaporation signatures, and placement metrics tied to downstream interconnect feasibility.</p>
</div>

## What I’d do next

If I were moving this toward a production screen, I would automate the video-to-metric pipeline first. The bottleneck is not only the droplet experiment; it is making the same measurement fast enough that substrate candidates can be compared before the process drifts. The next engineering gate is a replicate-backed edge/center ratio and density-uniformity threshold that predicts whether Ag nanoparticle interconnect routing remains practical.

<div class="case-cta-row">
 <a class="button primary" href="{{ '/projects/printed-interconnect-reliability/' | relative_url }}">Related reliability case →</a>
 <a class="button secondary" href="{{ '/assets/files/Nathan_Anderson_Resume.pdf' | relative_url }}" download="Nathan_Anderson_Resume.pdf">Download Resume</a>
 <a class="button tertiary" href="mailto:{{ site.email }}">Contact</a>
</div>
