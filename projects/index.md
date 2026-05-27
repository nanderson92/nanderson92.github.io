---
layout: page
title: Engineering Case Files
category: Engineering Case Files
subtitle: Build logs from real systems I measured, tuned, automated, or ran under pressure.
description: Engineering case files for wet processing, microfluidics, printed electronics reliability, automation, materials, and image-analysis workflows.
body_class: projects-page
---

<section class="projects-index-hero startup-projects-hero plain-prose-section" aria-label="Projects introduction">
 <p>Each case file follows the same proof logic: system, variables, <abbr title="Critical-to-Quality">CTQ</abbr>, screen, result, and next iteration.</p>
 <div class="case-filter-bar" aria-label="Filter case files">
  <button type="button" class="filter-chip is-active" data-filter="all">All</button>
  <button type="button" class="filter-chip" data-filter="wet">Wet processing</button>
  <button type="button" class="filter-chip" data-filter="microfluidics">Microfluidics</button>
  <button type="button" class="filter-chip" data-filter="reliability">Reliability</button>
  <button type="button" class="filter-chip" data-filter="automation">Automation</button>
  <button type="button" class="filter-chip" data-filter="materials">Materials</button>
 </div>
</section>

<section class="case-group flagship-group" aria-label="Featured case files">
 <div class="case-heading"><h2>Featured case files</h2></div>
 <div class="portfolio-grid startup-project-grid equal-project-grid casefile-project-grid">
  <article class="portfolio-card evidence-card build-log-card primary-build" data-tags="wet materials">
   <img class="case-thumb" src="{{ '/assets/images/artifact-measurement-plot.svg' | relative_url }}" alt="Droplet metric thumbnail" loading="lazy">
   <div class="card-topline"><span>Wet processing · printed electronics · Filler Lab · Georgia Tech · 2025–present</span><span class="outcome-badge">Screening framework</span></div>
   <h2>Micromodular Electronics Deposition</h2>
   <p class="metric-callout">What this proved: final stains were not enough. Video-derived contact-line traces gave the screen a real control variable.</p>
   <p class="transferable-line"><strong>Skill carried forward:</strong> substrate-screening and image-derived <abbr title="Critical-to-Quality">CTQs</abbr>.</p>
   <p><a href="{{ '/projects/micromodular-deposition/' | relative_url }}">Open case file →</a></p>
  </article>
  <article class="portfolio-card evidence-card build-log-card primary-build" data-tags="microfluidics">
   <img class="case-thumb" src="{{ '/assets/images/artifact-device-image.svg' | relative_url }}" alt="Capsule image thumbnail" loading="lazy">
   <div class="card-topline"><span>Microfluidics · Mayo Clinic · Rochester, MN · Summer 2025</span><span class="outcome-badge">20× throughput</span></div>
   <h2>Stem-Cell Microencapsulation</h2>
   <p class="metric-callout">What this proved: throughput only counted when flow ratio, tooling, and crosslink timing kept capsules usable.</p>
   <p class="transferable-line"><strong>Skill carried forward:</strong> throughput/yield operating-window development.</p>
   <p><a href="{{ '/projects/microencapsulation-process-development/' | relative_url }}">Open case file →</a></p>
  </article>
 </div>
</section>

<section class="case-group" aria-label="Reliability and control">
 <div class="case-heading"><h2>Reliability &amp; control</h2></div>
 <div class="portfolio-grid startup-project-grid equal-project-grid casefile-project-grid">
  <article class="portfolio-card evidence-card build-log-card" data-tags="reliability wet">
   <img class="case-thumb" src="{{ '/assets/images/reliability-drift-plot.svg' | relative_url }}" alt="Reliability plot thumbnail" loading="lazy">
   <div class="card-topline"><span>Reliability · printed electronics · Filler Lab · Georgia Tech · 2025–present</span><span class="outcome-badge">Failure logic</span></div>
   <h2>Printed Interconnect Reliability</h2>
   <p class="metric-callout">What this proved: a line can pass time-zero continuity and still show process-built vulnerability under stress.</p>
   <p class="transferable-line"><strong>Skill carried forward:</strong> failure classification and process-feedback logic.</p>
   <p><a href="{{ '/projects/printed-interconnect-reliability/' | relative_url }}">Open case file →</a></p>
  </article>
  <article class="portfolio-card evidence-card build-log-card" data-tags="automation">
   <img class="case-thumb" src="{{ '/assets/images/thermocycler-profile.svg' | relative_url }}" alt="Thermal control thumbnail" loading="lazy">
   <div class="card-topline"><span>Automation · Mayo Clinic · Rochester, MN · Summer 2025</span><span class="outcome-badge">Control prototype</span></div>
   <h2>Thermocycler Process Automation</h2>
   <p class="metric-callout">What this proved: a setpoint is not validation unless the sample region sees the intended thermal history.</p>
   <p class="transferable-line"><strong>Skill carried forward:</strong> thermal-control validation.</p>
   <p><a href="{{ '/projects/thermocycler-process-automation/' | relative_url }}">Open case file →</a></p>
  </article>
 </div>
</section>

<section class="case-group supporting-group" aria-label="Materials and workflows">
 <div class="case-heading"><h2>Materials and workflows</h2></div>
 <div class="portfolio-grid startup-project-grid equal-project-grid casefile-project-grid support-case-grid">
  <article class="portfolio-card evidence-card build-log-card" data-tags="materials">
   <img class="case-thumb" src="{{ '/assets/images/thin-film-characterization-visual.svg' | relative_url }}" alt="Materials characterization thumbnail" loading="lazy">
   <div class="card-topline"><span>Materials · semiconductors · Georgia Tech · 2025–present</span><span class="outcome-badge">Process response</span></div>
   <h2>Semiconductor Materials Exposure</h2>
   <p class="metric-callout">What this proved: characterization has to answer a process question, not just produce a pretty readout.</p>
   <p class="transferable-line"><strong>Skill carried forward:</strong> linking process conditions to material response.</p>
   <p><a href="{{ '/projects/thin-film-semiconductor-research/' | relative_url }}">Open case file →</a></p>
  </article>
  <article class="portfolio-card evidence-card build-log-card" data-tags="wet automation">
   <img class="case-thumb" src="{{ '/assets/images/artifact-flow-schematic.svg' | relative_url }}" alt="Image workflow thumbnail" loading="lazy">
   <div class="card-topline"><span>Image analysis · droplet metrics · Filler Lab · Georgia Tech · 2025–present</span><span class="outcome-badge">Video → CTQ</span></div>
   <h2>Droplet Image Analysis Workflows</h2>
   <p class="metric-callout">What this proved: raw microscopy videos become useful only after calibration, segmentation, and trace QC.</p>
   <p class="transferable-line"><strong>Skill carried forward:</strong> video-to-metric workflow design.</p>
   <p><a href="{{ '/projects/droplet-image-analysis-workflows/' | relative_url }}">Open case file →</a></p>
  </article>
  <article class="portfolio-card evidence-card build-log-card" data-tags="materials automation">
   <img class="case-thumb" src="{{ '/assets/images/artifact-simulation-flow.svg' | relative_url }}" alt="Simulation schematic thumbnail" loading="lazy">
   <div class="card-topline"><span>Simulation · balances · Georgia Tech · 2025–present</span><span class="outcome-badge">Flowsheet logic</span></div>
   <h2>Process Simulation and Design</h2>
   <p class="metric-callout">What this proved: a model is useful only when basis, assumptions, and decision use are explicit.</p>
   <p class="transferable-line"><strong>Skill carried forward:</strong> simulation-backed decision framing.</p>
   <p><a href="{{ '/projects/process-simulation-design/' | relative_url }}">Open case file →</a></p>
  </article>
  <article class="portfolio-card evidence-card build-log-card currently-working-card" data-tags="reliability">
   <div class="card-topline"><span>Currently working on</span><span class="outcome-badge">Next notes</span></div>
   <h2>Printed-Line Control-Plan Draft</h2>
   <p class="metric-callout">This is a working update slot for converting interconnect failure classes into a compact control-plan outline.</p>
   <p class="transferable-line"><strong>Follow-up:</strong> email me for the current draft or check future notes.</p>
   <p><a href="{{ '/notes/' | relative_url }}">See thinking notes →</a></p>
  </article>
 </div>
</section>

<section class="cta-band project-page-contact-cta tone-dark" aria-label="Project contact call to action">
 <div><h2>Talk through a case file with me.</h2><p>Internships, project work, startup conversations, or technical discussions. Happy to walk through the experiments, tooling, and what I’d change next.</p></div>
 <div class="cta-row compact-cta"><a class="button primary email-button" href="mailto:{{ site.email }}">Email Nathan →</a><a class="button secondary" href="{{ '/assets/files/Nathan_Anderson_Resume.pdf' | relative_url }}" download="Nathan_Anderson_Resume.pdf">Resume PDF</a></div>
</section>
