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
 <p class="build-log-definition">A build log is my record of a real system: the bottleneck, the variables I changed, the result I could measure, and what I would change in the next version. These are not resume bullets stretched into pages; they are the work habits I would bring into a hard-tech team.</p>
</section>

<section class="project-equal-grid-section" aria-label="Main projects">
 <div class="portfolio-grid startup-project-grid equal-project-grid six-card-grid">
 <article class="portfolio-card evidence-card build-log-card primary-build">
  <div class="card-topline"><span>Filler Lab · printed electronics</span><span>Screening framework</span></div>
  <h2>Droplet Deposition Screening</h2>
  <p class="problem-line">Microdevices printed from droplets crowd at the edges. I built the measurement workflow for identifying substrate conditions that produce useful placement.</p>
  <div class="evidence-table compact-evidence-table"><span><strong>Result</strong> Substrate-screening decision logic based on contact-line motion, edge/center ratio, density, and repeatability.</span></div>
  <p><a href="{{ '/projects/micromodular-deposition/' | relative_url }}">Open build log →</a></p>
 </article>

 <article class="portfolio-card evidence-card build-log-card operations-build">
  <div class="card-topline"><span>Operations · quality loops</span><span>Throughput discipline</span></div>
  <h2>Drive-Through Operations</h2>
  <p class="problem-line">I managed live high-throughput systems where bottlenecks, staffing, QC, and downtime showed up immediately.</p>
  <div class="evidence-table compact-evidence-table"><span><strong>Result</strong> Documented throughput, handoff-time, and downtime gains after prep-staging and maintenance changes.</span></div>
  <p><a href="{{ '/projects/operations-quality-systems/' | relative_url }}">Open build log →</a></p>
 </article>

 <article class="portfolio-card evidence-card build-log-card">
  <div class="card-topline"><span>Mayo Clinic · biotech process dev</span><span>Throughput 20×</span></div>
  <h2>Stem-Cell Microencapsulation</h2>
  <p class="problem-line">A flow-focused core-shell process tuned around flow ratio, crosslink dwell time, coalescence, and microscopy QC.</p>
  <div class="evidence-table compact-evidence-table"><span><strong>Result</strong> Throughput increased by 20× and usable encapsulation yield improved by roughly half within the tested workflow.</span></div>
  <p><a href="{{ '/projects/microencapsulation-process-development/' | relative_url }}">Open build log →</a></p>
 </article>

 <article class="portfolio-card evidence-card build-log-card">
  <div class="card-topline"><span>Reliability · process control</span><span>Failure logic</span></div>
  <h2>Printed Interconnect Reliability</h2>
  <p class="problem-line">Printed conductive lines can look fine on day one and fail later. I turned those failures into threshold logic.</p>
  <div class="evidence-table compact-evidence-table"><span><strong>Result</strong> Go/no-go failure classes that point back to candidate process steps.</span></div>
  <p><a href="{{ '/projects/printed-interconnect-reliability/' | relative_url }}">Open build log →</a></p>
 </article>

 <article class="portfolio-card evidence-card build-log-card">
  <div class="card-topline"><span>Automation · diagnostics</span><span>Control prototype</span></div>
  <h2>Thermocycler Control</h2>
  <p class="problem-line">A biological protocol became a controlled temperature-time process with ramp rate, overshoot, hold stability, and thermal lag as constraints.</p>
  <div class="evidence-table compact-evidence-table"><span><strong>Result</strong> A thermal-control prototype organized around ramp rate, settling time, overshoot, steady-state error, and repeatability.</span></div>
  <p><a href="{{ '/projects/thermocycler-process-automation/' | relative_url }}">Open build log →</a></p>
 </article>

 <article class="portfolio-card evidence-card build-log-card">
  <div class="card-topline"><span>Maher Lab · Mayo Clinic</span><span>Assay controls</span></div>
  <h2>DNA Flexibility Assay</h2>
  <p class="problem-line">Earlier molecular-biology research developing experimental habits around controls, troubleshooting, and small-signal readout discipline.</p>
  <div class="evidence-table compact-evidence-table"><span><strong>Result</strong> Assay workflow and control logic for probing DNA flexibility at short base-pair lengths.</span></div>
  <p><a href="{{ '/projects/dna-pcr-flexibility/' | relative_url }}">Open build log →</a></p>
 </article>
 </div>
</section>

<section class="additional-work-section compact-additional-section" aria-label="Additional technical work">
 <div class="supporting-proof-header section-header-tight">
 <strong>Additional technical work</strong>
 <span>Shorter proof points that add materials, simulation, and consulting context without pretending every experience is a full project.</span>
 </div>
 <div class="additional-evidence-strip centered-evidence-strip">
 <a class="evidence-strip-item" href="{{ '/projects/thin-film-semiconductor-research/' | relative_url }}"><strong>Semiconductor Materials Exposure</strong><span>MBE deposition context and SEM/XRD/XPS/Raman characterization literacy.</span></a>
 <a class="evidence-strip-item" href="{{ '/projects/consult-your-community/' | relative_url }}"><strong>Consult Your Community</strong><span>Scoped ambiguous goals into CTQs, KPIs, and a practical workplan.</span></a>
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
