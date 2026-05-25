---
layout: page
title: Build Logs
category: Projects
subtitle: "Real systems I measured, tuned, automated, or ran under pressure: printed electronics, stem-cell microencapsulation, reliability, thermal control, operations, and process computation."
body_class: projects-page
---

<section class="projects-index-hero startup-projects-hero" aria-label="Projects introduction">
 <p class="system-label small">PROJECTS</p>
 <h1>Build Logs</h1>
 <p>Four or five projects should be enough to tell whether I can think through a physical system. These are the ones I would talk about first.</p>
</section>

<section class="project-equal-grid-section" aria-label="Main projects">
 <div class="portfolio-grid startup-project-grid equal-project-grid">
 <article class="portfolio-card evidence-card build-log-card primary-build">
  <div class="card-topline"><span>Wet processing · Printed electronics</span><span>2025–present</span></div>
  <h2>Micromodular Electronics Deposition</h2>
  <p class="problem-line">Microdevices printed from droplets crowd at the edges; I built the measurement workflow for identifying substrate conditions that produce useful placement.</p>
  <div class="evidence-table compact-evidence-table">
   <span><strong>Output</strong> Substrate-screening decision framework based on contact-line motion, edge/center ratio, density, and repeatability.</span>
   <span><strong>Tools</strong> Keyence · Rame-Hart · Python · ImageJ/Fiji · JMP · optical microscopy.</span>
  </div>
  <p><a href="{{ '/projects/micromodular-deposition/' | relative_url }}">Open build log →</a></p>
 </article>

 <article class="portfolio-card evidence-card build-log-card operations-build">
  <div class="card-topline"><span>Operations · Quality loops</span><span class="metric-pill-strong">110 cars/hr peak</span></div>
  <h2>Operations &amp; Quality Systems</h2>
  <p class="problem-line">I managed live high-throughput systems where bottlenecks, staffing, QC, and downtime showed up immediately.</p>
  <div class="evidence-table compact-evidence-table">
   <span><strong>Outcomes</strong> +20% cars/hour, -15% order-to-handoff time, and ~30% downtime reduction.</span>
   <span><strong>Transfer</strong> Bottleneck recognition, standard work, QC discipline, and corrective action under pressure.</span>
  </div>
  <p><a href="{{ '/projects/operations-quality-systems/' | relative_url }}">Open build log →</a></p>
 </article>

 <article class="portfolio-card evidence-card build-log-card">
  <div class="card-topline"><span>Microfluidics · Biotech process dev</span><span class="metric-pill-strong">20× throughput</span></div>
  <h2>Stem-Cell Microencapsulation</h2>
  <p class="problem-line">Flow-focused core-shell capsule fabrication tuned around flow ratio, crosslink dwell time, coalescence, and microscopy QC.</p>
  <div class="evidence-table compact-evidence-table">
   <span><strong>Outcomes</strong> 20× throughput increase and ~50% encapsulation-yield improvement.</span>
   <span><strong>Method</strong> Flow-ratio tuning, crosslinking adjustment, and capsule-quality inspection.</span>
  </div>
  <p><a href="{{ '/projects/microencapsulation-process-development/' | relative_url }}">Open build log →</a></p>
 </article>

 <article class="portfolio-card evidence-card build-log-card">
  <div class="card-topline"><span>Reliability · Process control</span><span>Resistance drift</span></div>
  <h2>Printed Interconnect Reliability</h2>
  <p class="problem-line">Electrical drift and pass/fail behavior became a feedback loop for printed micromodular circuits.</p>
  <div class="evidence-table compact-evidence-table">
   <span><strong>Signal</strong> Initial R, R/R₀ drift, intermittent opens, and stress response.</span>
   <span><strong>Output</strong> Go/no-go threshold logic and process-step failure candidates.</span>
  </div>
  <p><a href="{{ '/projects/printed-interconnect-reliability/' | relative_url }}">Open build log →</a></p>
 </article>

 <article class="portfolio-card evidence-card build-log-card">
  <div class="card-topline"><span>Automation · Diagnostics</span><span>Setpoint tracking</span></div>
  <h2>Thermocycler Automation</h2>
  <p class="problem-line">A biological protocol became a controlled temperature-time process with ramp rate, overshoot, hold stability, and thermal lag as the real constraints.</p>
  <div class="evidence-table compact-evidence-table">
   <span><strong>Controlled outputs</strong> Ramp rate, settling time, overshoot, steady-state error, and repeatability.</span>
   <span><strong>Tools</strong> ESP32/Arduino · PID control · temperature sensors · RT-qPCR workflow logic.</span>
  </div>
  <p><a href="{{ '/projects/thermocycler-process-automation/' | relative_url }}">Open build log →</a></p>
 </article>
 </div>
</section>

<section class="additional-work-section compact-additional-section" aria-label="Additional technical work">
 <div class="supporting-proof-header section-header-tight">
 <strong>Additional technical work</strong>
 <span>Smaller proof points that add materials, assay, image-analysis, and process-design context.</span>
 </div>

 <div class="additional-evidence-strip five-evidence-strip">
 <a class="evidence-strip-item" href="{{ '/projects/droplet-image-analysis-workflows/' | relative_url }}"><strong>Droplet image analysis</strong><span>Video → segmentation → calibration → process metrics</span></a>
 <a class="evidence-strip-item" href="{{ '/projects/process-simulation-design/' | relative_url }}"><strong>Process simulation/design</strong><span>PFDs · balances · Aspen/MATLAB tradeoff logic</span></a>
 <a class="evidence-strip-item" href="{{ '/projects/thin-film-semiconductor-research/' | relative_url }}"><strong>Thin-film semiconductor growth</strong><span>MBE · SEM/XRD/XPS/Raman characterization matrix</span></a>
 <a class="evidence-strip-item" href="{{ '/projects/dna-pcr-flexibility/' | relative_url }}"><strong>DNA/PCR assay development</strong><span>Maher Lab, Mayo Clinic · assay workflow and controls</span></a>
 </div>
</section>

<section class="cta-band project-page-contact-cta" aria-label="Project contact call to action">
 <div>
  <p class="system-label small">OPEN THREAD</p>
  <h2>Want to talk through one of these builds?</h2>
  <p>I can go deeper on the experiments, constraints, tooling, and what I would change in a next version.</p>
 </div>
 <div class="cta-row compact-cta">
  <a class="button primary" href="mailto:{{ site.email }}">Email Nathan</a>
  <a class="button secondary" href="{{ '/assets/files/Nathan_Anderson_Resume.pdf' | relative_url }}" download="Nathan_Anderson_Resume.pdf">Resume</a>
 </div>
</section>
