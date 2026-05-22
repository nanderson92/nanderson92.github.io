---
layout: page
title: Projects
category: Case File Library
subtitle: Engineering case files: process development, micro/nano manufacturing, reliability, automation, and operations systems.
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

<div class="section-note">
  <strong>Additional Technical Work</strong> — compact cards for earlier research and supporting methods. These add breadth without distracting from the four flagship case files.
</div>

<div class="portfolio-grid projects-library">
  <article class="portfolio-card evidence-card">
    <div class="card-visual visual-signal" aria-hidden="true"></div>
    <div class="card-topline"><span>Semiconductors · Thin Films</span><span>Status: Compact case</span></div>
    <h2>Thin Film Semiconductor Growth &amp; Characterization</h2>
    <p class="problem-line">MBE deposition and characterization of Se/In thin films for band-gap and device-relevant semiconductor research.</p>
    <div class="evidence-table">
      <span><strong>Method</strong> High-vacuum deposition, parameter optimization, and materials characterization.</span>
      <span class="output-row"><strong>Output</strong> Research summary focused on process parameters, crystal quality, and characterization evidence.</span>
      <span><strong>Tools</strong> MBE · SEM · XRD · XPS · Raman.</span>
    </div>
    <p><a href="{{ '/projects/thin-film-semiconductor-research/' | relative_url }}">Open compact case →</a></p>
  </article>

  <article class="portfolio-card evidence-card">
    <div class="card-visual visual-compute" aria-hidden="true"></div>
    <div class="card-topline"><span>Molecular Biology · Assay Development</span><span>Status: Earlier research</span></div>
    <h2>DNA/PCR Flexibility Assay Development</h2>
    <p class="problem-line">Experimental work measuring DNA flexibility at extremely short base-pair lengths.</p>
    <div class="evidence-table">
      <span><strong>Method</strong> PCR-based experimental development, molecular-biology workflow execution, and assay troubleshooting.</span>
      <span class="output-row"><strong>Output</strong> Earlier research case emphasizing experimental design, precision, and biological measurement discipline.</span>
      <span><strong>Tools</strong> PCR · gel/workflow methods · DNA assay development.</span>
    </div>
    <p><a href="{{ '/projects/dna-pcr-flexibility/' | relative_url }}">Open compact case →</a></p>
  </article>
</div>

<div class="section-note">
  <strong>Systems, Quality, and Strategy</strong> — transferable process instincts from operations leadership and client-facing consulting.
</div>

<div class="portfolio-grid projects-library">
  <article class="portfolio-card evidence-card">
    <div class="card-visual visual-pfd" aria-hidden="true"></div>
    <div class="card-topline"><span>Operations · Quality · Throughput</span><span>Status: Transferable proof</span></div>
    <h2>Operations &amp; Quality Systems</h2>
    <p class="problem-line">Food-service operations translated into manufacturing-relevant instincts: throughput, standard work, quality logs, and corrective action.</p>
    <div class="evidence-table">
      <span><strong>Problem</strong> High-volume operations fail when bottlenecks, quality checks, maintenance, and training are not controlled.</span>
      <span><strong>Method</strong> Line balancing, queue analysis, CCP logs, shift training, corrective actions, and preventive-maintenance routines.</span>
      <span class="output-row"><strong>Output</strong> Quantified throughput, handoff-time, compliance, downtime, and maintenance improvements across leadership roles.</span>
      <span><strong>Places</strong> McDonald’s · Chick-fil-A · Flapdoodles.</span>
    </div>
    <p><a href="{{ '/projects/operations-quality-systems/' | relative_url }}">Open systems summary →</a></p>
  </article>

  <article class="portfolio-card evidence-card">
    <div class="card-visual visual-pfd" aria-hidden="true"></div>
    <div class="card-topline"><span>Consulting · Strategy · Communication</span><span>Status: Compact case</span></div>
    <h2>Consult Your Community: Nonprofit Growth Strategy</h2>
    <p class="problem-line">Pro-bono consulting for a local Atlanta nonprofit, focused on practical growth recommendations and client communication.</p>
    <div class="evidence-table">
      <span><strong>Problem</strong> Small organizations need actionable strategy that fits real bandwidth, constraints, and execution capacity.</span>
      <span><strong>Method</strong> Client discovery, market/communication analysis, recommendation synthesis, and slide-based delivery.</span>
      <span class="output-row"><strong>Output</strong> Growth and social-media recommendations translated into a client-facing implementation plan.</span>
      <span><strong>Tools</strong> PowerPoint · research · client interviews · communication strategy.</span>
    </div>
    <p><a href="{{ '/projects/consult-your-community/' | relative_url }}">Open compact case →</a></p>
  </article>
</div>
