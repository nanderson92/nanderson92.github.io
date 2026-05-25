---
layout: page
title: Thin Film Semiconductor Growth & Characterization
category: MBE + characterization matrix
tags: Semiconductors · Thin Films · Materials Characterization
subtitle: Thin-film work connecting deposition conditions to morphology, phase, composition, and structural readouts.
---

## Summary

This compact build log captures semiconductor materials work focused on thin-film growth and characterization. The useful lesson was not “I know the acronyms”; it was learning how a growth condition becomes a measurable film response.

## Problem / motivation

Thin-film semiconductor properties depend strongly on deposition conditions, crystallinity, composition, and microstructure. The hard part is connecting growth parameters to measurable material quality and device-relevant behavior without overclaiming what one characterization technique can prove.

<figure class="thin-film-visual-card">
 <img src="{{ '/assets/images/thin-film-characterization-visual.svg' | relative_url }}" alt="Representative thin-film characterization schematic connecting MBE growth to SEM, XRD, XPS, and Raman readouts." loading="lazy">
 <figcaption>Representative characterization map: deposition conditions only become useful when they can be connected to film structure and device-relevant material quality.</figcaption>
</figure>

## Deposition-to-characterization flow

<div class="process-map compact-flow-map" aria-label="Thin film semiconductor process flow">
 <div class="process-map-stage"><p>DEPOSITION CONDITIONS</p><span>source material</span><span>vacuum</span><span>substrate</span></div>
 <div class="process-map-arrow" aria-hidden="true">→</div>
 <div class="process-map-stage"><p>FILM STRUCTURE</p><span>composition</span><span>morphology</span><span>crystallinity</span></div>
 <div class="process-map-arrow" aria-hidden="true">→</div>
 <div class="process-map-stage decision-stage"><p>CHARACTERIZATION RESPONSE</p><span>device-relevant material quality</span></div>
</div>

## Characterization matrix

| Technique | What it tells you |
|---|---|
| SEM | Morphology / surface structure |
| XRD | Crystallinity / phase |
| XPS | Surface composition / chemical state |
| Raman | Vibrational and structural signatures |

<div class="badge-row"><span class="badge">MBE</span><span class="badge">SEM</span><span class="badge">XRD</span><span class="badge">XPS</span><span class="badge">Raman</span><span class="badge">Thin Films</span></div>

## What I’d do next

To make this page a stronger standalone story, I would add one concrete experiment: deposition condition, characterization response, and the interpretation that followed. Right now the strongest honest use of this work is as a materials-characterization proof point rather than a full process-development case.

<div class="case-cta-row">
 <a class="button primary" href="{{ '/projects/' | relative_url }}">View all projects</a>
 <a class="button secondary" href="{{ '/assets/files/Nathan_Anderson_Resume.pdf' | relative_url }}" download="Nathan_Anderson_Resume.pdf">Download Resume</a>
 <a class="button tertiary" href="mailto:{{ site.email }}">Contact</a>
</div>
