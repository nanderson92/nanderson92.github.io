---
layout: page
title: Process Simulation & Design
category: PFDs · Balances · Simulation
tags: Aspen · MATLAB · Process Design
subtitle: I turn process descriptions into flowsheets, balance structures, assumptions, and tradeoff decisions.
---

Simulation is only useful when the assumptions are visible. I use PFDs, material balances, and operating-condition logic to make a process model explainable instead of black-box.

## Workflow

<div class="process-map compact-flow-map" aria-label="Process simulation workflow"><div class="process-map-stage"><p>FEED</p><span>basis</span><span>composition</span></div><div class="process-map-arrow">→</div><div class="process-map-stage"><p>MIX</p><span>streams</span><span>recycle</span></div><div class="process-map-arrow">→</div><div class="process-map-stage"><p>SEPARATE</p><span>VLE</span><span>recovery</span></div><div class="process-map-arrow">→</div><div class="process-map-stage decision-stage"><p>PRODUCT</p><span>purity, yield, duty</span></div></div>

## The hard part

The hard part is not drawing boxes. It is deciding which assumptions are strong enough to support a design decision and which ones only make the model look precise. I learned to treat convergence as a starting point, not proof that the process makes sense.

## Variables I watch

| Variable | Why it matters |
|---|---|
| Feed composition | Sets material-balance basis and separation difficulty. |
| Operating temperature / pressure | Affects phase behavior, energy duty, and equipment feasibility. |
| Recovery / purity targets | Define whether an alternative is technically acceptable. |
| Thermodynamic model | Determines whether VLE/separation predictions are physically reasonable. |

## What I’d do next

For a startup process model, I would keep the first version brutally simple: one defensible PFD, one balance table, one sensitivity plot, and one clear decision. The failure mode is over-modeling before anyone knows which knob matters.

<div class="case-cta-row"><a class="button primary" href="{{ '/projects/' | relative_url }}">See all projects</a><a class="button secondary" href="{{ '/assets/files/Nathan_Anderson_Resume.pdf' | relative_url }}" download="Nathan_Anderson_Resume.pdf">Resume (PDF, 1 page)</a><a class="button tertiary" href="mailto:{{ site.email }}">Contact</a></div>
