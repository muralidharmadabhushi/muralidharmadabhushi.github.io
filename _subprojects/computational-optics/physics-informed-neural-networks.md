---
layout: research-project
title: Physics-informed Neural Networks
project_id: pinn
nav_id: projects
order: 2
category_id: computational-optics
category_title: Computational Optics
category_url: /projects/computational-optics.html
image: /assets/images/subprojects/computational-optics/physics-informed-neural-networks.svg
image_alt: Physics-informed Neural Networks figure
#brief_image: /assets/images/subprojects/computational-optics/physics-informed-neural-networks.svg
#brief_image_alt: Physics-informed Neural Networks figure
technologies_title: "Under the Hood"
applications_title: "Broader Applications"
brief: >
  We developed a physics-informed neural network framework for solving ill-posed inverse problems, leveraging the expressive power and implicit regularization of deep neural networks. The neural network provides a flexible representation of the unknown solution, while a task-specific physical model constrains the solution to agree with actual measurements. This allows us to solve the inverse problem by optimizing the network for measurement consistency, without requiring labeled training data.
technologies: >
  - We designed the framework to be modular, allowing us to solve fundamentally different inverse problems by simply swapping the physical model. We demonstrated this across three applications: computer-generated holography (CGH), phase unwrapping, and indirect imaging correlography for looking around corners.
  
  - We explored different neural network architectures, including convolutional neural networks (CNNs) and coordinate-based multilayer perceptrons, to represent unknown solutions. We applied these to problems including phase unwrapping in interferometric synthetic aperture radar (InSAR) and fringe projection, each requiring a different physical model.
  
  - We extended our indirect imaging correlography approach to reconstruct complex, high-resolution images of objects hidden around corners, including text in unfamiliar languages. This is particularly challenging under noisy measurement conditions, where collecting representative training data is difficult and conventional supervised learning approaches may struggle to generalize.
  
#technologies_image: /assets/images/subprojects/coherent-imaging/fmcw-lidar-key-tech.svg
#technologies_image_alt: FMCW LiDAR optical setup

applications: >
  Our physics-informed neural network framework could extend to diffuse optical tomography (DOT) for reconstructing tissue properties from scattered light, and applications like imaging through atmospheric turbulence for recovering images distorted by turbulent air. Similar physics-informed approaches could also support computational lithography and semiconductor manufacturing applications, where inferring nanoscale structural information from diffraction patterns measured using EUV light is a challenging inverse problem.
publications:
  - fmcw-paper-1
  - fmcw-paper-2
---