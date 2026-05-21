---
layout: page
title: Portfolio
category: Technical Portfolio
subtitle: Evidence-oriented project cards for research, process engineering, computation, and manufacturing translation.
---

<div class="portfolio-grid">
  <article class="portfolio-card">
    <div class="card-visual visual-droplet" aria-hidden="true"></div>
    <p class="tag">Research · Advanced Manufacturing · Interfacial Transport</p>
    <h2>Micromodular Printed Electronics Deposition</h2>
    <div class="artifact-line">
      <span><strong>Problem:</strong> Nonuniform deposition limits scalable printed electronics assembly.</span>
      <span><strong>System:</strong> IPA droplet + porous substrate + suspended microdevices.</span>
      <span><strong>My role:</strong> Designed experiments, captured top/side-view droplet videos, compared substrate boundary conditions, and developed process-window metrics.</span>
      <span><strong>Constraints:</strong> Microscopy geometry, droplet reproducibility, substrate heterogeneity, and confidentiality around lab visuals.</span>
      <span><strong>Methods:</strong> Optical microscopy, droplet tracking, contact-line dynamics, image analysis, substrate comparison.</span>
      <span><strong>Tools:</strong> Keyence · Python · ImageJ/Fiji · JMP.</span>
      <span><strong>Engineering output:</strong> Process-window metrics and substrate-selection logic for more uniform deposition.</span>
    </div>
    <div class="badge-row"><span class="badge">STATUS: In progress</span><span class="badge">TYPE: Research</span></div>
    <p><a href="{{ '/projects/micromodular-deposition/' | relative_url }}">Open full case study →</a></p>
  </article>

  <article class="portfolio-card">
    <div class="card-visual visual-pfd" aria-hidden="true"></div>
    <p class="tag">Process Engineering · Simulation · Design</p>
    <h2>Process Simulation and Design</h2>
    <div class="artifact-line">
      <span><strong>Problem:</strong> Convert process requirements into flowsheets, balances, and defensible design decisions.</span>
      <span><strong>System:</strong> Chemical process units, separations, recycle logic, and thermodynamic models.</span>
      <span><strong>My role:</strong> Built process logic, performed calculations, and evaluated engineering tradeoffs.</span>
      <span><strong>Constraints:</strong> Model selection, material/energy balance closure, and realistic operating conditions.</span>
      <span><strong>Methods:</strong> PFDs, mass/energy balances, VLE reasoning, Aspen simulation, design comparison.</span>
      <span><strong>Tools:</strong> Aspen · MATLAB · Excel.</span>
      <span><strong>Engineering output:</strong> Process models, flow diagrams, operating-condition comparisons, and technical calculations.</span>
    </div>
    <div class="badge-row"><span class="badge">STATUS: Buildout</span><span class="badge">TYPE: Coursework + independent</span></div>
  </article>

  <article class="portfolio-card">
    <div class="card-visual visual-signal" aria-hidden="true"></div>
    <p class="tag">Reliability · Experimental Analysis · Statistics</p>
    <h2>Printed Interconnect Reliability / Experimental Analysis</h2>
    <div class="artifact-line">
      <span><strong>Problem:</strong> Understand how printed interconnect resistance changes under stress and aging.</span>
      <span><strong>System:</strong> Printed Ag nanoparticle interconnects, resistance measurements, and environmental stress data.</span>
      <span><strong>My role:</strong> Organized experimental data, compared behavior across conditions, and interpreted statistical outputs.</span>
      <span><strong>Constraints:</strong> Limited sample sizes, drift, outliers, and separating measurement noise from real degradation.</span>
      <span><strong>Methods:</strong> Reliability plots, ANOVA-style comparisons, trend analysis, and engineering interpretation.</span>
      <span><strong>Tools:</strong> JMP · Excel · Python.</span>
      <span><strong>Engineering output:</strong> Stress-response summaries and process/reliability interpretation.</span>
    </div>
    <div class="badge-row"><span class="badge">STATUS: Framework developing</span><span class="badge">TYPE: Data analysis</span></div>
  </article>

  <article class="portfolio-card">
    <div class="card-visual visual-compute" aria-hidden="true"></div>
    <p class="tag">Computation · Image Analysis · Experimental Workflows</p>
    <h2>Image Analysis / Technical Computation</h2>
    <div class="artifact-line">
      <span><strong>Problem:</strong> Extract quantitative engineering variables from videos, microscopy images, and experimental time series.</span>
      <span><strong>System:</strong> Droplet videos, deposition images, time-dependent radius/contact-angle/volume measurements.</span>
      <span><strong>My role:</strong> Built and tested analysis workflows for segmentation, tracking, plotting, and interpretation.</span>
      <span><strong>Constraints:</strong> Low contrast, scale calibration, variable lighting, and noisy boundaries.</span>
      <span><strong>Methods:</strong> Segmentation, time-series extraction, curve plotting, and validation against baseline observations.</span>
      <span><strong>Tools:</strong> Python · ImageJ/Fiji · MATLAB.</span>
      <span><strong>Engineering output:</strong> Measurement workflows for r(t), θ(t), V(t), and deposition distributions.</span>
    </div>
    <div class="badge-row"><span class="badge">STATUS: In progress</span><span class="badge">TYPE: Computation</span></div>
  </article>
</div>
