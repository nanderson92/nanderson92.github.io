---
layout: page
title: Micromodular Electronics Deposition
category: Filler Lab · Georgia Tech · edge crowding → useful placement
tags: Semiconductors · Process Development · Interfacial Transport · Automation & Data
subtitle: "When you print microdevices from a droplet, they crowd at the edges and land in useless patterns. I spent a year figuring out which substrate conditions actually fix that."
---

<p class="credential-line"><strong>Affiliation:</strong> Filler Lab, Georgia Tech · Micromodular printed electronics</p>

<figure class="flagship-page-visual">
 <img src="{{ '/assets/images/micromodular-workflow-deposition-focus.png' | relative_url }}" alt="Micromodular electronics workflow with the deposition subsystem highlighted." loading="eager">
 <figcaption>System view: deposition sits between fabricated components and printable circuit assembly. If placement is useless, the downstream wiring problem gets harder.</figcaption>
</figure>

<div class="thesis-box promoted-thesis-box">
 <h2>If the substrate controls how liquid leaves the droplet, it controls where devices end up.</h2>
 <p>The hard part was separating surface wetting, porous drainage, evaporation, and contact-line pinning instead of treating the final stain pattern as the whole story.</p>
</div>

<div class="role-block flagship-role-block emphasis-role-block">
 <p>I designed the experiments from scratch: chose the substrates, set up both top-view and side-view video capture, wrote the Python and ImageJ pipelines to extract contact-line metrics, and used those metrics to figure out which boundary conditions actually produce useful placement.</p>
 <p><strong>Core output:</strong> a substrate-screening decision framework the lab can use to evaluate new deposition surfaces before committing to downstream interconnect printing.</p>
</div>

## Why this matters

Suspended microdevices can raft, crowd, pin near the contact line, and accumulate nonuniformly as the carrier liquid spreads, evaporates, and/or imbibes into the substrate.

The practical question is simple: **which boundary condition leaves devices in places that can still be wired later?**

The working answer is that porous AAO-like surfaces with controlled drainage/backing behavior are more promising than glass-like low-uptake controls. They shorten the late-stage edge-sweep problem and give the lab a surface condition worth screening before interconnect printing. The exact substrate/coating decision still depends on replicate images and edge/center metrics, which is why the measurement pipeline matters.

## Process map

<div class="process-map central-process-map" aria-label="Process input to engineering decision map">
 <div class="process-map-stage">
 <p>INPUTS</p>
 <span>Droplet volume</span>
 <span>Solvent</span>
 <span>Device loading</span>
 <span>Substrate</span>
 <span>Backing layer</span>
 </div>
 <div class="process-map-arrow" aria-hidden="true">→</div>
 <div class="process-map-stage">
 <p>TRANSPORT</p>
 <span>Spreading</span>
 <span>Imbibition</span>
 <span>Evaporation</span>
 <span>Pinning</span>
 <span>Rafting/crowding</span>
 </div>
 <div class="process-map-arrow" aria-hidden="true">→</div>
 <div class="process-map-stage">
 <p>METRICS</p>
 <span>r(t)/r₀</span>
 <span>θ(t)</span>
 <span>Edge/center ratio</span>
 <span>Density map</span>
 <span>Repeatability</span>
 </div>
 <div class="process-map-arrow" aria-hidden="true">→</div>
 <div class="process-map-stage decision-stage">
 <p>DECISION</p>
 <span>Accept / reject / redesign substrate boundary condition.</span>
 </div>
</div>

## Why this is hard

<div class="editorial-hard-list text-only-hard-list">
 <p><strong>Coupled liquid removal.</strong> Evaporation and imbibition compete, so the final deposit does not reveal the full transport history.</p>
 <p><strong>Contact-line memory.</strong> A pinned, receding, or mixed contact line can write different device distributions even with similar final footprints.</p>
 <p><strong>Device interactions.</strong> Microdevices raft, rotate, crowd, and block each other near the edge, which makes particle-like intuition incomplete.</p>
 <p><strong>Measurement burden.</strong> The useful output is not one pretty image. It is a repeatable metric set that compares substrate/backing conditions.</p>
</div>

## Process knobs

| Knob | Why it matters | What I varied / compared |
|---|---|---|
| Substrate porosity / permeability | Controls liquid uptake and vertical drain rate. | Porous membranes versus low-uptake controls. |
| Backing condition | Changes whether the porous substrate behaves like a drain, membrane, or supported surface. | Glass, air gap, absorbent backing, and support conditions. |
| Contact angle / wetting | Sets footprint size, spreading dynamics, and transport length scale. | Contact-line behavior across substrate/backing states. |
| Contact-line pinning | Influences coffee-ring-like accumulation and edge crowding. | Pinned, receding, and mixed regimes from video. |
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
 <div class="process-map-stage decision-stage"><p>METRICS</p><span>r(t), density, edge/center ratio, repeatability</span></div>
</div>

## Methods and tools

<div class="two-col">
 <div class="matrix-card">
 <h3>Experimental methods</h3>
 <p>Sessile droplet deposition, AAO/substrate comparisons, backing-layer studies, optical microscopy, top-view videos, side-view videos, and process observation.</p>
 </div>
 <div class="matrix-card">
 <h3>Analysis methods</h3>
 <p>Droplet-radius extraction, contact-line tracking, deposition-pattern quantification, radial density maps, edge/center ratio, and statistical comparison.</p>
 </div>
</div>

<div class="badge-row">
 <span class="badge">Keyence</span>
 <span class="badge">Rame-Hart</span>
 <span class="badge">Python</span>
 <span class="badge">ImageJ/Fiji</span>
 <span class="badge">JMP</span>
 <span class="badge">Optical Microscopy</span>
</div>

## What I can show

<div class="text-output-grid">
 <article><h3>Contact-line dynamics</h3><p><strong>Metric:</strong> normalized radius, r(t)/r₀. <strong>Use:</strong> separates spreading, pinning, recession, and substrate drainage behavior.</p></article>
 <article><h3>Deposition uniformity</h3><p><strong>Metric:</strong> edge/center ratio. <strong>Use:</strong> compares edge crowding against useful central-device placement.</p></article>
 <article><h3>Substrate decision</h3><p><strong>Metric set:</strong> liquid removal behavior, contact-line behavior, deposition output, and repeatability. <strong>Use:</strong> screen new substrate/backing combinations before printing interconnects.</p></article>
</div>

<div class="placeholder-figure-grid deposition-output-grid">
 <figure class="data-placeholder-figure wide-placeholder">
  <img src="{{ '/assets/images/placeholder-deposition-comparison.svg' | relative_url }}" alt="Placeholder for side-by-side deposition microscopy images across substrate conditions." loading="lazy">
  <figcaption>Evidence slot: same-magnification optical microscopy images for glass/control, porous membrane/air gap, and porous membrane/absorbent backing.</figcaption>
 </figure>
 <figure class="data-placeholder-figure">
  <img src="{{ '/assets/images/placeholder-radius-trace.svg' | relative_url }}" alt="Placeholder for r(t)/r0 normalized contact-line trace." loading="lazy">
  <figcaption>Contact-line trace slot for r(t)/r₀ versus normalized drying/imbibition time.</figcaption>
 </figure>
 <figure class="data-placeholder-figure">
  <img src="{{ '/assets/images/placeholder-edge-center-ratio.svg' | relative_url }}" alt="Placeholder for edge to center deposition ratio chart." loading="lazy">
  <figcaption>Decision-metric slot for edge/center ratio across substrate/backing conditions.</figcaption>
 </figure>
</div>

## What I’d do next

If I were moving this toward a production screen, I would automate the video-to-metric pipeline first. The bottleneck is not only the droplet experiment; it is making the same measurement fast enough that substrate candidates can be compared before the process drifts.

<div class="case-cta-row">
 <a class="button primary" href="{{ '/projects/printed-interconnect-reliability/' | relative_url }}">Related reliability build →</a>
 <a class="button secondary" href="{{ '/assets/files/Nathan_Anderson_Resume.pdf' | relative_url }}" download="Nathan_Anderson_Resume.pdf">Download Resume</a>
 <a class="button tertiary" href="mailto:{{ site.email }}">Contact</a>
</div>
