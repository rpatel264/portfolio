---
layout: page
title: Walking Gait Modeling
description: Analyzing joint angles and torques during uphill and level walking using biomechanical simulation tools.
img: assets/projectimages/slope/skeletalmodel.png
importance: 3
category: work
related_publications: false
---
<!-- 🧭 Project Overview -->
<h4 class="text-center mt-5">Project Overview</h4>
<div class="text-center my-4">
This project focused on evaluating how walking on inclined versus flat surfaces affects human joint mechanics. Using OpenSim, we simulated gait patterns to measure changes in joint angles and torque across different terrains.
</div>

<div class="row">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/projectimages/slope/skeletalmodel.png" title="Blade Profiles" alt="Comparing multiple blade designs" class="img-fluid rounded z-depth-1" style="height: 250px; object-fit: contain;" %}
  </div>
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/projectimages/slope/downhillimage.png" title="Finalized Profile" alt="CAD model showing finalized blade profile" class="img-fluid rounded z-depth-1" style="height: 250px; object-fit: contain;" %}
  </div>
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/projectimages/slope/graphdata.png" title="Aluminum Prototype" alt="Machined aluminum blade prototype" class="img-fluid rounded z-depth-1" style="height: 250px; object-fit: contain;" %}
  </div>
</div>

<div class="caption">
We recorded video footage of subjects walking on flat and sloped surfaces, then used motion tracking software to extract kinematic data. These datasets were imported into OpenSim, allowing us to create skeletal models and run dynamic simulations for each scenario. 
</div>

<!-- 🔧 Final Outcome -->
<h4 class="text-center mt-5">Final Outcome</h4>
<div class="text-center my-4">
Our simulations revealed key differences in joint loading and movement patterns when walking on inclined surfaces compared to level ground. This insight contributes to broader research in gait analysis and rehabilitation, especially for individuals with mobility impairments or post-injury recovery needs.
</div>

