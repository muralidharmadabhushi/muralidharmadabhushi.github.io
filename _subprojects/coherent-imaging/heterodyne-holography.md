---
layout: research-project
title: Heterodyne Holography
project_id: heterodyne-holography
nav_id: projects
order: 2
category_id: coherent-imaging
category_title: Coherent Imaging
category_url: /projects/coherent-imaging.html
#image: /assets/images/subprojects/coherent-imaging/heterodyne-holography.svg
image: /assets/images/under_construction.svg
image_alt: Heterodyne Holography figure
brief_image: /assets/images/subprojects/coherent-imaging/fmcw-lidar.svg
brief_image_alt: FMCW LiDAR figure
technologies_title: "Under the Hood"
applications_title: "Broader Applications"
brief: >
  We developed an FMCW LiDAR system that measures the time-of-flight distribution of light, i.e., the distribution of travel times from a source to a detector through a scattering material, with a temporal resolution of approximately 1 picosecond. By selectively analyzing light that has traveled along different paths, we can recover information otherwise hidden by scattering, opening up new possibilities for imaging through fog and biological tissue.
technologies: >
  - To achieve picosecond-scale temporal resolution, we needed to tune our laser over an exceptionally wide frequency range while maintaining sweep linearity. We developed an inverse-filtering approach to compensate for the laser's thermal response, combined with interferometric feedback to correct residual nonlinearities.

  - We built a state-machine-based control system to coordinate different portions of the laser sweep with instrument triggering and data acquisition, ensuring precise timing and repeatable measurements.

  - To ensure that every sweep starts at a reproducible optical frequency, we implemented and carefully tuned feedback loops using beat-note detection, phase-locked loops, and offset locking relative to a master laser. We also incorporated rubidium-based frequency referencing to monitor long-term stability.

technologies_image: /assets/images/subprojects/coherent-imaging/fmcw-lidar-key-tech.svg
technologies_image_alt: FMCW LiDAR optical setup

applications: >
  Beyond LiDAR, our laser sweep linearization and frequency stabilization techniques could support chemical fingerprinting and trace-gas detection through laser spectroscopy, optical frequency combs for broadband molecular measurements, quantum sensing with atom-interferometric gravimeters and accelerometers, and precision optical metrology for photonic chip characterization. These applications share a need for precisely controlled, accurately calibrated, and repeatable optical frequency sweeps.

publications:
  - fmcw-paper-1
  - fmcw-paper-2
---
