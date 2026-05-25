---
layout: page
title: Build Logs
category: Projects
subtitle: Real systems I measured, tuned, automated, or ran under pressure.
body_class: projects-page
---

<section class="projects-index-hero startup-projects-hero" aria-label="Projects introduction">
 <p class="system-label small">PROJECTS</p>
 <h1>Build Logs</h1>
 <p>Real systems I measured, tuned, automated, or ran under pressure.</p>
</section>

<section class="project-equal-grid-section" aria-label="Main projects">
 <div class="portfolio-grid startup-project-grid equal-project-grid">
 <article class="portfolio-card evidence-card build-log-card primary-build">
  <div class="card-topline"><span>Wet processing · printed electronics</span><span>2025–present</span></div>
  <h2>Micromodular Electronics Deposition</h2>
  <p class="problem-line">Microdevices printed from droplets crowd at the edges. I built the measurement workflow for identifying substrate conditions that produce useful placement.</p>
  <div class="evidence-table compact-evidence-table">
   <span><strong>Output</strong> Substrate-screening decision framework based on contact-line motion, edge/center ratio, density, and repeatability.</span>
   <span><strong>Tools</strong> Keyence · Rame-Hart · Python · ImageJ/Fiji · JMP · optical microscopy.</span>
  </div>
  <p><a href="{{ '/projects/micromodular-deposition/' | relative_url }}">Open build log →</a></p>
 </article>

 <article class="portfolio-card evidence-card build-log-card operations-build">
  <div class="card-topline"><span>Operations · quality loops</span><span class="metric-pill-strong">110 cars/hr peak</span></div>
  <h2>Operations &amp; Quality Systems</h2>
  <p class="problem-line">I managed live high-throughput systems where bottlenecks, staffing, QC, and downtime showed up immediately.</p>
  <div class="evidence-table compact-evidence-table">
   <span><strong>Outcomes</strong> +20% cars/hour, -15% order-to-handoff time, and ~30% downtime reduction.</span>
   <span><strong>Transfer</strong> Bottleneck recognition, standard work, QC discipline, and corrective action under pressure.</span>
  </div>
  <p><a href="{{ '/projects/operations-quality-systems/' | relative_url }}">Open build log →</a></p>
 </article>

 <article class="portfolio-card evidence-card build-log-card">
  <div class="card-topline"><span>Microfluidics · biotech process dev</span><span class="metric-pill-strong">20× throughput</span></div>
  <h2>Stem-Cell Microcapsules</h2>
  <p class="problem-line">A flow-focused core-shell process tuned around flow ratio, crosslink dwell time, coalescence, and microscopy QC.</p>
  <div class="evidence-table compact-evidence-table">
   <span><strong>Outcomes</strong> 20× throughput increase and ~50% encapsulation-yield improvement.</span>
   <span><strong>Method</strong> Flow-ratio tuning, crosslinking adjustment, and capsule-quality inspection.</span>
  </div>
  <p><a href="{{ '/projects/microencapsulation-process-development/' | relative_url }}">Open build log →</a></p>
 </article>

 <article class="portfolio-card evidence-card build-log-card">
  <div class="card-topline"><span>Reliability · process control</span><span>Drift / open / intermittent</span></div>
  <h2>Printed Interconnect Reliability</h2>
  <p class="problem-line">Printed conductive lines can look fine on day one and fail later. I turned those failures into threshold logic.</p>
  <div class="evidence-table compact-evidence-table">
   <span><strong>Signal</strong> Initial R, R/R₀ drift, intermittent opens, and stress response.</span>
   <span><strong>Output</strong> Go/no-go failure classes that point back to process-step candidates.</span>
  </div>
  <p><a href="{{ '/projects/printed-interconnect-reliability/' | relative_url }}">Open build log →</a></p>
 </article>

 <article class="portfolio-card evidence-card build-log-card">
  <div class="card-topline"><span>Automation · diagnostics</span><span>Setpoint tracking</span></div>
  <h2>Thermocycler Automation</h2>
  <p class="problem-line">A biological protocol became a controlled temperature-time process with ramp rate, overshoot, hold stability, and thermal lag as the constraints.</p>
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
 <span>Shorter proof points that add assay and materials context without pretending every experience is a full project.</span>
 </div>
 <div class="additional-evidence-strip five-evidence-strip">
 <a class="evidence-strip-item" href="{{ '/projects/dna-pcr-flexibility/' | relative_url }}"><strong>DNA Flexibility — Assay Development</strong><span>Maher Lab, Mayo Clinic · assay workflow and controls</span></a>
 <span class="evidence-strip-item"><strong>Semiconductor materials exposure</strong><span>Working knowledge of MBE deposition and SEM/XRD/XPS/Raman characterization.</span></span>
 </div>
</section>

<section class="cta-band project-page-contact-cta" aria-label="Project contact call to action">
 <div>
  <h2>Want to talk through one of these builds?</h2>
  <p>I can go deeper on the experiments, constraints, tooling, and what I would change in a next version.</p>
 </div>
 <div class="cta-row compact-cta">
  <a class="button primary" href="mailto:{{ site.email }}">Email Nathan →</a>
  <a class="button secondary" href="{{ '/assets/files/Nathan_Anderson_Resume.pdf' | relative_url }}" download="Nathan_Anderson_Resume.pdf">Resume →</a>
 </div>
</section>
