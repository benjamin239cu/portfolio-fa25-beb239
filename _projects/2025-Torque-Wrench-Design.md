---
layout: project
title: Torque Wrench Design
description: Autodesk Fusion, ANSYS Project
technologies: [Autodesk Fusion, ANSYS]
image: /assets/images/TorqueWrenchRendered.jpg
---

Anyone whose used a torque wrench or other hand tool knows that one of the most important attributes of the material and design chosen is life cycle. In choosing a material for my design, I opted for one which I could confidently say would last longer than a user would ever need it, and a design that would never fail them. I chose a low alloy steel, specifically AISI 9255, oil quenched and tempered at 205 degC. I specifically searched for a material that had been tempered and hardened using metal cold, hot, and press forming to remove deformations and imperfections in an otherwise untempered material. The steel has a Young’s Modulus of 31.3E6 psi, yield strength of 327 ksi, Poisson’s ratio of 0.295, and fatigue strength at 106 cycles of 102 ksi. A picture depicting the dimensions of the torque wrench is shown below.

![Dimensions of wrench]({{ "/assets/images/TorqueWrench-Dimensions.png" | relative_url }}){: style="width: 1000px"}

Using ANSYS requires finding the governing equation of the model, which primarily means inputting the Young's Modulus and Poisson's Ratio of the materials used in your model.  

![Boundary condition setting process]({{ "/assets/images/BCDiagram.png" | relative_url }}){: style="width: 900px"}

Using FEM, I was able to analyze the normal strain and maximum principal stresses using contour plots created in ANSYS. Using the FEM, I found a torque wrench sensitivity of 1.0064 mV/V. Finally, for my design, I selected the SGD-1.5/120-LY41 Precision Strain Gauge from Omega, with dimensions of 0.185 in x 0.134 in.

![Normal strain contours from FEM]({{ "/assets/images/NormalStrain.png" | relative_url }}){: style="width: 700px"}

![Strain at strain gauge]({{ "/assets/images/StrainGauge.png" | relative_url }}){: style="width: 700px"}

![Normal Stress, FEM]({{ "/assets/images/NormalStress.png" | relative_url }}){: style="width: 700px"}  

![Deflection of load point, FEM]({{ "/assets/images/LoadPointDeflection.png" | relative_url }}){: style="width: 700px"}  

![Max principal stress, FEM]({{ "/assets/images/MaxPrincStress.png" | relative_url }}){: style="width: 700px"}  