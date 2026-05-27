---
layout: page
title: Semiconductor Materials Exposure
category: Materials · semiconductors · Georgia Tech
date_range: 2025–present
metric_chips: '<span>Process response</span><span>Characterization matrix</span>'
description: Semiconductor materials case file connecting deposition variables to characterization readouts and film-response decisions.
subtitle: Materials work connecting deposition conditions to morphology, phase, composition, and structural readouts.
body_class: case-file-page
---

<section class="artifact-panel setup-snapshot">
 <h2>The setup</h2>
 <ul class="snapshot-list">
  <li><strong>System:</strong> thin-film and semiconductor-materials work where deposition conditions are tied to characterization readouts.</li>
  <li><strong>Inputs handled:</strong> growth condition, substrate state, film morphology, phase/composition signals, and process comparison.</li>
  <li><strong>Outputs:</strong> a characterization matrix that separates what each tool can show from what it cannot prove alone.</li>
 </ul>
</section>
<section class="acronym-legend">
 <strong>Notation:</strong> <span><abbr title="Critical-to-Quality">CTQ</abbr> = measurable requirement the workflow has to deliver.</span> <span><abbr title="Design of Experiments">DOE</abbr> = structured run plan.</span> <span><abbr title="Failure Mode and Effects Analysis">FMEA</abbr> = failure-mode map used to prioritize checks.</span>
</section>



<section class="artifact-panel setup-snapshot"><h2>What good looks like</h2><p>Growth conditions become useful only when they can be connected to measurable film response. The case file frames deposition variables against characterization readouts without overclaiming what one tool can prove.</p></section>



<section class="insight-block tone-dark"><p>Characterization is useful when each readout answers a process question: morphology, composition, structure, or whether the growth condition should change.</p></section>

<section class="mini-flow-card"><h2>Materials screen flow</h2><div class="mini-flow"><span>Growth condition</span><b>→</b><span>Film response</span><b>→</b><span>Characterization</span><b>→</b><span>Pass/fail readout</span><b>→</b><span>Next run</span></div></section>

## What I'd do next

<div class="next-iteration-callout"><p>The next iteration should define a small characterization control plan for each deposition change: one morphology check, one structure/composition check, and one pass/fail criterion. The engineering decision is which film response justifies changing the growth condition.</p></div>

<section class="visual-artifact-grid" aria-label="Visual artifact slots">
 <figure><img src="{{ '/assets/images/artifact-materials-plot.svg' | relative_url }}" alt="Materials characterization plot area" loading="lazy"><figcaption>Add characterization trend, roughness, composition, or response comparison once data are cleared for display.</figcaption></figure>
 <figure><img src="{{ '/assets/images/thin-film-characterization-visual.svg' | relative_url }}" alt="Thin-film characterization visual" loading="lazy"><figcaption>Add film, substrate, SEM/optical, or characterization image once available.</figcaption></figure>
 <figure><img src="{{ '/assets/images/artifact-flow-schematic.svg' | relative_url }}" alt="Materials workflow schematic area" loading="lazy"><figcaption>Add deposition-condition → film-response → characterization workflow once the final analysis path is ready.</figcaption></figure>
</section>

<section class="artifact-link-slot">
 <strong>External artifact slot</strong>
 <span>Add poster, GitHub notebook, PDF memo, slide, or shareable writeup link when available.</span>
</section>


## Characterization matrix

<div class="artifact-table-wrap"><table class="artifact-table"><thead><tr><th>Readout</th><th>What it can show</th><th>What it cannot prove alone</th></tr></thead><tbody>
<tr><td>SEM / optical</td><td>Morphology, coverage, defects, gross film quality.</td><td>Composition or phase identity by itself.</td></tr>
<tr><td>XRD</td><td>Crystallinity, phase, orientation signals.</td><td>Local surface chemistry or point defects.</td></tr>
<tr><td>XPS</td><td>Surface composition and chemical states.</td><td>Bulk structure without depth context.</td></tr>
<tr><td>Raman</td><td>Vibrational signatures and structural indicators.</td><td>Full process causality without paired conditions.</td></tr>
</tbody></table></div>

## What this shifted

<div class="what-changed-block changed-panel"><p>The work made characterization feel like a process screen: each readout answers one part of the film-quality question and needs a paired process condition to become actionable.</p></div>


<div class="case-cta-row two-button-cta">
 <a class="button primary" href="{{ '/projects/droplet-image-analysis-workflows/' | relative_url }}">Next: Droplet Image Analysis Workflows →</a>
 <a class="button secondary email-button" href="mailto:{{ site.email }}">Email Nathan</a>
</div>
