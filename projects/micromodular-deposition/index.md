---
layout: page
title: Micromodular Electronics Deposition
category: Edge crowding → useful placement
tags: Semiconductors · Process Development · Interfacial Transport · Automation & Data
subtitle: "When you print microdevices from a droplet, they crowd at the edges and land in useless patterns. I spent a year figuring out which substrate conditions actually fix that."
---

<figure class="flagship-page-visual">
 <img src="{{ '/assets/images/micromodular-workflow-deposition-focus.png' | relative_url }}" alt="Micromodular electronics workflow with the deposition subsystem highlighted." loading="eager">
 <figcaption>System view: deposition is the boundary-condition-controlled subsystem between fabricated components and printable circuit assembly.</figcaption>
</figure>

The manufacturing goal is not simply to deposit devices. The goal is to create repeatable, spatially useful placement so that downstream interconnect printing can become more reliable.

<div class="case-summary-box startup-summary-box">
 <p class="system-label small">CASE SUMMARY</p>
 <div class="case-summary-grid">
  <span><strong>Role</strong> Designed substrate/backing experiments, built video capture workflows, and extracted deposition metrics.</span>
  <span><strong>System</strong> IPA-based suspended microdevice deposition onto substrate/backing conditions.</span>
  <span><strong>Inputs</strong> Droplet volume, substrate, backing, wetting behavior, device loading, and deposition method.</span>
  <span><strong>Measured outputs</strong> r(t), θ(t), V(t) proxy, edge/center ratio, useful areal density, and repeatability.</span>
  <span><strong>Decision</strong> Identify conditions that reduce edge crowding and preserve interconnect access.</span>
 </div>
</div>

<div class="role-block flagship-role-block">
 <p class="system-label small">MY ROLE</p>
 <p>I designed the experiments from scratch: chose the substrates, set up both top-view and side-view video capture, wrote the Python and ImageJ pipelines to extract contact-line metrics, and used those metrics to figure out which boundary conditions actually produce useful placement.</p>
 <p><strong>Core output:</strong> a substrate-screening decision framework the lab can use to evaluate new deposition surfaces before committing to downstream interconnect printing.</p>
</div>

## Why this matters

Suspended microdevices can raft, crowd, pin near the contact line, and accumulate nonuniformly as the carrier liquid spreads, evaporates, and/or imbibes into the substrate.

The practical question is:

> What substrate boundary conditions produce repeatable, spatially useful deposition instead of edge-heavy accumulation?

## Where this project fits in the workflow

<figure class="wide-figure flagship-workflow-figure">
 <img src="{{ '/assets/images/micromodular-workflow-deposition-focus.png' | relative_url }}" alt="High-level micromodular electronics workflow with the deposition subsystem highlighted across suspending components in ink and printing components." loading="lazy">
 <figcaption><strong>Micromodular electronics workflow.</strong> The highlighted subsystem covers the deposition problem: getting fabricated components into an ink and printing them onto a substrate in a way that produces useful placement for downstream circuit assembly.</figcaption>
</figure>

<div class="thesis-box">
 <p class="system-label small">WHAT CHANGED MY THINKING</p>
 <h2>If the substrate controls how liquid leaves the droplet, it controls where devices end up.</h2>
 <p>The hard part was separating surface wetting, porous drainage, evaporation, and contact-line pinning instead of treating the final stain pattern as the whole story.</p>
</div>

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
 <p>TRANSPORT REGIME</p>
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

<div class="hard-problem-grid editorial-hard-list">
 <div class="matrix-card"><h3>Coupled liquid removal</h3><p>Evaporation and imbibition compete, so the final deposit does not reveal the full transport history.</p></div>
 <div class="matrix-card"><h3>Contact-line memory</h3><p>Pinned, depinned, and receding regimes can produce similar final images.</p></div>
 <div class="matrix-card"><h3>Device crowding</h3><p>Dense deposits are not automatically useful if devices become inaccessible to interconnect routing.</p></div>
 <div class="matrix-card"><h3>Manufacturing constraint</h3><p>The best pattern preserves interconnect access, not merely the highest local device density.</p></div>
</div>

## What did not work at first

Some early conditions looked promising because they moved liquid quickly, but the deposit still ended up edge-heavy or spatially useless. That pushed the work away from “which surface looks best?” and toward a harder question: which substrate/backing boundary condition gives a repeatable transport history and a pattern that can still be wired later?

## Variables studied

| Variable | Why it matters | What I varied / compared |
|---|---|---|
| Substrate porosity / permeability | Controls liquid uptake and vertical drain rate. | Porous membranes versus low-uptake controls. |
| Backing condition | Changes whether the porous substrate behaves like a drain, membrane, or supported surface. | Glass, air gap, absorbent backing, and support conditions. |
| Contact angle / wetting | Sets footprint size, spreading dynamics, and transport length scale. | Contact-line behavior across substrate/backing states. |
| Contact-line pinning | Influences coffee-ring-like accumulation and edge crowding. | Pinned, receding, and mixed regimes from video. |
| Evaporation vs. imbibition | Determines whether flow is dominated by drying or liquid uptake. | Glass-like evaporation baseline versus porous uptake behavior. |
| Device loading | Affects crowding, raft interactions, and useful areal density. | Qualitative loading/crowding state during deposition. |

## Methods and tools

<div class="two-col">
 <div class="matrix-card">
 <h3>Experimental methods</h3>
 <p>Sessile droplet deposition, AAO/substrate comparisons, backing-layer studies, optical microscopy, top-view videos, side-view videos, and process observation.</p>
 </div>
 <div class="matrix-card">
 <h3>Analysis methods</h3>
 <p>Droplet-radius extraction, contact-line tracking, deposition-pattern quantification, radial density maps, edge/center ratio, process-window framing, and statistical comparison.</p>
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

## Engineering artifacts

<div class="artifact-grid flagship-artifact-grid">
 <article class="artifact-card">
 <div>
 <p class="system-label small">ARTIFACT 01</p>
 <h3>Contact-line dynamics: r(t)</h3>
 <p><strong>Purpose:</strong> track how the droplet footprint changes over time on different substrate/backing conditions.</p>
 <p><strong>Why it matters:</strong> the contact-line trajectory reflects whether the droplet is spreading, pinned, receding, or being drained through the substrate.</p>
 <p><strong>Output:</strong> a normalized droplet-radius plot, r(t)/r₀, comparing representative substrate conditions.</p>
 </div>
 <figure class="result-figure">
 <img src="{{ '/assets/images/preliminary-radius-plot.svg' | relative_url }}" alt="Representative normalized droplet radius plot." loading="lazy">
 <figcaption>Representative target curves: glass-like baseline versus porous substrate behavior, with a repeatability band.</figcaption>
 </figure>
 </article>

 <article class="artifact-card">
 <div>
 <p class="system-label small">ARTIFACT 02</p>
 <h3>Deposition uniformity: edge/center ratio</h3>
 <p><strong>Definition:</strong> edge/center ratio = device density near the droplet perimeter ÷ device density in the useful central region.</p>
 <p><strong>Interpretation:</strong> a high edge/center ratio indicates edge-heavy accumulation. A lower, repeatable edge/center ratio indicates more spatially useful deposition.</p>
 <p><strong>Why it matters:</strong> the useful pattern is the one that leaves devices accessible for downstream interconnect routing.</p>
 </div>
 <figure class="result-figure">
 <img src="{{ '/assets/images/deposition-pattern-schematic.svg' | relative_url }}" alt="Radial deposition schematic showing edge and center regions." loading="lazy">
 <figcaption>Radial deposition schematic used to explain the edge/center metric.</figcaption>
 </figure>
 </article>

 <article class="artifact-card process-window-artifact">
 <div>
 <p class="system-label small">ARTIFACT 03</p>
 <h3>Substrate-selection process window</h3>
 <p><strong>Purpose:</strong> classify substrate/backing conditions by whether they produce useful, repeatable deposition.</p>
 <p><strong>Candidate axes:</strong> liquid removal behavior, contact-line behavior, deposition output, and repeatability.</p>
 <p><strong>Decision:</strong> a substrate condition is promising if it improves useful areal density, limits edge crowding, and produces repeatable behavior across trials.</p>
 </div>
 <div class="process-window-mini scatter-window" aria-label="Qualitative process window scatter diagram">
 <span class="axis-label x-label">liquid uptake / evaporation behavior</span>
 <span class="axis-label y-label">edge/center ratio</span>
 <i class="region"></i>
 <b class="point baseline"><em></em>Glass-like baseline</b>
 <b class="point porous"><em></em>AAO-like boundary</b>
 <b class="point target"><em></em>Engineered skin</b>
 </div>
 </article>
</div>

## Technical basis

Particle-laden sessile droplets often form nonuniform deposits because evaporation, capillary flow, contact-line pinning, substrate permeability, and particle interactions are coupled. In this system, the substrate is not just a passive support. It becomes a process variable that can redirect how liquid leaves the droplet and how microdevices are transported before the pattern locks.

## What I’d do next

If I were building this toward production, I would move from substrate screening to a controlled coating stack: one top surface that sets wetting and pinning, one porous or absorbent layer that sets liquid removal, and one backing condition that makes the behavior repeatable independent of the final device substrate. I would also add automated frame-to-frame particle tracking so the decision rule is based on device motion during drying, not only the final deposit.

<div class="case-cta-row">
 <a class="button primary" href="{{ '/projects/printed-interconnect-reliability/' | relative_url }}">Related reliability build →</a>
 <a class="button secondary" href="{{ '/assets/files/Nathan_Anderson_Resume.pdf' | relative_url }}" download="Nathan_Anderson_Resume.pdf">Download Resume</a>
 <a class="button tertiary" href="mailto:{{ site.email }}">Contact</a>
</div>
