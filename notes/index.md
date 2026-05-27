---
layout: page
title: Notes
category: Thinking notes
subtitle: Short engineering notes on measurement, reliability, and operator instincts.
description: Engineering notes on printed-line reliability, wet-process changeovers, and CTQ judgment.
body_class: notes-page
last_updated: May 2026
---

<article class="published-note note-article">
 <p class="system-label">May 2026 · 6 min read</p>
 <h2>Why time-zero continuity is the wrong test for printed lines</h2>
 <p>Time-zero continuity is a weak reliability test because it asks the easiest possible question: does current pass right now? That matters, but it does not tell you whether a printed line has enough process margin to survive humidity, handling, thermal exposure, probe contact, or the next assembly step.</p>
 <p>A printed interconnect can pass at time zero while still carrying a built-in failure mode. A line with marginal cure, poor edge definition, thin necking, weak adhesion, or probe-sensitive contact may look acceptable until stress makes the defect visible. The pass/fail label arrives late because the measurement was not connected to the failure mechanism.</p>
 <p>The better screen is resistance behavior under a defined stress interval. I would rather know whether normalized resistance, <abbr title="resistance divided by initial resistance">R/R₀</abbr>, drifts smoothly, jumps suddenly, or flips intermittently than know only that the line was initially continuous. Smooth drift points toward material aging or environmental sensitivity. A sudden open points toward cracking, delamination, or handling damage. Intermittent readings force a measurement-artifact check before blaming the line.</p>
 <p>That is why the measurement has to be paired with inspection and retest logic. Four-point resistance testing helps separate contact resistance from line resistance, but it does not remove every artifact. Probe marks, alignment, surface contamination, and local geometry still matter. A good control plan treats those as classes, not excuses.</p>
 <p>The useful output is not a prettier plot. It is a decision table: pass, monitor, fail, or artifact. Pass means the line stays inside the resistance-drift window and the physical inspection is clean. Monitor means drift is visible but not yet disqualifying. Fail means the electrical and physical evidence agree. Artifact means the measurement chain needs a retest before the process is blamed.</p>
 <p>Time-zero continuity belongs at the front of the screen, not the end. The engineering question is whether the line has process margin after the first stress it is likely to see.</p>
</article>

<section class="notes-grid compact-notes-grid" aria-label="Future notes">
 <article class="note-card"><p class="system-label">Future note</p><h2>What McDonald’s taught me about wet-process changeovers</h2><p>Queue control, prep timing, and bottleneck response trained the same habits I now use in wet-lab workflow debugging and manufacturing-development decisions.</p></article>
 <article class="note-card"><p class="system-label">Future note</p><h2>The five questions I ask before believing a CTQ</h2><p>A CTQ is worth trusting only when it connects to a decision, survives measurement noise, maps to a failure mode, and changes the next run.</p></article>
</section>
