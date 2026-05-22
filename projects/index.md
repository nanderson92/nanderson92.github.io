---
layout: page
title: Projects
category: Case File Library
subtitle: Engineering case files: process development, micro/nano manufacturing, reliability, automation, and operations systems.
---

<div class="section-note">
  <strong>Projects = engineering proof-of-work.</strong> This page is organized as a case-file library: each project explains the problem, method, output, tools, and artifact status. The goal is not to list everything I have done; it is to show how I build, measure, troubleshoot, and improve technical systems.
</div>

<div class="filter-row" aria-label="Project filters">
  <span class="filter-chip active">All</span>
  <span class="filter-chip">Featured</span>
  <span class="filter-chip">Semiconductors</span>
  <span class="filter-chip">Microfluidics</span>
  <span class="filter-chip">Process Development</span>
  <span class="filter-chip">Reliability &amp; Quality</span>
  <span class="filter-chip">Automation &amp; Data</span>
  <span class="filter-chip">Strategy / Operations</span>
</div>

<div class="section-note">
  <strong>Featured Engineering Case Files</strong> — the four strongest technical stories I am currently building out with public-safe figures, recreated schematics, methods, metrics, and implementation notes.
</div>

<div class="portfolio-grid projects-library">
  <article id="process-development" class="portfolio-card feature-project evidence-card">
    <div class="card-visual visual-droplet" aria-hidden="true"></div>
    <div class="card-topline"><span>Featured · Semiconductors · Interfacial Transport</span><span>Status: Active buildout</span></div>
    <h2>Micromodular Electronics Deposition</h2>
    <p class="problem-line">Substrate-controlled process windows for stochastic microdevice placement.</p>
    <div class="evidence-table">
      <span><strong>Problem</strong> Suspended microdevices can accumulate nonuniformly during droplet spreading, drying, and imbibition, limiting scalable printed-electronics assembly.</span>
      <span><strong>Method</strong> AAO/substrate comparisons, top/side-view microscopy, droplet kinematics, contact-line analysis, deposition-density mapping, and Python tracking.</span>
      <span class="output-row"><strong>Output</strong> Process-window metrics, edge/center deposition logic, substrate-selection criteria, and a reusable public-safe analysis workflow.</span>
      <span><strong>Tools</strong> Keyence · Rame-Hart · Python · ImageJ/Fiji · JMP.</span>
      <span><strong>Status</strong> In progress; flagship case page includes recreated schematics and buildout targets.</span>
    </div>
    <p><a href="{{ '/projects/micromodular-deposition/' | relative_url }}">Open full case study →</a></p>
  </article>

  <article id="reliability-quality" class="portfolio-card evidence-card">
    <div class="card-visual visual-signal" aria-hidden="true"></div>
    <div class="card-topline"><span>Featured · Reliability · Process Control</span><span>Status: Active buildout</span></div>
    <h2>Printed Interconnect &amp; FET Reliability</h2>
    <p class="problem-line">Electrical test, resistance drift, yield visibility, and process-control loops for micromodular electronics.</p>
    <div class="evidence-table">
      <span><strong>Problem</strong> Printed interconnects and device interfaces can fail through resistance drift, intermittent opens, and process-step variability.</span>
      <span><strong>Method</strong> Keithley go/no-go screening, threshold limits, stress comparisons, failure-mode interpretation, JMP analysis, and process-step correlation.</span>
      <span class="output-row"><strong>Output</strong> Reliability plots, CTQ logic, screening pipeline notes, and process-window recommendations for tighter yield control.</span>
      <span><strong>Tools</strong> Keithley · Python · JMP · Excel · optical microscopy.</span>
      <span><strong>Status</strong> In progress; public-safe plots and process-control artifacts are being added.</span>
    </div>
    <p><a href="{{ '/projects/printed-interconnect-reliability/' | relative_url }}">Open full case study →</a></p>
  </article>

  <article id="microfluidics" class="portfolio-card evidence-card">
    <div class="card-visual visual-droplet" aria-hidden="true"></div>
    <div class="card-topline"><span>Featured · Microfluidics · Process Development</span><span>Status: New case file</span></div>
    <h2>Scalable Stem-Cell Microencapsulation</h2>
    <p class="problem-line">Flow-focused core–shell capsule process development for regenerative-medicine workflows.</p>
    <div class="evidence-table">
      <span><strong>Problem</strong> Complex hydrogel microcapsules need high throughput, low coalescence, and repeatable capsule quality without compromising biological utility.</span>
      <span><strong>Method</strong> Flow-ratio tuning, crosslink dwell-time optimization, PEG/alginate core–shell capsule fabrication, and microscopy-based QC.</span>
      <span class="output-row"><strong>Output</strong> Improved encapsulation yield, reduced coalescence, stable capsule-production conditions, and process-development notes.</span>
      <span><strong>Tools</strong> Microfluidics · microscopy · cell culture · flow control · image-based inspection.</span>
      <span><strong>Status</strong> New portfolio page; final visuals should use recreated device/capsule schematics.</span>
    </div>
    <p><a href="{{ '/projects/microencapsulation-process-development/' | relative_url }}">Open full case study →</a></p>
  </article>

  <article id="automation-data" class="portfolio-card evidence-card">
    <div class="card-visual visual-compute" aria-hidden="true"></div>
    <div class="card-topline"><span>Featured · Automation · Diagnostics</span><span>Status: New case file</span></div>
    <h2>Thermocycler Process Automation</h2>
    <p class="problem-line">PID-controlled thermal cycling hardware for rapid molecular-diagnostics workflows.</p>
    <div class="evidence-table">
      <span><strong>Problem</strong> RT-qPCR workflows require fast ramping, stable temperature holds, and repeatable automated thermal control.</span>
      <span><strong>Method</strong> Embedded controller prototyping, heater/cooling integration, sensor feedback, PID tuning, calibration, and repeatability checks.</span>
      <span class="output-row"><strong>Output</strong> Functional thermocycler prototype with quantified ramp rate and steady-state temperature stability.</span>
      <span><strong>Tools</strong> ESP32/Arduino · PID control · sensors · Python/microcontroller code · RT-qPCR workflow logic.</span>
      <span><strong>Status</strong> New portfolio page; add control-loop figure and thermal-profile plot.</span>
    </div>
    <p><a href="{{ '/projects/thermocycler-process-automation/' | relative_url }}">Open full case study →</a></p>
  </article>
</div>


<div id="process-simulation" class="skill-anchor" aria-label="Process simulation, PFDs, balances, Aspen, and MATLAB evidence"></div>

<section class="supporting-work" aria-labelledby="supporting-work-title">
  <div class="supporting-header">
    <p class="system-label">Supporting Work</p>
    <h2 id="supporting-work-title">Additional technical breadth</h2>
    <p>Earlier research and transfer-work examples kept intentionally compact so the four flagship engineering case files stay dominant.</p>
  </div>

  <div class="supporting-grid">
    <a class="supporting-card" href="{{ '/projects/thin-film-semiconductor-research/' | relative_url }}">
      <span class="supporting-tag">Thin films · Semiconductors</span>
      <strong>Thin Film Semiconductor Growth &amp; Characterization</strong>
      <p>MBE deposition and characterization work summarized as a compact materials-process case.</p>
    </a>

    <a class="supporting-card" href="{{ '/projects/dna-pcr-flexibility/' | relative_url }}">
      <span class="supporting-tag">Molecular biology · Assays</span>
      <strong>DNA/PCR Flexibility Assay Development</strong>
      <p>Earlier PCR-based experimental work emphasizing precision, measurement discipline, and troubleshooting.</p>
    </a>
  </div>
</section>

<section class="supporting-work muted-supporting" aria-labelledby="transfer-work-title">
  <div class="supporting-header small">
    <p class="system-label">Transferable Proof</p>
    <h2 id="transfer-work-title">Operations, quality, and client-facing work</h2>
    <p>Useful context, but secondary to the engineering case files above.</p>
  </div>

  <div class="supporting-list">
    <a href="{{ '/projects/operations-quality-systems/' | relative_url }}">
      <span>Operations · Quality · Throughput</span>
      <strong>Operations &amp; Quality Systems</strong>
      <p>Standard work, bottleneck control, training, logs, corrective action, and throughput instincts from high-volume operations.</p>
    </a>

    <a href="{{ '/projects/consult-your-community/' | relative_url }}">
      <span>Consulting · Strategy</span>
      <strong>Consult Your Community: Nonprofit Growth Strategy</strong>
      <p>Client discovery, recommendation synthesis, communication strategy, and implementation planning for a local nonprofit.</p>
    </a>
  </div>
</section>
