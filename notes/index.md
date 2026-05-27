---
layout: page
title: Notes
category: Engineering notes
subtitle: Short process-engineering notes on measurement, reliability, and operator instincts.
description: Engineering notes on printed-line reliability, wet-process changeovers, and critical-to-quality judgment.
body_class: notes-page
last_updated: May 2026
---

<article class="long-note-card published-note">
 <p class="system-label">May 2026 · 6 min read</p>
 <h2>Why time-zero continuity is the wrong test for printed lines</h2>
 <p>Time-zero continuity is a weak reliability screen because it answers the easiest question in the system: did current pass through the line once, under the measurement conditions I gave it? That matters, but it is not the same as asking whether the printed line has enough margin to survive handling, humidity, temperature, probe contact, or the next processing step.</p>
 <p>A printed interconnect can look acceptable at time zero and still carry a built-in failure mode. The line may have a narrow neck, a partially cured region, weak adhesion at the edge, local cracking that is not yet open, or a probe-contact artifact that hides the true line behavior. A single pass/fail continuity check compresses all of those states into one label. That is convenient for a quick screen, but it is poor process feedback.</p>
 <p>The better test is not simply “measure resistance more often.” The better test is to classify how resistance behaves. High initial resistance points toward geometry, cure, print continuity, or contact setup. Smooth upward drift suggests material aging, humidity sensitivity, or a slow change in the conductive network. A sudden open circuit suggests cracking, delamination, handling damage, or a mechanical weak point. Intermittent readings may be a real instability, but they may also be probe contact. Those cases should not receive the same engineering response.</p>
 <p>That distinction matters because a reliability screen should change the next run. If the line fails by gradual drift, I would look first at ink condition, cure history, stress exposure, and environmental sensitivity. If it fails suddenly, I would inspect morphology, adhesion, edge roughness, handling, and probe history. If readings are intermittent, I would retest the contact and image the line before calling the device bad. The point is not to collect a prettier plot. The point is to prevent the same failure mode from being printed again.</p>
 <p>Four-point resistance testing helps because it separates current sourcing from voltage sensing, reducing the chance that contact resistance dominates the measurement. It still does not solve the full problem by itself. A four-point value is useful only when paired with the stress condition, measurement cadence, probe setup, physical inspection, and a baseline definition such as R/R₀. Without that context, the number is too easy to overinterpret.</p>
 <p>For a process-development screen, I would rather see a simple classification matrix than a single continuity badge. Pass means stable resistance under the relevant stress window. Monitor means drift that has not crossed the failure threshold but is moving in the wrong direction. Fail means open circuit, high resistance, or clear physical damage. Artifact means the measurement itself needs to be questioned before the process is blamed. That fourth category is important. Treating every strange reading as a process failure wastes time; treating every strange reading as a contact issue hides real defects.</p>
 <p>Time-zero continuity can stay as an early gate, but it should not be the headline validation claim. The headline should be resistance behavior tied to a failure class and an upstream process check. That is the difference between testing a line and learning how to print a better one.</p>
</article>
