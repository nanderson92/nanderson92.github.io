---
layout: page
title: Thin-Film Semiconductor Research
category: Materials · semiconductors · Georgia Tech
date_range: 2025–present
last_updated: May 2026
metric_chips: '<span>Process response</span><span>Characterization matrix</span>'
description: Semiconductor materials case file connecting deposition variables to characterization readouts and film-response decisions.
subtitle: Materials work connecting deposition conditions to morphology, phase, composition, and structural readouts.
body_class: case-file-page
---

<section class="artifact-panel setup-snapshot">
 <h2>Setup</h2>
 <ul class="snapshot-list">
  <li><strong>System:</strong> thin-film and semiconductor-materials work where deposition conditions are tied to characterization readouts.</li>
  <li><strong>Inputs handled:</strong> growth condition, substrate state, film morphology, phase/composition signals, and process comparison.</li>
  <li><strong>Outputs:</strong> a characterization matrix that separates what each tool can show from what it cannot prove alone.</li>
 </ul>
</section>
<section class="acronym-legend">
 <strong>Notation:</strong> <span><abbr title="scanning electron microscopy">SEM</abbr> = morphology/coverage imaging.</span> <span><abbr title="X-ray diffraction">XRD</abbr> = crystallinity and phase readout.</span> <span><abbr title="X-ray photoelectron spectroscopy">XPS</abbr> = surface chemistry readout.</span>
</section>

<section class="artifact-card artifact-card-wide hero-artifact">
 <p class="artifact-label">CHARACTERIZATION LOGIC</p>
 <figure class="artifact-figure">
  <div class="artifact-image-frame frame-schematic"><img src="{{ '/assets/images/thin-film-characterization-visual.svg' | relative_url }}" alt="Thin-film characterization logic visual" loading="lazy"></div>
  <figcaption><strong>Figure 1. Characterization as a process screen.</strong> A growth condition becomes actionable only when paired with a measurable film response and a decision about the next run.</figcaption>
 </figure>
</section>

<section class="insight-block tone-dark"><p>Characterization is useful when each readout answers a process question: morphology, composition, structure, or whether the growth condition should change.</p></section>

<section class="mini-flow-card"><h2>Materials screen flow</h2><div class="mini-flow"><span>Growth condition</span><b>→</b><span>Film response</span><b>→</b><span>Characterization</span><b>→</b><span>Pass/fail readout</span><b>→</b><span>Next run</span></div></section>

## Characterization matrix

<div class="artifact-table-wrap"><table class="artifact-table"><thead><tr><th>Readout</th><th>What it can show</th><th>What it cannot prove alone</th></tr></thead><tbody>
<tr><td><abbr title="scanning electron microscopy">SEM</abbr> / optical</td><td>Morphology, coverage, defects, gross film quality.</td><td>Composition or phase identity by itself.</td></tr>
<tr><td><abbr title="X-ray diffraction">XRD</abbr></td><td>Crystallinity, phase, orientation signals.</td><td>Local surface chemistry or point defects.</td></tr>
<tr><td><abbr title="X-ray photoelectron spectroscopy">XPS</abbr></td><td>Surface composition and chemical states.</td><td>Bulk structure without depth context.</td></tr>
<tr><td>Raman</td><td>Vibrational signatures and structural indicators.</td><td>Full process causality without paired conditions.</td></tr>
</tbody></table></div>

## Next run

<div class="next-iteration-callout"><p>The next iteration should define a small characterization control plan for each deposition change: one morphology check, one structure/composition check, and one pass/fail criterion. The engineering decision is which film response justifies changing the growth condition.</p></div>

## What changed

<div class="what-changed-block changed-panel"><p>The work made characterization feel like a process screen: each readout answers one part of the film-quality question and needs a paired process condition to become actionable.</p></div>

<div class="case-cta-row two-button-cta">
 <a class="button primary" href="{{ '/projects/droplet-image-analysis-workflows/' | relative_url }}">Next: Droplet Image Analysis Workflows →</a>
 <a class="button secondary email-button" href="mailto:{{ site.email }}">Email Nathan</a>
</div>
