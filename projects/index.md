---
layout: page
title: Projects
category: Case File Library
subtitle: Engineering case files: process development, micro/nano manufacturing, reliability, automation, and operations systems.
body_class: projects-page
---

<div class="portfolio-grid projects-library">
  <article class="portfolio-card feature-project evidence-card">
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

  <article class="portfolio-card evidence-card">
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

  <article class="portfolio-card evidence-card">
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

  <article class="portfolio-card evidence-card">
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


<section class="supporting-proof-band" aria-label="Additional technical work and operations proof">
  <div class="section-note compact-section-note">
    <strong>Supporting proof</strong> — earlier research, operations, and strategy work kept intentionally compact so the four flagship engineering case files stay dominant.
  </div>

  <div class="mini-case-grid">
    <a class="mini-case-card" href="{{ '/projects/thin-film-semiconductor-research/' | relative_url }}">
      <span class="mini-meta">Semiconductors · Thin Films</span>
      <strong>Thin Film Semiconductor Growth</strong>
      <p>MBE deposition and characterization of Se/In thin films; process-parameter logic, band-gap relevance, and materials evidence.</p>
      <em>MBE · SEM · XRD · XPS · Raman</em>
    </a>

    <a class="mini-case-card" href="{{ '/projects/dna-pcr-flexibility/' | relative_url }}">
      <span class="mini-meta">Molecular Biology · Assays</span>
      <strong>DNA/PCR Flexibility Assay Development</strong>
      <p>PCR-based experimental design for measuring very short-length DNA flexibility; precision workflow execution and troubleshooting.</p>
      <em>PCR · DNA assays · experimental design</em>
    </a>

    <a class="mini-case-card" href="{{ '/projects/operations-quality-systems/' | relative_url }}">
      <span class="mini-meta">Operations · Quality · Throughput</span>
      <strong>Operations &amp; Quality Systems</strong>
      <p>High-volume service operations translated into standard work, bottleneck control, CCP logs, corrective actions, and training routines.</p>
      <em>Throughput · QC logs · PM routines</em>
    </a>

    <a class="mini-case-card" href="{{ '/projects/consult-your-community/' | relative_url }}">
      <span class="mini-meta">Consulting · Strategy</span>
      <strong>Nonprofit Growth Strategy</strong>
      <p>Client discovery, market/communication analysis, and practical recommendations for a local Atlanta nonprofit’s execution capacity.</p>
      <em>Client discovery · strategy · delivery</em>
    </a>
  </div>
</section>

