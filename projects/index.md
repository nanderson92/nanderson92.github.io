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
 <p class="build-log-definition">A build log is my record of a real system: the bottleneck, the variables I changed, the result I could measure, and what I would change in the next version. These are not résumé bullets stretched into pages; they are proof of the work habits I would bring into a hard-tech team.</p>
</section>

<section class="project-equal-grid-section" aria-label="Main projects">
 <div class="portfolio-grid startup-project-grid equal-project-grid">
 <article class="portfolio-card evidence-card build-log-card primary-build">
  <div class="card-topline"><span>Filler Lab · Georgia Tech</span><span>Screening framework</span></div>
  <h2>Droplet Deposition Screening</h2>
  <p class="problem-line">Microdevices printed from droplets crowd at the edges. I built the measurement workflow for identifying substrate conditions that produce useful placement.</p>
  <div class="evidence-table compact-evidence-table">
   <span><strong>Result</strong> Substrate-screening decision framework based on contact-line motion, edge/center ratio, density, and repeatability.</span>
   <span><strong>Tools</strong> Keyence · Rame-Hart · Python · ImageJ/Fiji · JMP · optical microscopy.</span>
  </div>
  <p><a href="{{ '/projects/micromodular-deposition/' | relative_url }}">Open build log →</a></p>
 </article>

 <article class="portfolio-card evidence-card build-log-card operations-build">
  <div class="card-topline"><span>High-volume operations</span><span class="metric-pill-strong">110 cars/hr peak</span></div>
  <h2>Drive-Through Operations</h2>
  <p class="problem-line">Managed live high-throughput systems where bottlenecks, staffing, QC, and downtime showed up immediately.</p>
  <div class="evidence-table compact-evidence-table">
   <span><strong>Result</strong> Documented +20% cars/hour, -15% order-to-handoff time, and ~30% downtime reduction from peak-shift observations and operating changes.</span>
   <span><strong>Tools</strong> Line balancing · shift control · QC logs · training · preventive maintenance.</span>
  </div>
  <p><a href="{{ '/projects/operations-quality-systems/' | relative_url }}">Open build log →</a></p>
 </article>

 <article class="portfolio-card evidence-card build-log-card">
  <div class="card-topline"><span>Mayo Clinic</span><span class="metric-pill-strong">20× throughput</span></div>
  <h2>Stem-Cell Microencapsulation</h2>
  <p class="problem-line">A flow-focused core-shell process tuned around flow ratio, crosslink dwell time, coalescence, and microscopy QC.</p>
  <div class="evidence-table compact-evidence-table">
   <span><strong>Result</strong> 20× throughput increase and ~50% encapsulation-yield improvement.</span>
   <span><strong>Tools</strong> Microfluidics · PEG/alginate · microscopy · capsule counting · flow-ratio tuning.</span>
  </div>
  <p><a href="{{ '/projects/microencapsulation-process-development/' | relative_url }}">Open build log →</a></p>
 </article>

 <article class="portfolio-card evidence-card build-log-card">
  <div class="card-topline"><span>Filler Lab · reliability</span><span>Failure taxonomy</span></div>
  <h2>Printed Interconnect Reliability</h2>
  <p class="problem-line">Printed conductive lines can look fine on day one and fail later. I turned those failures into threshold logic.</p>
  <div class="evidence-table compact-evidence-table">
   <span><strong>Result</strong> Go/no-go failure classes that point back to process-step candidates.</span>
   <span><strong>Tools</strong> Resistance testing · four-point probe · Keithley · Python · JMP · stress screening.</span>
  </div>
  <p><a href="{{ '/projects/printed-interconnect-reliability/' | relative_url }}">Open build log →</a></p>
 </article>

 <article class="portfolio-card evidence-card build-log-card">
  <div class="card-topline"><span>Automation · diagnostics</span><span>Setpoint tracking</span></div>
  <h2>Thermocycler Control</h2>
  <p class="problem-line">A biological protocol became a controlled temperature-time process with ramp rate, overshoot, hold stability, and thermal lag as the constraints.</p>
  <div class="evidence-table compact-evidence-table">
   <span><strong>Result</strong> Control prototype organized around ramp rate, settling time, overshoot, steady-state error, and repeatability.</span>
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
 <a class="evidence-strip-item" href="{{ '/projects/dna-pcr-flexibility/' | relative_url }}"><strong>DNA Flexibility Assay</strong><span>Maher Lab, Mayo Clinic · assay workflow and controls</span></a>
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
