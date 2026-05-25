---
layout: page
title: Stem-Cell Microencapsulation
category: 20× throughput increase
tags: Microfluidics · Stem-Cell Biotech · Process Development
subtitle: I tuned a flow-focused core-shell capsule process until throughput and usable yield moved together.
---

<div class="micro-stats-hero big-stat-strip" aria-label="Selected outcomes"><article><strong>20×</strong><span>throughput increase</span></article><article><strong>~50%</strong><span>encapsulation-yield improvement</span></article><article><strong>Lower</strong><span>coalescence through flow/crosslinking changes</span></article><article><strong>QC</strong><span>microscopy-supported screening workflow</span></article></div>

I worked on a flow-focused microfluidic encapsulation process for core-shell hydrogel capsules, connecting flow ratio, crosslinking dwell time, and microscopy QC to capsule throughput, coalescence, and usable yield.

## The hard part

The hard part was that throughput and capsule quality wanted to fight each other. Turning the flow rate up made the process faster, but it also exposed weak points in shell formation, collection, and coalescence. One early condition produced more capsules but worse usable output; that forced me to treat yield, not raw droplet count, as the actual metric.

<figure class="wide-figure microfluidic-schematic-figure"><img src="{{ '/assets/images/microfluidic-flow-schematic.svg' | relative_url }}" alt="Microfluidic process schematic showing core stream, shell stream, flow focusing, crosslinking dwell region, collection, and microscopy QC." loading="eager"><figcaption>Process logic: streams converge, capsules form, crosslinking stabilizes the shell, collection preserves the product, and microscopy decides whether the condition is useful.</figcaption></figure>

## Knobs I tuned

| Knob | Mechanism | Output affected |
|---|---|---|
| Continuous/dispersed flow ratio | Shear and droplet breakup | Capsule size, throughput, coalescence |
| Crosslink dwell time | Shell formation and stabilization | Handling stability and usable yield |
| Collection condition | Post-formation environment | Aggregation and coalescence |
| Cell suspension handling | Biological compatibility | Viability and usefulness |

## My role

<div class="role-block"><p>I tuned flow conditions, adjusted crosslinking logic, used microscopy to separate good capsules from coalesced or unstable output, and helped translate observations into a better operating window.</p></div>

## What I’d do next

If I built this again for a small biotech team, I would add a faster QC loop: size distribution, coalescence count, and shell-integrity scoring immediately after collection. The scale-up risk is not making more capsules; it is preserving a narrow enough distribution that downstream cell-culture conditions still mean what you think they mean.

<div class="case-cta-row"><a class="button primary" href="{{ '/projects/' | relative_url }}">See all projects</a><a class="button secondary" href="{{ '/assets/files/Nathan_Anderson_Resume.pdf' | relative_url }}" download="Nathan_Anderson_Resume.pdf">Resume (PDF, 1 page)</a><a class="button tertiary" href="mailto:{{ site.email }}">Contact</a></div>
