---
layout: project
title: Pressure Washer Nozzle Analysis
description: Thermodynamics (MAE 2210) Device Analysis
technologies: N/A
image: assets\images\327681193_RM_RYOBI.jpg
---

For my Thermodynamics course (MAE 2210), we were asked to select a real-world instance of the devices we studied in the course, explain its functions, perform an analysis of the system with methods learned in the course, and discuss how changes in its operating conditions would impact performance.

![Chart of pressure washer nozzle ratings]({{ "assets\images\pressure_washer_nozzles_v3-01_1.jpg" | relative_url }}){: .inline-image-r style="width: 200px"}

A pressure washer nozzle is an interchangeable attachment for a pressure washing device, altering the outcoming stream flow to best suit the desired task. I focused my analysis on Quick Connect (QC) nozzles. By industry standards, a QC nozzle is categorized based on the spray angle, that is the divergence of the fluid flow upon exiting the nozzle. Smaller angles produce more concentrated, powerful streams. They are color-coded by their spray angle, as outlined by the chart to the right (1). They are also categorized by their orifice size, which is the nozzle opening that releases the spray. The inlet opening, where the nozzle attaches to the washer hose, is a standard diamater of 0.25 inches.

The most deciding factors in choosing a nozzle are the required concentration of flow, and the specifications of the pressure washer to be utilized - the operable pressure and fluid flow rate. Usually, the machine is rated in pounds per square inch (PSI) and gallons per minute (GPM), respectively (2). These two operating characteristics can be used to determine the desired orifice size, which are usually tabulated on a reference chart.

![Image of QC Nozzle Kit]({{ "assets\images\nozzle-kit.jpg" | relative_url }}){: .inline-image-l style="width: 200px"}

For my analysis, I will assume the pressure washer is the RYOBI 1.8 GPM Automotive High Flow Pressure Washer (3), which is rated at 1200 PSI and 1.8 GPM. I will analyze the 25° QC nozzle from RAW Industrial Supplies Nozzle Kit Legacy 4/PK (4), which is shown to the left.

I'll determine the appropriate nozzle size using the chart below, provided by RAW Industrial Supplies. For my washer, a standard nozzle size of 3.5, which corresponds to a hole diameter of 0.048 inches, is appropriate.

![PSI_GPM chart to determine nozzle sizing]({{ "assets\images\raw-industrial-nozzle-sizing-real.jpg" | relative_url }}){: .full-width-image}

For my system analysis, I made the following assumptions:

- I used a control volume approach (analysis of one particular volume in space that mass was allowed to exit/enter) - Assumed steady state operation of the nozzle (change in energy and mass flow rate is zero)
- The fluid moves very quickly through the nozzle, therefore assume an adiabatic process (no heat transfer)
- The fluid velocity is perpendicular to the inlet and outlet crosssectional area
- Assume the fluid moving through the nozzle to be cold liquid water at 50 °F. I will treat it as incompressible, such that the density of the water remains constant and there is one specific heat coefficient. The density and specific heat values used can be found at (5), from the water property table for 1000 psia, which was within magnitude of the gauge pressure of the pressure washer.
- Assume negligible change in potential energy in the nozzle. 

Below is my device analysis. I drew a simplified system diagram, determined the inlet velocity, outlet velocity, mass flow rate, and outlet temperature of the fluid passing through the nozzle.

![QC nozzle analysis]({{ "assets\images\thermo - hw.jpeg.png" | relative_url }}){: .full-width-image}

From this analysis, I've determined that the nozzle converts the water's enthalpy into kinetic energy, resulting in the decrease of the water's temperature. This temperature difference is directly related to the difference in the square of the velocities, which is dependent on the ratio of the cross-sectional inlet and outlet areas.

The operating conditions that can be altered to better performance are the machine's PSI and GPM ratings. From the reference chart, it can be noted that increasing the PSI allows a smaller GPM for the same nozzle size. Thus, the same velocity difference can be achieved for less fluid overall. However, this is only a benefit depending on the desired usage of the pressure washer. If the goal is to strip paint or stains from a small area, then achieving more power from less fluid is a great benefit. On the other hand, if the goal is to spray a large area, such as an entire house, then more fluid flow would be needed. Ultimately, the best nozzle performance, which can be determined from the velocity difference at inlet and outlet, is dependent on the application of the nozzle. It is also of note that the velocity difference and this first law analysis is independent of the spray angle. The actual dispersion of the outlet stream is dependent on the design of the nozzle itself, and the indentation geometry of the nozzle head around the orifice.

___________________________________________________________________________________________________________________



References:

*(Cover) Image : <a href="https://www.homedepot.com/b/Outdoors-Outdoor-Power-Equipment-Pressure-Washers/N-5yc1vZbxbe" target="_blank" rel="noopener">Source</a>*

*(1) Image : <a href="https://skyvac.com/product/coloured-nozzles-pack-for-pressure-washers/" target="_blank" rel="noopener">Source</a>*

*(2) Reference : <a href="https://americanpressureinc.com/blog/gpm-psi-and-choosing-the-right-nozzle/" target="_blank" rel="noopener">Source</a>*

*(3) Reference : <a href="https://www.homedepot.com/p/RYOBI-1200-PSI-1-8-GPM-Cold-Water-Automotive-High-Flow-Electric-Pressure-Washer-Kit-RY14AM12/333071566" target="_blank" rel="noopener">Source</a>*

*(4) Reference : <a href="https://share.google/czvtxoYs3I8UIX51u" target="_blank" rel="noopener">Source</a>*

