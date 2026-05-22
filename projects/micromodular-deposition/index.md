---
layout: page
title: Micromodular Electronics Deposition
category: Flagship Case Study
tags: Semiconductors · Process Development · Interfacial Transport · Automation & Data
subtitle: Substrate-controlled process windows for stochastic microdevice placement in micromodular printed electronics.
---

<p class="case-thesis">This project asks a process-engineering question: how do substrate boundary conditions control where suspended microdevices end up after a droplet spreads, dries, and imbibes?</p>

The manufacturing goal is not simply to deposit devices. The goal is to create repeatable, spatially useful placement so that downstream interconnect printing can become more reliable.

<div class="buildout-note polished-note">This public-facing case study uses recreated schematics, anonymized process logic, and public-safe metrics to explain the engineering workflow without exposing raw lab visuals or unpublished details.</div>

<div class="role-block flagship-role-block">
  <p class="system-label small">MY ROLE</p>
  <p>I designed substrate/backing experiments, captured top-view and side-view droplet videos, extracted contact-line dynamics, compared deposition behavior across boundary conditions, and built Python/ImageJ workflows for converting microscopy data into process metrics.</p>
  <p><strong>Core output:</strong> a process-window framework connecting substrate choice, droplet transport, deposition uniformity, and downstream printed-electronics assembly.</p>
</div>

## Why this matters

Printed electronics is not only a materials problem; it is an assembly problem. Suspended microdevices can raft, crowd, pin near the contact line, and accumulate nonuniformly as the carrier liquid spreads, evaporates, and/or imbibes into the substrate.

The practical question is:

> What substrate boundary conditions produce repeatable, spatially useful deposition instead of edge-heavy accumulation?

## Where this project fits in the workflow

<figure class="wide-figure flagship-workflow-figure">
  <img src="{{ '/assets/images/micromodular-workflow-deposition-focus.png' | relative_url }}" alt="High-level micromodular electronics workflow with the deposition subsystem highlighted across suspending components in ink and printing components." loading="lazy">
  <figcaption><strong>Micromodular electronics workflow.</strong> The highlighted subsystem covers the deposition problem: getting fabricated components into an ink and printing them onto a substrate in a way that produces useful placement for downstream circuit assembly.</figcaption>
</figure>

<div class="thesis-box">
  <p class="system-label small">ENGINEERING THESIS</p>
  <h2>Micromodular deposition is not only a particle-placement problem. It is a boundary-condition problem.</h2>
  <p>If the substrate controls how liquid leaves the droplet, then the substrate also helps control device transport, crowding, edge accumulation, and final placement fidelity.</p>
  <p>The engineering task is to identify which boundary conditions create a repeatable deposition window.</p>
</div>

## Process map

<div class="process-map" aria-label="Process input to engineering decision map">
  <div class="process-map-stage">
    <p>PROCESS INPUTS</p>
    <span>Droplet volume</span>
    <span>Solvent</span>
    <span>Device loading</span>
    <span>Substrate</span>
    <span>Backing layer</span>
    <span>Deposition method</span>
  </div>
  <div class="process-map-arrow" aria-hidden="true">→</div>
  <div class="process-map-stage">
    <p>TRANSPORT BEHAVIOR</p>
    <span>Spreading</span>
    <span>Imbibition</span>
    <span>Evaporation</span>
    <span>Contact-line pinning</span>
    <span>Edgeward flow</span>
    <span>Device rafting/crowding</span>
  </div>
  <div class="process-map-arrow" aria-hidden="true">→</div>
  <div class="process-map-stage">
    <p>MEASURED OUTPUTS</p>
    <span>r(t)</span>
    <span>θ(t)</span>
    <span>V(t) proxy</span>
    <span>Radial density</span>
    <span>Edge/center ratio</span>
    <span>Repeatability</span>
  </div>
  <div class="process-map-arrow" aria-hidden="true">→</div>
  <div class="process-map-stage decision-stage">
    <p>ENGINEERING DECISION</p>
    <span>Which boundary condition gives repeatable, useful placement for downstream interconnect printing?</span>
  </div>
</div>

## Why this is hard

<div class="matrix hard-problem-grid">
  <div class="matrix-card"><h3>Coupled liquid removal</h3><p>The droplet footprint changes as liquid spreads, evaporates, and/or imbibes through the substrate.</p></div>
  <div class="matrix-card"><h3>Contact-line regimes</h3><p>The perimeter can pin, depin, or recede depending on the surface and backing condition.</p></div>
  <div class="matrix-card"><h3>Device crowding</h3><p>Suspended microdevices can raft, collide, and accumulate in regions that are visually dense but not useful.</p></div>
  <div class="matrix-card"><h3>Hidden histories</h3><p>The same final image can hide different transport histories, so time-resolved video matters.</p></div>
  <div class="matrix-card"><h3>Manufacturing utility</h3><p>The best pattern is not automatically the densest one; it is the one that enables downstream interconnect access.</p></div>
  <div class="matrix-card"><h3>Mechanism over appearance</h3><p>The engineering challenge is separating what looks better from what is actually controllable and repeatable.</p></div>
</div>

## Variables studied

| Variable | Why it matters |
|---|---|
| Substrate porosity / permeability | Controls liquid uptake and vertical drain rate. |
| Backing condition | Changes whether the porous substrate behaves like a drain, membrane, or supported surface. |
| Contact angle / wetting | Sets footprint size, spreading dynamics, and transport length scale. |
| Contact-line pinning | Influences coffee-ring-like accumulation and edge crowding. |
| Evaporation vs. imbibition | Determines whether flow is dominated by drying or liquid uptake. |
| Device loading | Affects crowding, raft interactions, and useful areal density. |

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

## Public-safe engineering artifacts

<div class="artifact-grid flagship-artifact-grid">
  <article class="artifact-card">
    <div>
      <p class="system-label small">ARTIFACT 01</p>
      <h3>Contact-line dynamics: r(t)</h3>
      <p><strong>Purpose:</strong> track how the droplet footprint changes over time on different substrate/backing conditions.</p>
      <p><strong>Why it matters:</strong> the contact-line trajectory reflects whether the droplet is spreading, pinned, receding, or being drained through the substrate. These regimes affect how suspended devices are transported before final deposition.</p>
      <p><strong>Output:</strong> a normalized droplet-radius plot, r(t)/r0, comparing representative substrate conditions.</p>
    </div>
    <figure class="result-figure">
      <img src="{{ '/assets/images/preliminary-radius-plot.svg' | relative_url }}" alt="Public-safe representative normalized droplet radius plot." loading="lazy">
      <figcaption>Representative public-safe radius trace. Replace with final experimental plot when publishable.</figcaption>
    </figure>
  </article>

  <article class="artifact-card">
    <div>
      <p class="system-label small">ARTIFACT 02</p>
      <h3>Deposition uniformity: edge/center ratio</h3>
      <p><strong>Definition:</strong> edge/center ratio = device density near the droplet perimeter ÷ device density in the useful central region.</p>
      <p><strong>Interpretation:</strong> a high edge/center ratio indicates edge-heavy accumulation. A lower, repeatable edge/center ratio indicates more spatially useful deposition.</p>
      <p><strong>Why it matters:</strong> for micromodular electronics, the useful pattern is the one that leaves devices accessible for downstream interconnect routing.</p>
    </div>
    <figure class="result-figure">
      <img src="{{ '/assets/images/deposition-pattern-schematic.svg' | relative_url }}" alt="Public-safe radial deposition schematic showing edge and center regions." loading="lazy">
      <figcaption>Public-safe radial deposition schematic used to explain the edge/center metric.</figcaption>
    </figure>
  </article>

  <article class="artifact-card process-window-artifact">
    <div>
      <p class="system-label small">ARTIFACT 03</p>
      <h3>Substrate-selection process window</h3>
      <p><strong>Purpose:</strong> classify substrate/backing conditions by whether they produce useful, repeatable deposition.</p>
      <p><strong>Candidate axes:</strong> liquid removal behavior, contact-line behavior, deposition output, and repeatability.</p>
      <p><strong>Engineering decision:</strong> a substrate condition is only promising if it improves useful areal density, limits edge crowding, and produces repeatable behavior across trials.</p>
    </div>
    <div class="process-window-mini" aria-label="Qualitative process window diagram">
      <span class="axis-label x-label">liquid uptake / evaporation behavior</span>
      <span class="axis-label y-label">edge/center ratio</span>
      <i class="region"></i>
      <b class="point baseline">Glass-like baseline</b>
      <b class="point porous">AAO-like boundary</b>
      <b class="point target">Engineered skin</b>
    </div>
  </article>
</div>

## Technical basis

Particle-laden sessile droplets often form nonuniform deposits because evaporation, contact-line pinning, and internal capillary flow can transport suspended material toward the perimeter. For micromodular electronics, the same general physics becomes a manufacturing issue: edge-heavy deposition can reduce useful placement and complicate downstream interconnect printing.

This project studies whether substrate boundary conditions can shift the system away from uncontrolled edge accumulation and toward a repeatable deposition window.

## Manufacturing relevance

A lab demonstration can tolerate stochastic placement. A manufacturing process cannot.

For micromodular electronics, deposition quality affects whether devices land in useful regions, whether interconnect printing can reach them, whether placement varies too much from drop to drop, whether process settings can be transferred across substrates, and whether inspection metrics can predict downstream assembly success.

This case study frames deposition as a process-control problem: define the controllable inputs, measure the transport response, quantify the final pattern, and identify the boundary conditions that create a usable process window.

## Skills demonstrated

<div class="skill-proof-grid">
  <div class="matrix-card"><h3>Process development</h3><p>Designed controlled substrate/backing comparisons and translated visual deposition behavior into process criteria.</p></div>
  <div class="matrix-card"><h3>Transport phenomena</h3><p>Connected spreading, evaporation, imbibition, pinning, and particle/device transport to final manufacturing output.</p></div>
  <div class="matrix-card"><h3>Data analysis</h3><p>Used microscopy, Python, ImageJ/Fiji, and statistical comparison to extract process descriptors from videos and images.</p></div>
  <div class="matrix-card"><h3>Manufacturing thinking</h3><p>Defined output metrics such as edge/center ratio, useful areal density, repeatability, and downstream interconnect feasibility.</p></div>
  <div class="matrix-card"><h3>Technical communication</h3><p>Built public-safe schematics and process maps to explain unpublished lab work without exposing sensitive details.</p></div>
</div>

## Ongoing development

<div class="matrix">
  <div class="matrix-card"><h3>Artifact development</h3><p>Replace recreated figures with publishable images, annotated frames, and clean comparison plots when appropriate.</p></div>
  <div class="matrix-card"><h3>Metric definition</h3><p>Lock edge/center ratio, useful areal density, and acceptable repeatability thresholds.</p></div>
  <div class="matrix-card"><h3>Manufacturing translation</h3><p>Connect AAO-like behavior to a substrate-agnostic coating or boundary-condition design rule.</p></div>
</div>

<div class="case-cta-row">
  <a class="button primary" href="{{ '/projects/printed-interconnect-reliability/' | relative_url }}">Related reliability project →</a>
  <a class="button secondary" href="{{ '/assets/files/Nathan_Anderson_Resume.pdf' | relative_url }}">Download Resume</a>
  <a class="button tertiary" href="mailto:{{ site.email }}">Contact</a>
</div>
