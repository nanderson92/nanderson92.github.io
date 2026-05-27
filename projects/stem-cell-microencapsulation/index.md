---
layout: page
title: Stem-Cell Microencapsulation
category: Microfluidics · Mayo Clinic · Rochester, MN
date_range: Summer 2025
metric_chips: '<span><strong>20×</strong> throughput increase</span><span><strong>~50%</strong> usable-yield improvement</span>'
subtitle: Microfluidic capsule-generation work that made throughput useful by keeping yield and handling stability inside the operating window.
meta_description: Case file on Mayo Clinic microfluidic stem-cell microencapsulation, 20x throughput, usable-yield improvement, and process levers.
---

<section class="artifact-panel setup-panel"><h2>The setup</h2><ul class="snapshot-list"><li><strong>System:</strong> flow-focusing microfluidic alginate-core / PEG-shell capsule generation for ARPE-19 cell culture.</li><li><strong>Inputs adjusted:</strong> flow ratio, tooling geometry, shielding/crosslinking conditions, and collection workflow.</li><li><strong>Outputs measured:</strong> capsule-generation rate, microscopy-counted usable yield, coalescence, shell integrity, and handling stability.</li><li><strong>Result:</strong> increased capsule-generation throughput by 20× and improved microscopy-counted usable encapsulation yield by ~50% after flow-ratio, tooling, and crosslinking adjustments.</li></ul></section>

<section class="insight-block dark-section"><p>Faster throughput was not automatically better. Speed only mattered when droplet formation, flow ratio, crosslink timing, and collection stayed inside the usable window.</p></section>

<section class="next-iteration-callout early-next"><h2>What I’d do next</h2><p>Convert yield categories into a control plan: acceptable capsule morphology, coalescence limit, collection timing, and microscopy sampling cadence. The decision is whether a faster run stays inside the usable-yield window without hiding new defect classes.</p></section>

<section class="visual-artifact-grid" aria-label="Artifact placeholders">
 <figure><img src="{{ '/assets/images/artifact-measurement-plot.svg' | relative_url }}" alt="Chart artifact placeholder" loading="lazy"><figcaption><strong>Artifact placeholder:</strong> replace with the real chart, graph, trace, or distribution.</figcaption></figure>
 <figure><img src="{{ '/assets/images/artifact-device-image.svg' | relative_url }}" alt="Lab or microscopy artifact placeholder" loading="lazy"><figcaption><strong>Artifact placeholder:</strong> replace with the real lab photo, microscopy still, device image, or run image.</figcaption></figure>
 <figure><img src="{{ '/assets/images/microfluidic-flow-schematic.svg' | relative_url }}" alt="Code, analysis, or process-flow artifact placeholder" loading="lazy"><figcaption><strong>Artifact placeholder:</strong> replace with code snippet, analysis workflow, control plan, or schematic.</figcaption></figure>
</section>

<h2>Process levers</h2>
<div class="artifact-table-wrap"><table class="artifact-table"><thead><tr><th>Process change</th><th>Failure mode addressed</th><th>Metric affected</th><th>Result</th></tr></thead><tbody><tr><td>Flow-ratio tuning</td><td>Unstable capsule formation / coalescence</td><td>Usable yield</td><td>~50% improvement</td></tr><tr><td>Tooling redesign</td><td>Low generation rate</td><td>Throughput</td><td>20× increase</td></tr><tr><td>Crosslink timing adjustment</td><td>Fragile shells / post-formation instability</td><td>Handling stability</td><td>Improved usable capsule fraction</td></tr><tr><td>Microscopy QC</td><td>Unclassified defects</td><td>Yield interpretation</td><td>Defect classes became visible</td></tr></tbody></table></div>
<p class="method-note"><strong>Yield definition:</strong> percent usable capsules after excluding coalesced, visibly defective, or handling-unstable capsules during microscopy QC.</p>

<section class="flow-diagram-card"><h2>Microencapsulation workflow</h2><svg class="flow-svg" viewBox="0 0 1000 230" role="img" aria-label="Microencapsulation workflow"><defs><marker id="arrow-cap" markerWidth="12" markerHeight="12" refX="10" refY="6" orient="auto"><path d="M0 0 L12 6 L0 12 Z" fill="#0d8eb1"/></marker></defs><g font-family="Inter, Arial"><rect x="40" y="60" width="190" height="100" rx="20" fill="#fff" stroke="#d8e2e7"/><text x="135" y="104" text-anchor="middle" font-size="21" font-weight="800" fill="#0f172a">Tune flows</text><text x="135" y="132" text-anchor="middle" font-size="15" fill="#64748b">ratio + rate</text><rect x="285" y="60" width="190" height="100" rx="20" fill="#fff" stroke="#d8e2e7"/><text x="380" y="104" text-anchor="middle" font-size="21" font-weight="800" fill="#0f172a">Form capsules</text><text x="380" y="132" text-anchor="middle" font-size="15" fill="#64748b">droplet regime</text><rect x="530" y="60" width="190" height="100" rx="20" fill="#fff" stroke="#d8e2e7"/><text x="625" y="104" text-anchor="middle" font-size="21" font-weight="800" fill="#0f172a">Crosslink</text><text x="625" y="132" text-anchor="middle" font-size="15" fill="#64748b">shell stability</text><rect x="775" y="60" width="190" height="100" rx="20" fill="#fff8ea" stroke="#f59e0b"/><text x="870" y="104" text-anchor="middle" font-size="21" font-weight="800" fill="#0f172a">QC</text><text x="870" y="132" text-anchor="middle" font-size="15" fill="#64748b">usable yield</text><line x1="230" y1="110" x2="275" y2="110" stroke="#0d8eb1" stroke-width="5" marker-end="url(#arrow-cap)"/><line x1="475" y1="110" x2="520" y2="110" stroke="#0d8eb1" stroke-width="5" marker-end="url(#arrow-cap)"/><line x1="720" y1="110" x2="765" y2="110" stroke="#0d8eb1" stroke-width="5" marker-end="url(#arrow-cap)"/></g></svg></section>

<section class="what-changed-block changed-panel"><h2>What this shifted</h2><p>The project moved from trying to make capsules faster to defining which flow and crosslinking conditions made faster capsule generation usable.</p></section>

<div class="case-cta-row two-button-cta"><a class="button primary" href="{{ '/projects/printed-interconnect-reliability/' | relative_url }}">Next: Printed Interconnect Reliability →</a><a class="button secondary email-button" href="mailto:{{ site.email }}">Email Nathan</a></div>
