---
layout: page
title: Printed Interconnect & FET Reliability
category: Reliability · Process Control
tags: Electrical Testing · Printed Interconnects · Reliability
subtitle: I use electrical drift and pass/fail behavior to identify process-control problems in printed micromodular circuits.
---

I think of this as the second half of the deposition problem. After the devices land, the question becomes simple: do the printed interconnects stay electrically usable, and can the failure point tell me which process step moved?

<div class="case-summary-box clean-metadata-layout">
 <p class="system-label small">QUICK READ</p>
 <div class="case-summary-grid"><span><strong>Signal</strong> Initial resistance, normalized drift, intermittent opens, and stress response.</span><span><strong>Decision</strong> Pass, monitor, fail, or trace the failure back to handling, contact, deposition, or cure.</span><span><strong>Tools</strong> Keithley measurements, Python/JMP analysis, Excel screening, optical inspection.</span></div>
</div>

<figure class="wide-figure reliability-plot-figure"><img src="{{ '/assets/images/reliability-drift-plot.svg' | relative_url }}" alt="Representative resistance drift plot with stable, drifting, and intermittent-open traces." loading="eager"><figcaption>Representative format for classifying stable traces, drifting traces, and intermittent opens under stress.</figcaption></figure>

## The hard part

Resistance is easy to measure once. Reliability is harder because a trace that passes initially can drift, jump, or fail only after handling or stress. The first analysis pass treated every high-resistance result the same; that was wrong. I learned to separate stable drift from intermittent contact behavior because those imply different process fixes.

## My role

<div class="role-block"><p>I organize electrical measurements into a process-control loop: measure initial R, stress the device or interconnect, measure drift, classify the failure mode, then connect that classification back to surface prep, deposition, contact, or cure conditions.</p></div>

## Go/no-go logic

<div class="process-map compact-flow-map" aria-label="Reliability control loop"><div class="process-map-stage"><p>MEASURE</p><span>initial R</span><span>continuity</span></div><div class="process-map-arrow">→</div><div class="process-map-stage"><p>STRESS</p><span>humidity</span><span>handling</span><span>time</span></div><div class="process-map-arrow">→</div><div class="process-map-stage"><p>CLASSIFY</p><span>stable</span><span>drift</span><span>open</span></div><div class="process-map-arrow">→</div><div class="process-map-stage decision-stage"><p>FIX</p><span>surface prep, contact, deposition, or cure</span></div></div>

## What I’d do next

For production, I would stop treating resistance as a single pass/fail number. I would define one drift threshold, one intermittent-open rule, and one sampling plan tied to the specific process step most likely to move. The assumption that breaks at scale is that failures are independent; in a real line, correlated drift across a batch is the signal.

<div class="case-cta-row"><a class="button primary" href="{{ '/projects/micromodular-deposition/' | relative_url }}">Related deposition build log →</a><a class="button secondary" href="{{ '/assets/files/Nathan_Anderson_Resume.pdf' | relative_url }}" download="Nathan_Anderson_Resume.pdf">Resume (PDF, 1 page)</a><a class="button tertiary" href="mailto:{{ site.email }}">Contact</a></div>
