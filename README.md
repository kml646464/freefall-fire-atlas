# Freefall Fire Atlas

Fire safety dashboard for Moon bases, rovers and spacecraft, built on NASA PSI microgravity combustion data. NASA Space Apps 2026, Flame in Freefall. Team The Core.

**Live dashboard:** https://kml646464.github.io/freefall-fire-atlas/freefall-fire-atlas.html

**Project demo (7 slides):** https://kml646464.github.io/freefall-fire-atlas/freefall-fire-atlas-demo.pdf

When a fire starts in a habitat, what should the crew do, and how certain can that answer be? The dashboard answers this for five habitats, a Moon base, a pressurized rover, a Mars base, a spacecraft in transit and a space station.

- A system-dynamics cabin fire model with our own model of the oxygen limit under airflow and gravity
- Bayesian calibration against eight NASA observations, keeping 138 of 60,000 parameter sets
- Monte Carlo simulation of 1,920 fires per habitat and crew response, reported with ranges
- A neural network trained on SAME-R ISS flight sensor data, tested on runs it never saw
- All 23 PSI combustion investigations ranked per habitat, with CSV and JSON export
- A custom scenario page for any oxygen, pressure, gravity, volume and airflow
- English and Turkish

The whole dashboard is the single file `freefall-fire-atlas.html`. It runs locally in the browser and calls no external AI service.

## Data
NASA Physical Sciences Informatics (23 combustion investigations), SAME-R ISS flight sensor data (2010), NASA Technical Reports Server, NASA Spinoff.

## Use of SI (Super Intelligence)
The approach is the team's own, including the system-dynamics model, the oxygen-limit model, its calibration, the Monte Carlo design and the neural network. Claude (Anthropic) served as a development assistant, chiefly for the web interface, and helped implement and debug code and extract PSI metadata.
