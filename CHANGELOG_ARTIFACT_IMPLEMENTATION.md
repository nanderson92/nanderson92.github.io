# Artifact implementation changelog

## Images placed

- `artifact-microdevice-trajectory-overlay.png` from `trajectory_overlay(2).png`
  - Homepage artifact wall
  - Homepage/project index Micromodular Electronics Deposition thumbnail
  - Micromodular Electronics Deposition flagship Figure 1

- `artifact-group-motion-dashboard.png` from `00_group_motion_dashboard(2).png`
  - Micromodular Electronics Deposition Figure 2
  - Droplet Image Analysis Workflows Figure 1

- `artifact-radial-tangential-velocity.png` from `image(238).png`
  - Micromodular Electronics Deposition Figure 3
  - Droplet Image Analysis Workflows Figure 2
  - Homepage/project index Droplet Image Analysis thumbnail

- `artifact-microcapsule-microscopy.jpg` from `50mM30fr3.jpg`
  - Homepage artifact wall
  - Homepage/project index Stem-Cell Microencapsulation thumbnail
  - Stem-Cell Microencapsulation hero Figure 1

- `artifact-peg-shell-thickness.png` from `Picture1.png`
  - Stem-Cell Microencapsulation Figure 2 quantitative artifact

- `artifact-alginate-hardening.png` from `image(246).png`
  - Stem-Cell Microencapsulation Figure 3 mechanism schematic

- `artifact-thermocycler-front.png` from `image(241).png`
  - Homepage artifact wall
  - Homepage/project index Thermocycler Process Automation thumbnail
  - Thermocycler Process Automation hero hardware artifact

- `artifact-thermocycler-fan-electronics.png` from `image(242).png`
  - Thermocycler Process Automation annotated component artifact

- `artifact-thermocycler-pid-code.png` from `image(243).png`
  - Thermocycler Process Automation control-code artifact
  - Droplet Image Analysis Workflows secondary code/process artifact

- `artifact-thermocycler-display-code.png` from `image(244).png`
  - Thermocycler Process Automation display/feedback-code artifact

- `artifact-rame-hart-goniometer-cropped.jpg` from `image(239).png`
  - Droplet Image Analysis Workflows measurement setup artifact
  - Cropped to reduce blank wall and make the instrument larger in frame

## Redrawn or avoided artifacts

- `four-point-probe-method.svg` was redrawn as a site-native method diagram instead of embedding the supplied four-point reference image directly.
- `image(247).png` was not embedded because ownership/permission was unclear from the file alone.
- `site-native-alginate-hardening.svg` was added as a backup redrawn schematic option.

## Placeholders replaced

- Replaced public-facing artifact placeholders on:
  - Homepage technical proof section
  - Micromodular Electronics Deposition
  - Droplet Image Analysis Workflows
  - Stem-Cell Microencapsulation
  - Printed Interconnect Reliability
  - Thermocycler Process Automation

- Cleaned visible placeholder copy:
  - Removed `Replace with current artifact` from the homepage recent strip.
  - Replaced `Artifact placeholder` wording on generic pages with cleaner planned-evidence language.
  - Replaced `Placeholder excerpt` and `Ask for current draft` on the notes page.
  - Replaced `Resume maintenance note` heading with `Resume content focus`.

## Still needs final metadata or redesigned final figures

- Micromodular deposition trajectory artifacts need final run metadata:
  - solvent already noted as IPA
  - droplet volume
  - substrate/backing
  - frame rate
  - pixel-to-micron calibration
  - replicate count by condition

- Microencapsulation microscopy artifact needs final publication metadata:
  - scale bar verification
  - condition
  - flow rate
  - CaCl₂ concentration
  - run ID

- PEG shell-thickness chart should eventually be redesigned in the site visual style with:
  - n
  - error-bar definition
  - p-value threshold
  - clear legend labels

- Printed Interconnect Reliability still needs real artifacts:
  - microscope image of printed line
  - resistance drift plot
  - pass/monitor/fail classification example
  - stress protocol table

- Thermocycler Process Automation still needs:
  - setpoint vs. measured-temperature trace
  - ramp rate
  - overshoot
  - settling time
  - hold stability
  - cycle repeatability

## Anti-cropping fix

- Added CSS overrides for artifact cards, wall cards, project thumbnails, and visual grids so images use `object-fit: contain` and `height: auto` rather than cropped cover behavior.
- Artifact frames now preserve full image content on desktop and mobile, with padding and containment instead of forced full-bleed cropping.
