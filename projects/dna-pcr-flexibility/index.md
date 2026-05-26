---
layout: page
title: DNA Flexibility Assay Development
category: Early assay-development exposure
date_range: Earlier research
affiliation: Maher Lab, Mayo Clinic
tags: Molecular Biology · PCR · Experimental Design
subtitle: "Early assay-development exposure: PCR, controls, repeatability, and troubleshooting."
---

<p class="credential-line"><strong>Supporting evidence</strong> · DNA/PCR assay development</p>

This page is intentionally shorter than the flagship process-development case files. Its role is to show early experimental discipline: protocol execution, controls, troubleshooting, and keeping a fragile molecular workflow auditable enough to trust the readout.

## Assay-design problem

DNA mechanics at very short lengths are difficult to probe because small length scales demand careful assay design, clean controls, and precise molecular-biology execution. In this work, the useful contribution was exposure to assay logic and control-condition troubleshooting rather than a public standalone manufacturing result.

## Control logic snapshot

<div class="artifact-table-wrap">
<table class="artifact-table">
<thead><tr><th>Assay element</th><th>Purpose</th><th>Failure mode it protects against</th></tr></thead>
<tbody>
<tr><td>Positive control</td><td>Confirms the PCR/readout workflow can produce the expected signal.</td><td>False interpretation of a failed setup as a biological effect.</td></tr>
<tr><td>Negative control</td><td>Checks contamination and background behavior.</td><td>False positives from carryover or nonspecific amplification.</td></tr>
<tr><td>Comparison construct</td><td>Creates a reference condition for flexibility interpretation.</td><td>Unanchored readout with no internal comparison.</td></tr>
<tr><td>Troubleshooting loop</td><td>Separates prep, amplification, and readout problems.</td><td>Misassigning failure to the wrong step.</td></tr>
</tbody>
</table>
</div>

## Assay workflow

<div class="process-map assay-flow-map" aria-label="DNA PCR assay workflow schematic">
 <div class="process-map-stage"><p>SAMPLE / DESIGN</p><span>construct logic</span><span>length scale</span></div>
 <div class="process-map-arrow" aria-hidden="true">→</div>
 <div class="process-map-stage"><p>PCR WORKFLOW</p><span>prep</span><span>amplify</span><span>check</span></div>
 <div class="process-map-arrow" aria-hidden="true">→</div>
 <div class="process-map-stage"><p>CONTROL CONDITION</p><span>positive</span><span>negative</span><span>comparison</span></div>
 <div class="process-map-arrow" aria-hidden="true">→</div>
 <div class="process-map-stage decision-stage"><p>READOUT / LOOP</p><span>measurement and troubleshooting</span></div>
</div>

## Methods and tools

<div class="two-col">
 <div class="matrix-card"><h3>Experimental work</h3><p>Assisted with DNA/PCR-based experimental workflows, sample preparation, controls, and troubleshooting.</p></div>
 <div class="matrix-card"><h3>Measurement logic</h3><p>Helped develop experiments aimed at measuring DNA flexibility at very short base-pair lengths.</p></div>
</div>

<div class="badge-row"><span class="badge">PCR</span><span class="badge">DNA</span><span class="badge">Assay Development</span><span class="badge">Experimental Design</span><span class="badge">Mayo Clinic</span></div>

## What I’d do next

If I were expanding this work now, I would focus on the control logic, not a larger narrative. The engineering decision would be whether the assay has enough control evidence to trust the readout before interpreting a biological mechanism.

<div class="case-cta-row">
 <a class="button primary" href="{{ '/projects/' | relative_url }}">View all case files</a>
 <a class="button secondary" href="{{ '/assets/files/Nathan_Anderson_Resume.pdf' | relative_url }}" download="Nathan_Anderson_Resume.pdf">Download Resume</a>
 <a class="button tertiary" href="mailto:{{ site.email }}">Contact</a>
</div>
