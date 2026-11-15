---
layout: research-project
title: Indirect Imaging Correlography
project_id: correlography
nav_id: projects
order: 1
category_id: computational-optics
category_title: Computational Optics
category_url: /projects/computational-optics.html
image: /assets/images/subprojects/computational-optics/nlos-correlography.svg
image_alt: NLOS Correlography figure
brief_image: /assets/images/subprojects/computational-optics/nlos-correlography.svg
brief_image_alt: NLOS Correlography figure
technologies_title: "Under the Hood"
applications_title: "Broader Applications"
brief: >
  When laser light illuminates objects, either directly or indirectly, as in looking-around-corners geometries shown here, it produces seemingly random intensity patterns known as speckle. However, these patterns contain a wealth of hidden information about the objects. We developed a technique called **Indirect Imaging Correlography** that exploits the hidden structure within these speckle patterns to reconstruct images of objects around corners.
technologies: >
  - We derived an imaging operator to analytically model how the position and orientation of an object affects image formation and resolution in a looking around corner setting. This required modeling light propagation in non-trivial geometries, including steep tilts, which are beyond the assumptions of conventional optical propagators.

  - We developed an experimental procedure to measure the modulation transfer function (MTF) of our indirect imaging correlography system, allowing us to quantitatively characterize imaging performance and validate theoretical predictions. We demonstrated the reconstruction of features as small as 250 µm a distance of 1 meter around a corner.
  
  - We explored different ways to make the ill-posed phase retrieval problem, i.e., recovering an image from its power spectrum, more tractable by introducing additional structure and constraints. These included structural constraints from opportunistic features such as a line reference (HERALDO), data-driven constraints from image priors learned by CNNs, and physics-based constraints from light-propagation models incorporated into physics-informed neural networks.

technologies_image: /assets/images/subprojects/coherent-imaging/fmcw-lidar-key-tech.svg
technologies_image_alt: FMCW LiDAR optical setup

applications: >
  Our techniques for phase retrieval and solving inverse problems in general could extend to coherent diffraction imaging and semiconductor metrology, where X-ray diffraction patterns are used to reconstruct nanoscale features, identify defects, and characterize complex 3D semiconductor structures. Our mathematical modeling of light propagation in complex geometries could also support holographic AR/VR displays, where modelling propagation between highly tilted or non-parallel surfaces presents unique challenges.

publications:
  - fmcw-paper-1
  - fmcw-paper-2
---