---
layout: page
title: Droplet Image Analysis Workflows
category: Python · ImageJ · Video Metrics
tags: Image Analysis · Microscopy · Process Metrics
subtitle: I convert microscope videos into time-series metrics that can actually guide process decisions.
---

I built analysis workflows because visual inspection was not enough. A droplet video looks convincing until you try to compare two substrate conditions across trials. Then you need calibration, segmentation, time alignment, and a metric you can defend.

## Workflow

<div class="process-map compact-flow-map" aria-label="Droplet image analysis workflow"><div class="process-map-stage"><p>VIDEO</p><span>top view</span><span>side view</span></div><div class="process-map-arrow">→</div><div class="process-map-stage"><p>SEGMENT</p><span>edge</span><span>footprint</span></div><div class="process-map-arrow">→</div><div class="process-map-stage"><p>CALIBRATE</p><span>pixel scale</span><span>time base</span></div><div class="process-map-arrow">→</div><div class="process-map-stage decision-stage"><p>METRICS</p><span>r(t), θ(t), density, decision</span></div></div>

## The hard part

The first thresholding pass failed whenever the droplet edge had weak contrast. That pushed me toward workflows that combine controlled cropping, calibration, and manual review instead of pretending a single automatic threshold was universally reliable.

## My role

<div class="role-block"><p>I wrote and tested image-analysis steps for extracting droplet radius, contact-line motion, and deposition-region behavior from microscopy videos. The goal was not pretty plots; it was turning video into process variables.</p></div>

## GitHub

<p><a class="button tertiary" href="{{ site.github }}">GitHub profile →</a></p>

## What I’d do next

I would build a small public repo with sanitized sample frames, a calibration notebook, and one end-to-end example from video to normalized radius trace. The production version would flag low-confidence edges automatically rather than silently returning bad metrics.

<div class="case-cta-row"><a class="button primary" href="{{ '/projects/micromodular-deposition/' | relative_url }}">Related deposition project →</a><a class="button secondary" href="{{ '/assets/files/Nathan_Anderson_Resume.pdf' | relative_url }}" download="Nathan_Anderson_Resume.pdf">Resume (PDF, 1 page)</a><a class="button tertiary" href="mailto:{{ site.email }}">Contact</a></div>
