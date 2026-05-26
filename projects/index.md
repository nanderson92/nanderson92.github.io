---
layout: page
title: Engineering Case Files
category: Projects
subtitle: Build logs from real systems I measured, tuned, automated, or ran under pressure.
body_class: projects-page
---

<section class="projects-index-hero startup-projects-hero" aria-label="Projects introduction">
 <p class="system-label small">Engineering Case Files</p>
 <p>Build logs from real systems I measured, tuned, automated, or ran under pressure.</p>
 <p class="build-log-definition">Each case file follows the same proof logic: system, CTQs, measured outputs, failure behavior, and the engineering decision that followed.</p>
 <div class="case-filter-bar" aria-label="Filter case files">
  <button class="filter-chip is-active" data-filter="all" type="button">All</button>
  <button class="filter-chip" data-filter="wet-processing" type="button">Wet processing</button>
  <button class="filter-chip" data-filter="microfluidics" type="button">Microfluidics</button>
  <button class="filter-chip" data-filter="reliability" type="button">Reliability</button>
  <button class="filter-chip" data-filter="automation" type="button">Automation</button>
  <button class="filter-chip" data-filter="materials" type="button">Materials</button>
 </div>
</section>

<section class="case-section flagship-case-section" aria-label="Flagship process development">
 <div class="section-heading compact-heading">
  <p class="system-label small">Flagship process development</p>
  <h2>Wet systems, yield, placement, and operating windows.</h2>
 </div>
 <div class="portfolio-grid startup-project-grid equal-project-grid casefile-project-grid">
 <article class="portfolio-card evidence-card build-log-card primary-build" data-tags="wet-processing materials">
  <img class="card-chip" src="{{ '/assets/images/chip-droplet.svg' | relative_url }}" alt="Droplet metric icon">
  <div class="card-topline"><span>Wet processing · printed electronics · 2025–present</span><span class="outcome-badge">Screening framework</span></div>
  <h2>Micromodular Electronics Deposition</h2>
  <p><strong>System:</strong> IPA droplet deposition of suspended microdevices on substrate/backing candidates.</p>
  <p><strong>Measured:</strong> contact-line traces, placement bias, repeatability, and interconnect-accessible density.</p>
  <p class="transferable-line"><strong>Skill carried forward:</strong> substrate-screening and image-derived CTQs.</p>
  <p><a href="{{ '/projects/micromodular-deposition/' | relative_url }}">Open case file →</a></p>
 </article>

 <article class="portfolio-card evidence-card build-log-card primary-build" data-tags="microfluidics">
  <img class="card-chip" src="{{ '/assets/images/chip-capsule.svg' | relative_url }}" alt="Capsule throughput icon">
  <div class="card-topline"><span>Microfluidics · Mayo Clinic · Rochester, MN · Summer 2025</span><span class="outcome-badge">20× throughput</span></div>
  <h2>Stem-Cell Microencapsulation</h2>
  <p><strong>System:</strong> flow-focusing core-shell capsule generation with crosslinking and microscopy QC.</p>
  <p><strong>Measured:</strong> usable capsule yield, generation rate, coalescence, capsule size, and run-to-run variability.</p>
  <p class="transferable-line"><strong>Skill carried forward:</strong> throughput/yield operating-window development.</p>
  <p><a href="{{ '/projects/microencapsulation-process-development/' | relative_url }}">Open case file →</a></p>
 </article>
 </div>
</section>

<section class="case-section" aria-label="Reliability and control">
 <div class="section-heading compact-heading">
  <p class="system-label small">Reliability &amp; control</p>
  <h2>Failure classes, validation loops, and automation.</h2>
 </div>
 <div class="portfolio-grid startup-project-grid equal-project-grid casefile-project-grid">
 <article class="portfolio-card evidence-card build-log-card" data-tags="reliability">
  <img class="card-chip" src="{{ '/assets/images/chip-reliability.svg' | relative_url }}" alt="Reliability trace icon">
  <div class="card-topline"><span>Reliability · process feedback · 2025–present</span><span class="outcome-badge">Failure logic</span></div>
  <h2>Printed Interconnect Reliability</h2>
  <p>Printed conductive lines can pass time-zero checks and fail later. Resistance behavior becomes a reliability screen when the trace is classified.</p>
  <p class="transferable-line"><strong>Skill carried forward:</strong> failure classification and upstream process-feedback logic.</p>
  <p><a href="{{ '/projects/printed-interconnect-reliability/' | relative_url }}">Open case file →</a></p>
 </article>

 <article class="portfolio-card evidence-card build-log-card" data-tags="automation">
  <img class="card-chip" src="{{ '/assets/images/chip-thermal.svg' | relative_url }}" alt="Thermal profile icon">
  <div class="card-topline"><span>Automation · diagnostics · Mayo Clinic · Rochester, MN · Summer 2025</span><span class="outcome-badge">Control prototype</span></div>
  <h2>Thermocycler Process Automation</h2>
  <p>A biological protocol became a temperature-time validation problem: ramp rate, overshoot, settling, hold stability, and repeatability.</p>
  <p class="transferable-line"><strong>Skill carried forward:</strong> thermal-control validation.</p>
  <p><a href="{{ '/projects/thermocycler-process-automation/' | relative_url }}">Open case file →</a></p>
 </article>
 </div>
</section>

<section class="case-section" aria-label="Operations and earlier research">
 <div class="section-heading compact-heading">
  <p class="system-label small">Operations &amp; earlier research</p>
  <h2>Materials context, image analysis, and modeling support.</h2>
 </div>
 <div class="portfolio-grid startup-project-grid equal-project-grid casefile-project-grid support-case-grid">
 <article class="portfolio-card evidence-card build-log-card support-build" data-tags="materials">
  <img class="card-chip" src="{{ '/assets/images/chip-materials.svg' | relative_url }}" alt="Materials characterization icon">
  <div class="card-topline"><span>Materials · characterization · Georgia Tech</span><span class="outcome-badge">Materials context</span></div>
  <h2>Semiconductor Materials Exposure</h2>
  <p>Working knowledge of MBE deposition, SEM/XRD/XPS/Raman characterization, surface roughness, Aspen Plus, MATLAB, JMP, and process-simulation framing.</p>
  <p class="transferable-line"><strong>Skill carried forward:</strong> linking process conditions to material response.</p>
  <p><a href="{{ '/projects/thin-film-semiconductor-research/' | relative_url }}">Open case file →</a></p>
 </article>

 <article class="portfolio-card evidence-card build-log-card support-build" data-tags="wet-processing">
  <img class="card-chip" src="{{ '/assets/images/chip-image-analysis.svg' | relative_url }}" alt="Image analysis icon">
  <div class="card-topline"><span>Image analysis · droplet CTQs · 2025–present</span><span class="outcome-badge">Metric extraction</span></div>
  <h2>Droplet Image Analysis Workflows</h2>
  <p>Video analysis converts droplet geometry, radial drift, and final placement into CTQs that can be compared across substrate screens.</p>
  <p class="transferable-line"><strong>Skill carried forward:</strong> extracting usable engineering variables from noisy videos.</p>
  <p><a href="{{ '/projects/droplet-image-analysis-workflows/' | relative_url }}">Open case file →</a></p>
 </article>

 <article class="portfolio-card evidence-card build-log-card support-build" data-tags="materials automation">
  <img class="card-chip" src="{{ '/assets/images/chip-simulation.svg' | relative_url }}" alt="Simulation icon">
  <div class="card-topline"><span>Simulation · design tools · Georgia Tech</span><span class="outcome-badge">Modeling discipline</span></div>
  <h2>Process Simulation &amp; Design</h2>
  <p>Aspen, MATLAB, Excel, and JMP support thermodynamics, screening tables, statistical comparison, and communication-ready engineering summaries.</p>
  <p class="transferable-line"><strong>Skill carried forward:</strong> turning calculations into decision support.</p>
  <p><a href="{{ '/projects/process-simulation-design/' | relative_url }}">Open case file →</a></p>
 </article>

 <article class="portfolio-card evidence-card build-log-card currently-card" data-tags="all">
  <div class="card-topline"><span>Currently working on</span><span class="outcome-badge">Notes in progress</span></div>
  <h2>Open technical notes</h2>
  <p>More public-safe build notes are being converted into case files as artifacts become shareable.</p>
  <p><a href="{{ site.linkedin }}">Follow updates on LinkedIn →</a></p>
 </article>
 </div>
</section>

<section class="cta-band project-page-contact-cta" aria-label="Project contact call to action">
 <div>
  <h2>Want to talk through one of these case files?</h2>
  <p>Happy to walk through the experiments, tooling, and what I'd change next.</p>
 </div>
 <div class="cta-row compact-cta">
  <a class="button primary email-button" href="mailto:{{ site.email }}">Email Nathan →</a>
  <a class="button secondary" href="{{ '/assets/files/Nathan_Anderson_Resume.pdf' | relative_url }}" download="Nathan_Anderson_Resume.pdf">Resume →</a>
 </div>
</section>

<script>
(function(){
 const chips = document.querySelectorAll('.filter-chip');
 const cards = document.querySelectorAll('[data-tags]');
 chips.forEach((chip) => chip.addEventListener('click', () => {
  chips.forEach((c) => c.classList.remove('is-active'));
  chip.classList.add('is-active');
  const filter = chip.dataset.filter;
  cards.forEach((card) => {
   const tags = (card.dataset.tags || '').split(/\s+/);
   const show = filter === 'all' || tags.includes(filter) || tags.includes('all');
   card.style.display = show ? '' : 'none';
  });
 }));
})();
</script>
