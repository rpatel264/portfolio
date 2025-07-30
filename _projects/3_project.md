<!-- 🧭 Project Overview -->
<h4 class="text-center mt-5">Project Overview</h4>
<div class="text-center my-4">
  This project focused on evaluating how walking on inclined versus flat surfaces affects human joint mechanics. Using OpenSim, we simulated gait patterns to measure changes in joint angles and torque across different terrains.
</div>

<!-- 🖼️ Image Gallery -->
<div class="row justify-content-center text-center mt-4">
  <div class="col-sm-4 mb-3">
    {% include figure.liquid loading="eager" path="assets/projectimages/slope/skeletalmodel.png" title="Skeletal Model" alt="Human skeletal model in OpenSim" class="img-fluid rounded z-depth-1" style="height: 250px; object-fit: contain;" %}
  </div>
  <div class="col-sm-4 mb-3">
    {% include figure.liquid loading="eager" path="assets/projectimages/slope/downhillimage.png" title="Downhill Walking Simulation" alt="Simulated gait for slope walking" class="img-fluid rounded z-depth-1" style="height: 250px; object-fit: contain;" %}
  </div>
  <div class="col-sm-4 mb-3">
    {% include figure.liquid loading="eager" path="assets/projectimages/slope/graphdata.png" title="Kinematic Data Graph" alt="Joint torque and angle graph" class="img-fluid rounded z-depth-1" style="height: 250px; object-fit: contain;" %}
  </div>
</div>

<div class="text-center caption mt-2 text-muted" style="font-size: 0.9rem;">
  We recorded video footage of subjects walking on flat and sloped surfaces, then used motion tracking software to extract kinematic data. These datasets were imported into OpenSim, allowing us to create skeletal models and run dynamic simulations for each scenario.
</div>

<!-- 🔧 Final Outcome -->
<h4 class="text-center mt-5">Final Outcome</h4>
<div class="text-center my-4">
  Our simulations revealed key differences in joint loading and movement patterns when walking on inclined surfaces compared to level ground. This insight contributes to broader research in gait analysis and rehabilitation, especially for individuals with mobility impairments or post-injury recovery needs.
</div>

