---
layout: project
title: "Fluids Final Project"
permalink: /projects/fluids/
image: /assets/images/CAD-for-blade.png
summary: Wind-tunnel validated 6-inch turbine blade using BEMT-driven geometry and SLA prototype hardware.
---
<section class="project-hero">
  <p class="text-muted mb-2">MAE 4272 · Blade Design Project</p>
  <h2>Wind Turbine Blade for Laboratory Test Rig</h2>
  <p class="lead">Designed, fabricated, and validated a 6-inch diameter, high-efficiency blade that exceeded predicted output in wind-tunnel testing.</p>
  <div class="metrics-grid">
    <div class="metric-card">
      <span>Blade Diameter</span>
      <strong>6 in</strong>
    </div>
    <div class="metric-card">
      <span>Design TSR</span>
      <strong>≈3</strong>
    </div>
    <div class="metric-card">
      <span>Stress Limit</span>
      <strong>44 MPa</strong>
    </div>
    <div class="metric-card">
      <span>Test Output</span>
      <strong>1.29 W</strong>
    </div>
  </div>
</section>

### Project Overview
The MAE 4272 brief tasked our team with creating a 6-inch wind turbine blade that could be 3D printed, survive a 44 MPa flexural limit, and deliver competitive power when mounted in Cornell’s wind-tunnel fixture. We selected the NACA 4412 airfoil and engineered the geometry so the turbine could be shared with industry recruiters as a concise demonstration of aerodynamic design, structural verification, and data-driven validation.

We approached the work as a condensed engineering program: translating customer constraints (diameter, axial projection, manufacturability) into aerodynamic targets, modeling the blade with Blade Element Momentum Theory (BEMT), and building in the instrumentation needed to learn from static and dynamic tests. The result is a manufacturable blade that met every design constraint and achieved higher-than-predicted output.

### Design Process
- **BEMT-driven geometry:** Interpolated NACA 4412 airfoil data across multiple Reynolds numbers and ran full-span BEMT convergence to align chord, pitch, and thrust profiles with the desired 5.04 m/s design wind speed.
- **Root/tip smoothing:** Applied quadratic root blending and linear tip smoothing to eliminate numerical noise and enforce continuous geometry that prints cleanly and sheds stress concentrations.
- **Structural verification:** Modeled flapwise bending loads and material utilization to keep peak stress well below the 44 MPa requirement with safety margin for resonance regions.
- **Manufacturability & assembly:** Packaged mounting hardware inside the axial projection limit (2 inches) and produced jigs that preserved twist accuracy during post-processing.

### Testing & Results
We fabricated the blade via SLA 3D printing, balanced it, and mounted it on the MAE torque-brake rig. Tests swept fan frequency and brake torque while logging wind speed, RPM, and electrical load to compute power and tip-speed ratio (TSR).

- **Performance:** Peak measured power of **1.29 W** at 5.56 m/s exceeded the ≈1.0 W prediction, even as the turbine operated around TSR ≈ 6 rather than the design point of 3.
- **Stability:** The blade rode through a resonance band at 2100–2500 RPM without structural degradation, validating the stress model.
- **Data insight:** The consistently high TSR indicates future revisions could be tuned for higher-speed operation to unlock additional performance.

### My Contribution
- Architected the BEMT modeling workflow, including Reynolds-number interpolation and chord/twist optimization routines.
- Led the smoothing, CAD detailing, and print preparation effort to ensure a manufacturable and structurally sound blade.
- Built the structural verification model and documented the load path to confirm compliance with the 44 MPa flex limit.
- Co-led the wind-tunnel test campaign, wiring instrumentation, capturing data, and comparing it to the analytical baseline.

### Figures
<div class="figure-grid">
  <figure class="figure-card">
    <img src="{{ '/assets/images/CAD-for-blade.png' | relative_url }}" alt="CAD render of the wind turbine blade geometry" loading="lazy">
    <figcaption>Blade geometry export highlighting the twist and chord distribution derived from BEMT.</figcaption>
  </figure>
  <figure class="figure-card">
    <img src="{{ '/assets/images/Performance-power-curves-for-blade.png' | relative_url }}" alt="Measured turbine power curves from the wind-tunnel tests" loading="lazy">
    <figcaption>Representative power vs. fan frequency curve from the wind-tunnel torque-brake sweep.</figcaption>
  </figure>
  <figure class="figure-card">
    <img src="{{ '/assets/images/Blades-in-hub.png' | relative_url }}" alt="Fabricated blades installed in the test hub" loading="lazy">
    <figcaption>3D-printed blades mounted in the hub for balance checks ahead of tunnel testing.</figcaption>
  </figure>
</div>

### Full Report & Supporting Data
- [View Full Fluids Final Report (PDF)]({{ '/assets/fluids/Fluids_Final_Report.pdf' | relative_url }})  
- GitHub Pages permalink: `{{ page.url | absolute_url }}`
