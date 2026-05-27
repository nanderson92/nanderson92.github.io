---
layout: page
title: Thin-Film Semiconductor Research
category: Materials · semiconductors · Georgia Tech
date_range: 2025–present
last_updated: May 2026
prev_title: Thermocycler Process Automation
prev_url: /projects/thermocycler-process-automation/
next_title: Droplet Image Analysis Workflows
next_url: /projects/droplet-image-analysis-workflows/
metric_chips: '<span>Process response</span><span>Characterization matrix</span>'
description: Thin-film semiconductor research case file linking growth conditions to characterization readouts and process decisions.
subtitle: Materials-characterization framing for connecting growth conditions to film response without overclaiming a single readout.
body_class: case-file-page
---

<section class="artifact-stack materials-artifacts" aria-label="Thin-film semiconductor research artifacts">
 <article class="artifact-card artifact-card-wide hero-artifact">
  <p class="artifact-label">CHARACTERIZATION FRAME</p>
  <figure class="artifact-figure">
   <div class="artifact-image-frame frame-schematic"><img src="{{ '/assets/images/thin-film-characterization-visual.svg' | relative_url }}" alt="Thin-film characterization workflow visual" loading="lazy"></div>
   <figcaption><strong>Figure 1. Characterization-to-process frame.</strong> The useful output is not a standalone image or spectrum; it is a process readout that helps decide whether the growth condition should change.</figcaption>
  </figure>
 </article>
</section>

<section class="artifact-panel setup-snapshot">
 <h2>Setup</h2>
 <ul class="snapshot-list">
  <li><strong>System:</strong> thin-film semiconductor research where growth condition, substrate state, and characterization readout have to be interpreted together.</li>
  <li><strong>Inputs handled:</strong> growth condition, sample identity, processing history, characterization method, and comparison baseline.</li>
  <li><strong>Outputs:</strong> morphology/composition/structure readouts tied to whether a process condition should be changed.</li>
 </ul>
</section>
<section class="acronym-legend">
 <strong>Notation:</strong> <span><abbr title="Scanning Electron Microscopy">SEM</abbr> = morphology/coverage imaging.</span> <span><abbr title="X-ray Diffraction">XRD</abbr> = crystallinity/phase readout.</span> <span><abbr title="X-ray Photoelectron Spectroscopy">XPS</abbr> = surface composition/chemical-state readout.</span>
</section>

<section class="insight-block tone-dark"><p>Characterization is a process screen, not just a discovery tool. Each readout should answer whether the growth condition, substrate, or handling path needs to change.</p></section>

<section class="mini-flow-card"><h2>Materials screen flow</h2><div class="mini-flow"><span>Growth condition</span><b>→</b><span>Film response</span><b>→</b><span>Characterization</span><b>→</b><span>Pass/fail readout</span><b>→</b><span>Next run</span></div></section>

## Characterization matrix

<div class="artifact-table-wrap"><table class="artifact-table"><thead><tr><th>Readout</th><th>What it can show</th><th>What it cannot prove alone</th></tr></thead><tbody>
<tr><td><abbr title="Scanning Electron Microscopy">SEM</abbr> / optical</td><td>Morphology, coverage, defects, gross film quality.</td><td>Composition or phase identity by itself.</td></tr>
<tr><td><abbr title="X-ray Diffraction">XRD</abbr></td><td>Crystallinity, phase, orientation signals.</td><td>Local surface chemistry or point defects.</td></tr>
<tr><td><abbr title="X-ray Photoelectron Spectroscopy">XPS</abbr></td><td>Surface composition and chemical states.</td><td>Bulk structure without depth context.</td></tr>
<tr><td>Raman</td><td>Vibrational signatures and structural indicators.</td><td>Full process causality without paired conditions.</td></tr>
</tbody></table></div>

## Next run

<div class="next-iteration-callout"><p>The next iteration should define a small characterization control plan for each deposition change: one morphology check, one structure/composition check, and one pass/fail criterion. The engineering decision is which film response justifies changing the growth condition.</p></div>

## What changed

<div class="what-changed-block changed-panel"><p>The work made characterization feel like a process screen: each readout answers one part of the film-quality question and needs a paired process condition to become actionable.</p></div>

<div class="case-cta-row two-button-cta">
 <a class="button primary" href="{{ '/projects/droplet-image-analysis-workflows/' | relative_url }}">Next: Droplet Image Analysis Workflows →</a>
 <a class="button secondary email-button" href="mailto:{{ site.email }}?subject=Thin-film%20case%20file">Email Nathan</a>
</div>
