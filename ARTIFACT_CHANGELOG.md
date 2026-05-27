# Artifact implementation changelog

## Images added to `assets/images/artifacts/`

- `microdevice-trajectory-overlay.png` from `trajectory_overlay(2).png`
- `group-motion-dashboard.png` from `00_group_motion_dashboard(2).png`
- `radial-tangential-velocity.png` from `image(238).png`
- `microcapsule-microscopy.jpg` from `50mM30fr3.jpg`
- `peg-shell-thickness-flowrate.png` from `Picture1.png`
- `alginate-hardening-concept.png` from `image(246).png`
- `thermocycler-prototype-front.png` from `image(241).png`
- `thermocycler-prototype-annotated.png` from `image(242).png`
- `thermocycler-code-pid-crop.png` from `image(243).png`
- `thermocycler-code-display-crop.png` from `image(244).png`
- `rame-hart-goniometer-cropped.jpg` from `image(239).png`, cropped to reduce blank wall and emphasize the instrument
- `four-point-probe-method.svg`, redrawn as a site-native method diagram instead of embedding the provided reference image
- `microencapsulation-flow-native.svg`, recreated as a site-native microfluidic encapsulation schematic instead of embedding an ownership-unclear reference image

## Homepage placements

- Added `Evidence, not just project summaries.` section near the top.
- Added three artifact cards only:
  - Microdevice trajectory extraction: `microdevice-trajectory-overlay.png`
  - Microencapsulation microscopy: `microcapsule-microscopy.jpg`
  - Thermocycler automation prototype: `thermocycler-prototype-front.png`
- Replaced the “Recently shipped” placeholder text with concrete artifact-update language.
- Removed the previous public-facing artifact-preview placeholder section.

## Project page placements

### Micromodular Electronics Deposition

- Replaced the top placeholder artifact grid with:
  - Figure 1: `microdevice-trajectory-overlay.png`
  - Figure 2: `group-motion-dashboard.png`
  - Figure 3: `radial-tangential-velocity.png`
- Added run metadata table with fields for solvent, droplet volume, substrate/backing, frame rate, calibration, and output metrics.
- Added a limitation note stating that the current plots represent preliminary run-level analysis and need replicate-backed comparison.

### Droplet Image Analysis Workflows

- Reframed the page as the tooling/methods case file behind droplet deposition analysis.
- Added pipeline section: raw video → calibration → object detection → track linking → radial/tangential decomposition → dashboard export.
- Added:
  - `group-motion-dashboard.png`
  - `radial-tangential-velocity.png`
  - `thermocycler-code-pid-crop.png` as a small code/control artifact card
  - `rame-hart-goniometer-cropped.jpg` as a setup image
- Added quality-control checklist for calibration, frame rate, track loss, smoothing window, sign convention, tracking coverage, and replicate count.

### Stem-Cell Microencapsulation

- Replaced placeholder artifacts with:
  - Figure 1: `microcapsule-microscopy.jpg`
  - Figure 2: `peg-shell-thickness-flowrate.png`
  - Figure 3: `alginate-hardening-concept.png`
  - Site-native process schematic: `microencapsulation-flow-native.svg`
- Added public-publication cleanup note for scale bar, condition, flow rate, CaCl₂ concentration, and run ID.
- Added before/after metric table using “to be filled” where baseline values are not known.

### Printed Interconnect Reliability

- Replaced the reference method image with a redrawn site-native SVG: `four-point-probe-method.svg`.
- Added deliberate missing-artifact slots:
  - Add resistance drift plot
  - Add microscope image of printed line
  - Add stress protocol table
  - Add pass/monitor/fail example
- Removed public-facing generic artifact-placeholder copy.

### Thermocycler Process Automation

- Replaced placeholder artifacts with:
  - Hero hardware artifact: `thermocycler-prototype-front.png`
  - Annotated component image: `thermocycler-prototype-annotated.png`
  - PID/control code card: `thermocycler-code-pid-crop.png`
  - Display/feedback code card: `thermocycler-code-display-crop.png`
- Added component legend with a verification note for the thermal input/sample-region label.
- Added missing-artifact slot for setpoint vs. measured-temperature trace.

## Global cleanup

- Added consistent artifact-card CSS for real images, captions, metadata, artifact labels, responsive grids, and deliberate missing-artifact slots.
- Cleaned public placeholder language from homepage, notes, resume, and relevant case-file sections.
- Updated the notes page and resume page to avoid public-facing placeholder language.
- Updated project index thumbnails for the major case files to use real artifacts where useful.

## Still needs final metadata or redesigned artifacts

- Micromodular deposition figures need final droplet volume, substrate/backing, frame rate, calibration, and run ID.
- Microcapsule microscopy needs final scale bar, run condition, flow rate, CaCl₂ concentration, and run ID before publication.
- PEG shell-thickness chart should be redesigned in the site’s visual style and include n, error-bar definition, p-value threshold, and clear legend labels.
- Printed interconnect reliability still needs real printed-line microscopy, resistance-drift plot, stress protocol table, and classification examples.
- Thermocycler automation still needs setpoint-vs-measured-temperature validation trace with ramp rate, overshoot, settling time, hold stability, and repeatability.
