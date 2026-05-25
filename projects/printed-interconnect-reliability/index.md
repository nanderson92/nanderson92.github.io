---
layout: page
title: Printed Interconnect & FET Reliability
category: Resistance drift → go/no-go logic
tags: Semiconductors · Reliability · Process Control · Manufacturing
subtitle: "Printed conductive lines look fine on day one and fail in week three through invisible drift, intermittent opens, or stress damage. I built the measurement protocol that catches those failure classes early enough to fix the process upstream."
---

## Failure classes

<div class="text-output-grid failure-taxonomy-grid">
 <article><h3>High initial R</h3><p>The line starts outside the acceptable range, pointing to deposition, geometry, or cure issues before stress testing begins.</p></article>
 <article><h3>Resistance drift</h3><p>The line passes at first but changes enough under stress to become a monitor/fail condition.</p></article>
 <article><h3>Open circuit</h3><p>The electrical path breaks. That failure is not “bad data”; it is a process event that needs a candidate cause.</p></article>
 <article><h3>Intermittent behavior</h3><p>Contact or handling effects create unstable readings that should be classified separately from smooth drift.</p></article>
</div>

<div class="role-block">
 <p>I built electrical screening workflows, organized resistance/failure data, interpreted stress-response behavior, and turned drift patterns into threshold logic that points back to likely process causes.</p>
</div>

<div class="connection-note"><strong>Connection:</strong> deposition asks where devices land. Reliability asks whether the printed interconnects and device interfaces stay electrically usable after assembly.</div>

## Process loop

<div class="process-map reliability-loop" aria-label="Printed interconnect reliability process-control loop">
 <div class="process-map-stage"><p>FABRICATE</p><span>surface prep</span><span>print interconnect</span><span>cure / handle</span></div>
 <div class="process-map-arrow" aria-hidden="true">→</div>
 <div class="process-map-stage"><p>MEASURE</p><span>initial R</span><span>continuity</span><span>repeat readings</span></div>
 <div class="process-map-arrow" aria-hidden="true">→</div>
 <div class="process-map-stage"><p>STRESS</p><span>humidity / temperature</span><span>time interval</span><span>re-measure</span></div>
 <div class="process-map-arrow" aria-hidden="true">→</div>
 <div class="process-map-stage decision-stage"><p>DECIDE</p><span>pass / monitor / fail / trace back to process step</span></div>
</div>

## What did not work at first

The easy mistake was treating a failed trace as just “bad data.” The more useful move was to ask what kind of failure it was. A smooth drift, a sudden open, and a noisy intermittent contact are different process clues.

## Process knobs

| Knob | Why it matters |
|---|---|
| Initial resistance | Separates geometry/deposition/cure issues from later reliability drift. |
| Normalized drift | Shows whether the line changes enough under stress to become a process concern. |
| Open-circuit behavior | Flags complete loss of electrical continuity rather than gradual degradation. |
| Intermittency | Separates contact/handling artifacts from material or interconnect aging. |
| Stress interval | Determines whether the screen is sensitive enough to catch early failure modes. |

## Methods and tools

<div class="two-col">
 <div class="matrix-card"><h3>Electrical testing</h3><p>Resistance measurements, continuity checks, stress/re-measure intervals, and failure classification.</p></div>
 <div class="matrix-card"><h3>Process feedback</h3><p>Threshold logic that links electrical symptoms to candidate changes in surface prep, printing, cure, or handling.</p></div>
</div>

<div class="badge-row"><span class="badge">Keithley</span><span class="badge">Four-point probe</span><span class="badge">Python</span><span class="badge">JMP</span><span class="badge">Excel</span><span class="badge">Reliability</span></div>

## What I’d do next

If I were building this into a production screen, I would standardize one resistance-normalization workflow and require each test to return both a number and a failure class. The next useful artifact is a short decision table that tells an operator what to change when a trace drifts, opens, or behaves intermittently.

<div class="case-cta-row">
 <a class="button primary" href="{{ '/projects/micromodular-deposition/' | relative_url }}">Related deposition build →</a>
 <a class="button secondary" href="{{ '/assets/files/Nathan_Anderson_Resume.pdf' | relative_url }}" download="Nathan_Anderson_Resume.pdf">Download Resume</a>
 <a class="button tertiary" href="mailto:{{ site.email }}">Contact</a>
</div>
