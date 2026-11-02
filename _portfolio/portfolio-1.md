---
title: "Modelling fracture and contact in geomaterials"
excerpt: <img src="https://pkc137.github.io/sudo_template_website/images/Graphical_abs.png" width="550">
collection: portfolio 

---

Modeling fracture in geomaterials having distinct strength and stiffness is complex due to their unique occurrence of crack branching, coalescence, and interaction patterns. Fractures in such materials are often initiated by contact-induced loading conditions, including joint slip, fault activation, and penetration. Accurately capturing the interplay between contact and fracture mechanics remains a challenge for computational modeling of rocks. This study addresses this fundamental duality by proposing a coupled Peridynamics–Discrete Element Method (PD-DEM) framework with realistic damage and contact models.

Rock fracture: Brazilian disc test
------
The Brazilian (indirect tensile) test loads a rock disc in compression across its diameter until it splits. The simulation captures the splitting crack that forms along the loaded diameter.

<div style="display: flex; justify-content: center;">
  <figure style="text-align: center; max-width: 600px; margin: 1em 0;">
    <video style="width: 100%;" autoplay loop muted playsinline controls>
      <source src="https://pkc137.github.io/sudo_template_website/images/brazilian_disc.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
    <figcaption style="width: 100%; font-size: 0.9em; margin-top: 5px;">Brazilian disc (64 mm diameter) compressed between two platens: damage on the face of the disc</figcaption>
  </figure>
</div>

Rock fracture at high strain rates
------
Under impact, rock is loaded at very high strain rates, which changes its strength and the way it fragments. Here a 10 mm steel ball strikes a free 100 mm rock cube at 2 km/s, with a rate-dependent strength and Weibull-distributed heterogeneity in the rock.

<div style="display: flex; justify-content: center;">
  <figure style="text-align: center; max-width: 320px; margin: 1em 0;">
    <img src="https://pkc137.github.io/sudo_template_website/images/impact_setup.jpg" style="width: 100%;">
    <figcaption style="width: 100%; font-size: 0.9em; margin-top: 5px;">(a) Setup: 10 mm steel ball impacting a 100 mm rock cube at 2 km/s</figcaption>
  </figure>
</div>

<div style="display: flex; flex-wrap: wrap; justify-content: center; gap: 20px;">
  <figure style="flex: 1 1 320px; max-width: 420px; text-align: center; margin: 1em 0;">
    <video style="width: 100%;" autoplay loop muted playsinline controls>
      <source src="https://pkc137.github.io/sudo_template_website/images/impact_radial_cracks.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
    <figcaption style="width: 100%; font-size: 0.9em; margin-top: 5px;">(b) Radial cracks, seen from above on a cut 25 mm below the impacted face</figcaption>
  </figure>

  <figure style="flex: 1 1 320px; max-width: 420px; text-align: center; margin: 1em 0;">
    <video style="width: 100%;" autoplay loop muted playsinline controls>
      <source src="https://pkc137.github.io/sudo_template_website/images/impact_crack_network.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
    <figcaption style="width: 100%; font-size: 0.9em; margin-top: 5px;">(c) Crack network: all material points with damage ≥ 0.1</figcaption>
  </figure>
</div>

Contact-induced fracture: crushing of rock ballast
------
The pictures below show the continuous crushing process in rock ballast simulated by the PD-DEM framework.

<img src="https://pkc137.github.io/sudo_template_website/images/LS_DEM_2.png" width="600">


<img src="https://pkc137.github.io/sudo_template_website/images/total_fabric.png" width="600">
