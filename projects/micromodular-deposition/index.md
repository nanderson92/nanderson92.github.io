---
layout: page
title: Micromodular Electronics Deposition
category: Active research · 2025–present
tags: Semiconductors · Wet processing · Image-derived metrics
subtitle: Boundary-condition control for placing suspended microdevices into useful printed-electronics layouts.
---

<p class="case-thesis">When you print microdevices from a droplet, they crowd at the edges and land in useless patterns. I spent a year figuring out which substrate conditions actually fix that.</p>

<figure class="wide-figure flagship-workflow-figure builder-wide-workflow">
 <img src="{{ '/assets/images/micromodular-workflow-deposition-focus.png' | relative_url }}" alt="Micromodular electronics workflow with the deposition subsystem highlighted." loading="eager">
 <figcaption>The highlighted subsystem is the part I work on: getting suspended components out of liquid and onto a substrate in patterns that downstream interconnect printing can actually use.</figcaption>
</figure>

<div class="case-summary-box clean-metadata-layout">
 <p class="system-label small">QUICK READ</p>
 <div class="case-summary-grid">
  <span><strong>Role</strong> I designed substrate/backing experiments, captured top-view and side-view droplet videos, and converted the videos into metrics.</span>
  <span><strong>System</strong> IPA-based suspended microdevice deposition onto porous and nonporous substrate/backing conditions.</span>
  <span><strong>Inputs</strong> Droplet volume, substrate, backing, wetting behavior, device loading, and deposition method.</span>
  <span><strong>Measured outputs</strong> r(t), θ(t), V(t) proxy, edge/center ratio, useful areal density, and repeatability.</span>
  <span><strong>Decision</strong> Screen boundary conditions that reduce edge crowding and preserve interconnect access.</span>
 </div>
</div>

<div class="role-block flagship-role-block">
 <p class="system-label small">MY ROLE</p>
 <p>I designed the experiments from scratch — chose the substrates, set up both top-view and side-view video capture, wrote the Python and ImageJ pipelines to extract contact-line metrics, and used those metrics to figure out which boundary conditions actually produce useful placement. The core output was a decision framework the lab now uses to screen new substrates.</p>
</div>

## The hard part

Printed electronics is not only a materials problem; it is an assembly problem. Suspended microdevices can raft, crowd, pin near the contact line, and accumulate nonuniformly as the carrier liquid spreads, evaporates, and/or imbibes into the substrate.

> What substrate boundary conditions produce repeatable, spatially useful deposition instead of edge-heavy accumulation?

<div class="thesis-box builder-thesis-box">
 <p class="system-label small">WHAT I LEARNED</p>
 <h2>If the substrate controls how liquid leaves the droplet, it controls where devices end up.</h2>
 <p>The first substrate I tried made the coffee-ring problem worse than bare glass. That failure pushed me to stop treating “substrate” as one variable and start testing backing conditions as the hidden control variable.</p>
</div>

## Process map

<div class="process-map central-process-map" aria-label="Process input to engineering decision map">
 <div class="process-map-stage"><p>INPUTS</p><span>droplet volume</span><span>solvent</span><span>device loading</span><span>substrate</span><span>backing layer</span></div>
 <div class="process-map-arrow" aria-hidden="true">→</div>
 <div class="process-map-stage"><p>TRANSPORT</p><span>spreading</span><span>imbibition</span><span>evaporation</span><span>pinning</span><span>rafting/crowding</span></div>
 <div class="process-map-arrow" aria-hidden="true">→</div>
 <div class="process-map-stage"><p>METRICS</p><span>r(t)/r₀</span><span>θ(t)</span><span>edge/center ratio</span><span>density map</span><span>repeatability</span></div>
 <div class="process-map-arrow" aria-hidden="true">→</div>
 <div class="process-map-stage decision-stage"><p>DECISION</p><span>accept, reject, or redesign the boundary condition</span></div>
</div>

## Why it breaks

<div class="hard-problem-notes">
 <p><strong>Coupled liquid removal.</strong> Evaporation and imbibition compete, so the final deposit does not reveal the full transport history.</p>
 <p><strong>Contact-line memory.</strong> Pinned, depinned, and receding regimes can produce similar final images.</p>
 <p><strong>Device crowding.</strong> Dense deposits are not automatically useful if devices become inaccessible to interconnect routing.</p>
 <p><strong>Manufacturing constraint.</strong> The best pattern preserves interconnect access, not merely the highest local device density.</p>
</div>

## Variables I tested

| Variable | Why it matters | What I varied / observed |
|---|---|---|
| Substrate porosity / permeability | Controls liquid uptake and vertical drain rate. | Compared porous AAO-like behavior against less-draining surfaces. |
| Backing condition | Changes whether the porous substrate behaves like a drain, membrane, or supported surface. | Tested supported, open, and absorbent backing conditions. |
| Contact angle / wetting | Sets footprint size, spreading dynamics, and transport length scale. | Tracked footprint evolution and side-view wetting behavior. |
| Contact-line pinning | Influences coffee-ring-like accumulation and edge crowding. | Compared pinned, receding, and draining regimes through video. |
| Evaporation vs. imbibition | Determines whether flow is dominated by drying or liquid uptake. | Separated glass-like evaporation from porous liquid-removal behavior. |
| Device loading | Affects crowding, raft interactions, and useful areal density. | Interpreted final density and edge/center distribution against process conditions. |

## Public artifacts

<div class="artifact-grid flagship-artifact-grid">
 <article class="artifact-card"><div><p class="system-label small">ARTIFACT 01</p><h3>Contact-line dynamics: r(t)</h3><p><strong>Purpose:</strong> track how the droplet footprint changes over time on different substrate/backing conditions.</p><p><strong>Output:</strong> normalized droplet-radius behavior, r(t)/r₀, comparing representative substrate conditions.</p></div><figure class="result-figure"><img src="{{ '/assets/images/preliminary-radius-plot.svg' | relative_url }}" alt="Representative normalized droplet radius plot." loading="lazy"><figcaption>Representative figure — full data available on request where publishable.</figcaption></figure></article>
 <article class="artifact-card"><div><p class="system-label small">ARTIFACT 02</p><h3>Deposition uniformity: edge/center ratio</h3><p><strong>Definition:</strong> edge/center ratio = device density near the droplet perimeter ÷ device density in the useful central region.</p><p><strong>Why it matters:</strong> useful patterns leave devices accessible for downstream interconnect routing.</p></div><figure class="result-figure"><img src="{{ '/assets/images/deposition-pattern-schematic.svg' | relative_url }}" alt="Radial deposition schematic showing edge and center regions." loading="lazy"><figcaption>Radial schematic for explaining edge-heavy versus useful deposition.</figcaption></figure></article>
</div>

## Tools

<div class="badge-row"><span class="badge">Keyence</span><span class="badge">Rame-Hart</span><span class="badge">Python</span><span class="badge">ImageJ/Fiji</span><span class="badge">JMP</span><span class="badge">Optical Microscopy</span></div>

## What I’d do next

If I were building this for production, I would make the substrate/backing stack the controlled product, not an experimental convenience. I would add inline mass tracking, humidity control, and automated droplet dispense so the process window is based on flux and placement metrics rather than visual inspection alone.

<div class="case-cta-row">
 <a class="button primary" href="{{ '/projects/printed-interconnect-reliability/' | relative_url }}">Related reliability build log →</a>
 <a class="button secondary" href="{{ '/assets/files/Nathan_Anderson_Resume.pdf' | relative_url }}" download="Nathan_Anderson_Resume.pdf">Resume (PDF, 1 page)</a>
 <a class="button tertiary" href="mailto:{{ site.email }}">Contact</a>
</div>
