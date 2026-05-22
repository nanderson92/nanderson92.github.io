---
layout: page
title: Projects
category: Case Study Library
subtitle: Selected technical work in process development, manufacturing, data analysis, computation, and research translation.
---

<div class="filter-row" aria-label="Project categories">
  <span class="filter-chip active">All</span>
  <span class="filter-chip">Research</span>
  <span class="filter-chip">Process Engineering</span>
  <span class="filter-chip">Data</span>
  <span class="filter-chip">Computation</span>
  <span class="filter-chip">Manufacturing</span>
</div>

<div class="project-library">
  <article class="case-card case-feature">
    <div class="card-visual visual-droplet" aria-hidden="true"></div>
    <div class="case-topline"><span>Research · Advanced Manufacturing · Interfacial Transport</span><span>Status: In progress</span></div>
    <h2>Micromodular Printed Electronics Deposition</h2>
    <p class="case-problem">Nonuniform deposition limits scalable printed electronics assembly.</p>
    <dl>
      <div><dt>Problem</dt><dd>Suspended microdevices can accumulate nonuniformly during droplet drying and substrate imbibition.</dd></div>
      <div><dt>Method</dt><dd>Optical microscopy, top/side-view droplet videos, contact-line tracking, substrate comparison, and image analysis.</dd></div>
      <div><dt>Output</dt><dd>Process-window metrics, deposition-distribution maps, and substrate-selection logic for more uniform deposition.</dd></div>
      <div><dt>Tools</dt><dd>Keyence · Python · ImageJ/Fiji · JMP</dd></div>
    </dl>
    <a class="text-link" href="{{ '/projects/micromodular-deposition/' | relative_url }}">Open full case study <span aria-hidden="true">→</span></a>
  </article>

  <article class="case-card">
    <div class="card-visual visual-pfd" aria-hidden="true"></div>
    <div class="case-topline"><span>Process Engineering · Simulation</span><span>Status: Buildout</span></div>
    <h2>Process Simulation and Design</h2>
    <p class="case-problem">Convert process requirements into flowsheets, balances, and defensible design decisions.</p>
    <dl>
      <div><dt>Problem</dt><dd>Engineering decisions need traceable mass/energy balances, thermodynamic assumptions, and realistic operating conditions.</dd></div>
      <div><dt>Method</dt><dd>PFDs, material and energy balances, VLE reasoning, Aspen simulation, and design comparison.</dd></div>
      <div><dt>Output</dt><dd>Process models, flow diagrams, operating-condition comparisons, and calculation packages.</dd></div>
      <div><dt>Tools</dt><dd>Aspen · MATLAB · Excel</dd></div>
    </dl>
  </article>

  <article class="case-card">
    <div class="card-visual visual-signal" aria-hidden="true"></div>
    <div class="case-topline"><span>Reliability · Experimental Analysis</span><span>Status: Developing</span></div>
    <h2>Printed Interconnect Reliability</h2>
    <p class="case-problem">Understand how printed interconnect resistance changes under stress and aging.</p>
    <dl>
      <div><dt>Problem</dt><dd>Resistance drift and failure behavior must be separated from measurement noise and limited-sample uncertainty.</dd></div>
      <div><dt>Method</dt><dd>Resistance tracking, reliability plots, ANOVA-style comparisons, trend analysis, and engineering interpretation.</dd></div>
      <div><dt>Output</dt><dd>Stress-response summaries and reliability interpretation for manufacturing-relevant decisions.</dd></div>
      <div><dt>Tools</dt><dd>JMP · Excel · Python</dd></div>
    </dl>
  </article>

  <article class="case-card">
    <div class="card-visual visual-compute" aria-hidden="true"></div>
    <div class="case-topline"><span>Computation · Image Analysis</span><span>Status: In progress</span></div>
    <h2>Droplet and Image Analysis Workflows</h2>
    <p class="case-problem">Extract quantitative engineering variables from videos, microscopy images, and experimental time series.</p>
    <dl>
      <div><dt>Problem</dt><dd>Low contrast, calibration, lighting variation, and noisy boundaries make manual measurement slow and inconsistent.</dd></div>
      <div><dt>Method</dt><dd>Segmentation, time-series extraction, curve plotting, and validation against baseline observations.</dd></div>
      <div><dt>Output</dt><dd>Measurement workflows for r(t), θ(t), V(t), and deposition-distribution analysis.</dd></div>
      <div><dt>Tools</dt><dd>Python · ImageJ/Fiji · MATLAB</dd></div>
    </dl>
  </article>
</div>
