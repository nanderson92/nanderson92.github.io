---
layout: page
title: Projects
category: Case File Library
subtitle: Proof-of-work artifacts: project pages, methods, figures, tools, outputs, and current buildout status.
---

<div class="section-note">
  <strong>Projects = technical proof-of-work:</strong> this page collects case files around problem, method, output, tools, and status so visitors can quickly scan the engineering work behind the portfolio.
</div>

<div class="filter-row" aria-label="Project filters">
  <span class="filter-chip active">All</span>
  <span class="filter-chip">Research</span>
  <span class="filter-chip">Process Engineering</span>
  <span class="filter-chip">Data</span>
  <span class="filter-chip">Computation</span>
  <span class="filter-chip">Manufacturing</span>
</div>

<div class="portfolio-grid projects-library">
  <article class="portfolio-card feature-project evidence-card">
    <div class="card-visual visual-droplet" aria-hidden="true"></div>
    <div class="card-topline"><span>Research · Advanced Manufacturing · Interfacial Transport</span><span>Status: In progress</span></div>
    <h2>Micromodular Printed Electronics Deposition</h2>
    <p class="problem-line">Nonuniform deposition limits scalable printed electronics assembly.</p>
    <div class="evidence-table">
      <span><strong>Problem</strong> Microscale devices can accumulate nonuniformly during droplet drying or imbibition.</span>
      <span><strong>Method</strong> Optical microscopy, droplet tracking, substrate comparison, contact-line dynamics, image analysis.</span>
      <span class="output-row"><strong>Output</strong> Process-window metrics, deposition-pattern figures, and substrate-selection logic for more uniform deposition.</span>
      <span><strong>Tools</strong> Keyence · Python · ImageJ/Fiji · JMP.</span>
      <span><strong>Status</strong> In progress.</span>
    </div>
    <p><a href="{{ '/projects/micromodular-deposition/' | relative_url }}">Open full case study →</a></p>
  </article>

  <article class="portfolio-card evidence-card">
    <div class="card-visual visual-pfd" aria-hidden="true"></div>
    <div class="card-topline"><span>Process Engineering · Simulation</span><span>Status: Buildout</span></div>
    <h2>Process Simulation and Design</h2>
    <p class="problem-line">Translate process requirements into flowsheets, balances, and operating decisions.</p>
    <div class="evidence-table">
      <span><strong>Problem</strong> Chemical process design needs defensible assumptions, model choices, and balance closure.</span>
      <span><strong>Method</strong> PFDs, material/energy balances, VLE reasoning, Aspen simulation, design comparison.</span>
      <span class="output-row"><strong>Output</strong> Process models, design tradeoffs, operating-condition comparisons, and engineering calculations.</span>
      <span><strong>Tools</strong> Aspen · MATLAB · Excel.</span>
      <span><strong>Status</strong> Case study buildout in progress — current focus: method, metrics, and representative figures.</span>
    </div>
    <p><a href="{{ '/projects/process-simulation-design/' | relative_url }}">Open full case study →</a></p>
  </article>

  <article class="portfolio-card evidence-card">
    <div class="card-visual visual-signal" aria-hidden="true"></div>
    <div class="card-topline"><span>Reliability · Experimental Analysis</span><span>Status: Developing</span></div>
    <h2>Printed Interconnect Reliability Analysis</h2>
    <p class="problem-line">Understand how printed interconnect resistance changes under stress and aging.</p>
    <div class="evidence-table">
      <span><strong>Problem</strong> Resistance drift can hide process instability or reliability issues.</span>
      <span><strong>Method</strong> Resistance tracking, reliability plots, ANOVA-style comparisons, trend analysis.</span>
      <span class="output-row"><strong>Output</strong> Stress-response summaries, drift plots, and process/reliability interpretation.</span>
      <span><strong>Tools</strong> JMP · Excel · Python.</span>
      <span><strong>Status</strong> Case study buildout in progress — current focus: method, metrics, and representative figures.</span>
    </div>
    <p><a href="{{ '/projects/printed-interconnect-reliability/' | relative_url }}">Open full case study →</a></p>
  </article>

  <article class="portfolio-card evidence-card">
    <div class="card-visual visual-compute" aria-hidden="true"></div>
    <div class="card-topline"><span>Computation · Image Analysis</span><span>Status: In progress</span></div>
    <h2>Droplet and Image Analysis Workflows</h2>
    <p class="problem-line">Extract usable engineering variables from videos, microscopy images, and time series.</p>
    <div class="evidence-table">
      <span><strong>Problem</strong> Raw microscopy and droplet videos need consistent measurement workflows before they can support process decisions.</span>
      <span><strong>Method</strong> Segmentation, scale calibration, time-series extraction, plotting, validation against baseline observations.</span>
      <span class="output-row"><strong>Output</strong> Workflows for r(t), θ(t), V(t), edge/center ratio, and deposition distributions.</span>
      <span><strong>Tools</strong> Python · ImageJ/Fiji · MATLAB.</span>
      <span><strong>Status</strong> Case study buildout in progress — current focus: method, metrics, and representative figures.</span>
    </div>
    <p><a href="{{ '/projects/droplet-image-analysis-workflows/' | relative_url }}">Open full case study →</a></p>
  </article>
</div>
