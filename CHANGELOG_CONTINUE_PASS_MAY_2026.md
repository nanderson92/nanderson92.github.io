# Continuation polish pass — May 2026

## Implemented
- Added a homepage artifact wall, replacing the text-only proof row with three real evidence artifacts: microdevice trajectory extraction, microencapsulation microscopy, and thermocycler automation hardware.
- Strengthened image-card behavior so project thumbnails and artifact frames use non-cropping `object-fit: contain`, natural aspect ratios, visible overflow, and mobile-safe max heights.
- Added responsive WebP derivatives for large artifacts and poster imagery to improve performance while preserving image clarity.
- Removed public-facing resume maintenance/checklist language and replaced it with a finished recruiter-facing resume summary.
- Removed planned-note teaser cards from the Notes page so the public page only shows a completed note.
- Added final CSS overrides to prevent awkward heading hyphenation and word splitting across card titles, note titles, and project headings.
- Tightened artifact-card CSS so charts, dashboards, microscopy, and hardware photos do not clip axes, legends, labels, or physical components.

## Images placed or reinforced
- `artifact-microdevice-trajectory-overlay` — homepage artifact wall, Micromodular Deposition, Droplet Image Analysis, Case Files index.
- `artifact-group-motion-dashboard` — Micromodular Deposition and Droplet Image Analysis.
- `artifact-radial-tangential-velocity` — Micromodular Deposition, Droplet Image Analysis, Case Files index.
- `artifact-microcapsule-microscopy` — homepage artifact wall, homepage featured card, Stem-Cell Microencapsulation, Case Files index.
- `artifact-peg-shell-thickness` — Stem-Cell Microencapsulation.
- `artifact-thermocycler-front` and `artifact-thermocycler-fan-electronics` — homepage artifact wall, Thermocycler Process Automation, Case Files index.
- `four-point-probe-method.svg` — Printed Interconnect Reliability and homepage/Case Files cards.

## Remaining manual follow-up
- Run a full Jekyll build and browser QA in the final deployment environment.
- Replace the mailto-based “Schedule a call” action with a real Cal.com or Calendly URL when available.
- Add public GitHub/notebook links only when the repos or notebooks are ready to share.
- Add final run metadata, scale bars, calibration details, and redesigned publication-style plots as they become available.
