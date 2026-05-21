---
layout: page
title: Projects
category: Case Study Library
subtitle: Selected technical work in process development, manufacturing, computation, and research translation.
---

<div class="filter-row" aria-label="Project filters">
  <span class="filter-chip active">All</span>
  <span class="filter-chip">Research</span>
  <span class="filter-chip">Process Engineering</span>
  <span class="filter-chip">Data</span>
  <span class="filter-chip">Computation</span>
  <span class="filter-chip">Manufacturing</span>
</div>

<div class="portfolio-grid projects-library">
  <article class="portfolio-card feature-project">
    <div class="card-visual visual-droplet" aria-hidden="true"></div>
    <div class="card-topline"><span>Research · Advanced Manufacturing · Interfacial Transport</span><span>Status: In progress</span></div>
    <h2>Micromodular Printed Electronics Deposition</h2>
    <p class="problem-line">Problem: Nonuniform deposition limits scalable printed electronics assembly.</p>
    <div class="artifact-line">
      <span><strong>System:</strong> IPA droplet + porous substrate + suspended microdevices.</span>
      <span><strong>My role:</strong> Designed experiments, captured top/side-view droplet videos, compared substrate boundary conditions, and developed process-window metrics.</span>
      <span><strong>Constraints:</strong> Microscopy geometry, droplet reproducibility, substrate heterogeneity, and confidentiality around lab visuals.</span>
      <span><strong>Methods:</strong> Optical microscopy, droplet tracking, contact-line dynamics, image analysis, substrate comparison.</span>
      <span><strong>Tools:</strong> Keyence · Python · ImageJ/Fiji · JMP.</span>
      <span><strong>Engineering output:</strong> Process-window metrics and substrate-selection logic for more uniform deposition.</span>
    </div>
    <p><a href="{{ '/projects/micromodular-deposition/' | relative_url }}">Open full case study →</a></p>
  </article>

  <article class="portfolio-card">
    <div class="card-visual visual-pfd" aria-hidden="true"></div>
    <div class="card-topline"><span>Process Engineering · Simulation</span><span>Status: Buildout</span></div>
    <h2>Process Simulation and Design</h2>
    <div class="artifact-line">
      <span><strong>Problem:</strong> Convert process requirements into flowsheets, balances, and defensible design decisions.</span>
      <span><strong>System:</strong> Chemical process units, separations, recycle logic, and thermodynamic models.</span>
      <span><strong>Methods:</strong> PFDs, mass/energy balances, VLE reasoning, Aspen simulation, design comparison.</span>
      <span><strong>Tools:</strong> Aspen · MATLAB · Excel.</span>
      <span><strong>Output:</strong> Process models, flow diagrams, operating-condition comparisons, and technical calculations.</span>
    </div>
  </article>

  <article class="portfolio-card">
    <div class="card-visual visual-signal" aria-hidden="true"></div>
    <div class="card-topline"><span>Reliability · Experimental Analysis</span><span>Status: Developing</span></div>
    <h2>Printed Interconnect Reliability</h2>
    <div class="artifact-line">
      <span><strong>Problem:</strong> Understand how printed interconnect resistance changes under stress and aging.</span>
      <span><strong>System:</strong> Printed Ag nanoparticle interconnects, resistance measurements, and environmental stress data.</span>
      <span><strong>Methods:</strong> Reliability plots, ANOVA-style comparisons, trend analysis, and engineering interpretation.</span>
      <span><strong>Tools:</strong> JMP · Excel · Python.</span>
      <span><strong>Output:</strong> Stress-response summaries and process/reliability interpretation.</span>
    </div>
  </article>

  <article class="portfolio-card">
    <div class="card-visual visual-compute" aria-hidden="true"></div>
    <div class="card-topline"><span>Computation · Image Analysis</span><span>Status: In progress</span></div>
    <h2>Droplet and Image Analysis Workflows</h2>
    <div class="artifact-line">
      <span><strong>Problem:</strong> Extract quantitative engineering variables from videos, microscopy images, and experimental time series.</span>
      <span><strong>System:</strong> Droplet videos, deposition images, time-dependent radius/contact-angle/volume measurements.</span>
      <span><strong>Methods:</strong> Segmentation, time-series extraction, curve plotting, and validation against baseline observations.</span>
      <span><strong>Tools:</strong> Python · ImageJ/Fiji · MATLAB.</span>
      <span><strong>Output:</strong> Measurement workflows for r(t), θ(t), V(t), and deposition distributions.</span>
    </div>
  </article>
</div>
