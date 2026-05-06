---
layout: project
title: The Crusher — Client Report
description: MAE 2250 Client Report
technologies: N/A
image: assets/images/clientreport_title.png
subcollection: true
---

My group created a final report to submit to our clients in the course MAE 2250, Cornell CALS Extension, E & J Gallo Winery, and National Grape.

[Download the PDF of the Client Report]({{ '/assets/ODP_6_Client_Report_Final.pdf' | relative_url }})

**Problem Statement & Context:**

Vineyard owners across New York State are affected by the rapid spread of Spotted Lanternflies
(SLF), whose presence in the Lake Erie and Finger Lakes regions alone could have projected losses
reaching approximately $8.8 million within three years [1]. A single SLF egg mass contains 30–50 eggs,
and populations can spread rapidly across large areas of vineyard land. To effectively address this spread,
reduce proliferation, and prevent these economic losses from spreading to other parts of the nation, these
invasive insects should be targeted while in their egg stage. Destroying eggs prevents the flies from
maturing into reproductive adults, reducing the number of SLF that will lay future egg masses and
limiting their exponential population growth. Our team focused on developing a mechanical solution for
large-scale egg mass destruction that can be deployed at the vineyard level.

Current elimination methods are not suitable for addressing large-scale SLF populations.
Manually crushing individual egg masses is time-consuming and inconsistent. Submersion into rubbing
alcohol requires constant refilling and storage capacity. Experimental oil ovicides are only effective on
75% of eggs [2]. Additional consideration must be given to the consequences of ineffective elimination,
as even one surviving egg mass can enable SLF persistence, escalating plant damage and contaminated
harvests.

There is a need for a systematic method for eliminating large quantities of SLF egg masses that
can be integrated into existing collection workflows. This method must be consistently effective, practical
for real-world use, while minimizing storage, disposal, and labor demands on vineyard operations during
implementation.

---

**Final Prototype and Application:**

We developed a device that mechanically crushes eggs, utilizing a juicer-inspired crushing mechanism.
How it works:
- Eggs masses enter the mesh cylinder chamber through an inlet funnel.
- A rotating spiral, driven by an electric motor, transports the egg masses downward while
simultaneously pressing the eggs against the mesh cylinder, where the crushing occurs.
- A sweeper attached to the rotating spiral pushes crushed eggs towards a hole in the bottom of the
mesh housing, falling out of the device through an outlet funnel.

This device will be deployed in the field alongside the given collection method that best suits the
vineyard's needs, such as a manual scraper or an autonomous scraping robot. The device is modular, such
that its method of accepting and ejecting egg masses can be easily changed.

---

**Conclusion and Recommendation:**

We would recommend the continued research and development of the Egg Crusher for
applications in vineyards. The device in its current form is a successful proof of concept for a scalable,
efficient, and practical egg extermination method, demonstrating basic mechanical motion. Its ~80%
crushing efficiency is on par with current methods, without the drawbacks of consistent maintenance or
manual labor. Additionally, its 100% efficiency for ejecting crushed eggs of a standardized diameter
suggests the crushed eggs can be re-incorporated into the ecosystem as a compost ingredient if desired by
the vineyard owners.

We would suggest three primary redesigns in future phases of this project:

1. Spiral and sweeper geometry. Pitch angle, spiral diameter, and other features can be optimized to
improve crushing efficiency and properly push the crushed eggs towards the outlet funnel.
2. Compactness. The system can be scaled down to reduce weight and improve portability, making
it easier to deploy in the field alongside a collection device.
3. Contingency mechanisms. Incorporating multiple built-in crushing mechanisms arranged in a
linear series can improve crushing efficiency, as eggs not crushed by the first spiral will be
crushed by the second crushing mechanism right below.

---

**Testing and Results:**

Using hydrated Orbeez as model SLF eggs due to their comparable size and material properties as well as
their uniformity, we were able to test:

1. The dependence of the quantity of inputted eggs on machine ef iciency.

We wanted to determine if the system had an optimal loading range. Results showed that efficiency
decreases as quantity increases beyond the optimal operating load. Trials with 50 eggs produced a
crushing efficiency range of 72-92% with an average crushing efficiency of 82%. With trials of 100 eggs,
the crushing efficiency dropped to a range of 64-78% with an average crushing efficiency of 72%. This
indicates that overcrowding inside the chamber restricts motion and reduces effective processing, limiting
throughput at higher loads. However, it does also indicate that the device is suitable for crushing one egg
mass at a time which contains anywhere from 30-50 eggs.

2. The dependence of operation time on machine ef iciency.

We wanted to determine whether longer runtime improves performance. Across both 90 second and 3
minute trials with 100 eggs, results showed minimal or no improvement over time. Crushing efficiency
remained within similar ranges of 64-78% with an average crushing efficiency of 72% for 90 seconds and
65-78% with an average crushing efficiency of 71% for 3 minutes. This suggests that the system reached
a steady-state operating condition quickly which means that extending the operating time of the system
does not significantly enhance crushing performance once equilibrium is reached. This indicates that our
device can limit the amount of energy used as increasing the operating time does not increase the crushing
efficiency.

3. The system failure rate.

Finally, we evaluated the system failure rate which we defined as eggs that made it through the device
uncrushed. Across all trials, with our standard Orbeez model egg size of ⅛", no uncrushed eggs were
observed indicating a 0% failure rate under these standardized conditions. In the cases where an
uncrushed Orbeez made it through the device, the Orbeez tended to be less hydrated and smaller
measuring closer to 1/16" rather than ⅛".

Key outcomes:
- Optimal performance occurs at lower to moderate input quantities as the 50-100 eggs range
shows diminishing returns as the load increases
- Time is not a limiting factor after initial steady-state is reached, 90 seconds seems to be sufficient
- System reliability is high, with effectively complete crushing under tested conditions

---

**Prototype and Testing Details:**

Our design draws inspiration from juicer systems, where material is guided through a rotating
spiral and compressed against an abrasive mesh surface. Similarly, our device crushes input SLF egg
masses by forcing them downward through a rotating central spiral against a fixed mesh barrier. This
approach prioritizes compactness, portability, and compatibility with future system integration.

Following initial mock-ups to determine overall dimensions and structural layout, we developed
multiple iterative prototypes to address challenges in spiral alignment, clearance tolerances, and material
flow. The final functional prototype is shown in the figure below, which illustrates the full system
architecture and component interactions.

![Assembly diagram of the Egg Crusher prototype]({{ '/assets/images/assembly_diagram.png' | relative_url }})

**Component Specifications and Assembly:**

The final prototype consists of nine 3D-printed PLA components
fabricated using the Rapid Prototyping Lab, integrated with purchased
mechanical and electrical components. The central crushing mechanism
utilizes a McMaster 6409K17 compact DC gearmotor (12V DC, 26 rpm,
320 in-oz torque) to drive a custom-designed spiral shaft assembly. The
crushing chamber features a cylindrical mesh housing that secures a 304
stainless steel mesh cylinder (20x20 mesh, 0.034" openings) flush against
the rotating spiral. For enhanced filtration, a secondary fine mesh layer
(270x270 mesh, 0.0023" openings) provides additional crushing precision.
The spiral geometry was iteratively optimized through multiple prototypes
to achieve proper clearance tolerances and material flow characteristics.
Assembly is achieved through M3 x 25mm Phillips head screws
(McMaster 99461A948) that secure the mesh housing to the motor
housing, while the motor itself is mounted with dedicated bolts. A toggle
switch (SPST-NO, 6A rating, McMaster 7343K184) provides simple on/off
control. The modular design allows for easy disassembly for maintenance
or component replacement. Material flow follows a consistent path: egg
masses enter through the inlet funnel, are transported downward by the spiral while being compressed
against the mesh barrier, and crushed material exits via the sweeper-directed outlet funnel. The entire
assembly weighs approximately 2.5 pounds and measures roughly 12 inches in height, making it suitable
for field deployment alongside existing collection workflows.

---

**References**

[1] A. F. Pinto, B. C. Eshenaur, F. E. Acevedo, A. A. Calixto, M. Centinari, and M. I. Gómez, "Assessing
the potential economic impacts of spotted lanternfly (Hemiptera: Fulgoridae) infestations on grape
production in New York State," Journal of Integrated Pest Management, vol. 16, no. 1, 2025. [Online].
Available: <https://doi.org/10.1093/jipm/pmae039>

[2] G. Krawczyk, "What should you do with spotted lanternfly egg masses?" Penn State Extension.
[Online]. Available: <https://extension.psu.edu/what-should-you-do-with-spotted-lanternfly-egg-masses>

---

## Bill of Materials

<style>
  .bom-scroll-wrapper {
    overflow-x: auto;
    -webkit-overflow-scrolling: touch;
    border: 1px solid #444;
    border-radius: 6px;
    margin-bottom: 2rem;
    box-shadow: inset -6px 0 10px -6px rgba(0,0,0,0.3);
  }
  .bom-scroll-wrapper table {
    min-width: 900px;
    border-collapse: collapse;
    font-size: 0.85rem;
    width: 100%;
    background-color: #2a2a2a;
    color: #fff;
  }
  .bom-scroll-wrapper th {
    background-color: #111;
    color: #fff;
    padding: 8px 12px;
    text-align: left;
    white-space: nowrap;
    border-bottom: 2px solid #555;
  }
  .bom-scroll-wrapper td {
    padding: 7px 12px;
    border-bottom: 1px solid #444;
    vertical-align: top;
    background-color: #2a2a2a;
    color: #fff;
  }
  .bom-scroll-wrapper tr.total-row td {
    background-color: #111;
    color: #fff;
    font-weight: bold;
    border-top: 2px solid #555;
  }
  .bom-label {
    font-size: 0.78rem;
    color: #888;
    margin-bottom: 4px;
    font-style: italic;
  }
  .grand-total-table {
    border-collapse: collapse;
    font-size: 0.9rem;
    margin-top: 0.5rem;
    width: 100%;
    max-width: 400px;
    background-color: #2a2a2a;
    color: #fff;
  }
  .grand-total-table th {
    background-color: #111;
    color: #fff;
    padding: 8px 14px;
    text-align: left;
    border-bottom: 2px solid #555;
  }
  .grand-total-table td {
    padding: 7px 14px;
    border-bottom: 1px solid #444;
    background-color: #2a2a2a;
    color: #fff;
  }
  .grand-total-table tr.total-row td {
    background-color: #111;
    color: #fff;
    font-weight: bold;
    border-top: 2px solid #555;
  }
</style>

### Utilized in the Prototype

<div class="bom-scroll-wrapper">
  <table>
    <thead>
      <tr>
        <th>Part Name</th>
        <th>Quantity</th>
        <th>Unit of Measurement</th>
        <th>Source</th>
        <th>Specs</th>
        <th>Supplier/Process</th>
        <th>Cost ($)</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>Spiral</td>
        <td>1</td>
        <td>Each</td>
        <td>Fabricated</td>
        <td>238.500 grams, Light Gray PLA</td>
        <td>RPL (3D Print)</td>
        <td>11.93</td>
      </tr>
      <tr>
        <td>Spiral Shaft</td>
        <td>1</td>
        <td>Each</td>
        <td>Fabricated</td>
        <td>22.571 grams, Light Gray PLA</td>
        <td>RPL (3D Print)</td>
        <td>1.13</td>
      </tr>
      <tr>
        <td>Mesh Housing (Top)</td>
        <td>1</td>
        <td>Each</td>
        <td>Fabricated</td>
        <td>122.384 grams, Light Gray PLA</td>
        <td>RPL (3D Print)</td>
        <td>6.12</td>
      </tr>
      <tr>
        <td>Mesh Housing (Bottom)</td>
        <td>1</td>
        <td>Each</td>
        <td>Fabricated</td>
        <td>143.625 grams, Light Gray PLA</td>
        <td>RPL (3D Print)</td>
        <td>7.18</td>
      </tr>
      <tr>
        <td>Inlet Funnel</td>
        <td>1</td>
        <td>Each</td>
        <td>Fabricated</td>
        <td>100.636 grams, Light Gray PLA</td>
        <td>RPL (3D Print)</td>
        <td>5.03</td>
      </tr>
      <tr>
        <td>Motor Housing (Top)</td>
        <td>1</td>
        <td>Each</td>
        <td>Fabricated</td>
        <td>116.623 grams, Light Gray PLA</td>
        <td>RPL (3D Print)</td>
        <td>5.83</td>
      </tr>
      <tr>
        <td>Motor Housing (Bottom)</td>
        <td>1</td>
        <td>Each</td>
        <td>Fabricated</td>
        <td>325.375 grams, Light Gray PLA</td>
        <td>RPL (3D Print)</td>
        <td>16.27</td>
      </tr>
      <tr>
        <td>Switch Holder</td>
        <td>1</td>
        <td>Each</td>
        <td>Fabricated</td>
        <td>6.118 grams, Light Gray PLA</td>
        <td>RPL (3D Print)</td>
        <td>0.31</td>
      </tr>
      <tr>
        <td>Sweeper</td>
        <td>1</td>
        <td>Each</td>
        <td>Fabricated</td>
        <td>0.578 grams, Light Gray PLA</td>
        <td>RPL (3D Print)</td>
        <td>0.03</td>
      </tr>
      <tr>
        <td>Motor</td>
        <td>1</td>
        <td>Each</td>
        <td>Purchased</td>
        <td>Compact DC Gearmotor, Square Face, 12V DC, 26 rpm @ 320 in.-oz.</td>
        <td>McMaster (6409K17)</td>
        <td>72.64</td>
      </tr>
      <tr>
        <td>Switch</td>
        <td>1</td>
        <td>Each</td>
        <td>Purchased</td>
        <td>Toggle Switch, 2 Position, Round, Maintained, 2 Terminal, SPST-NO, 6A, Tab Terminal</td>
        <td>McMaster (7343K184)</td>
        <td>8.96</td>
      </tr>
      <tr>
        <td>Mesh Cylinder</td>
        <td>1x1</td>
        <td>Feet</td>
        <td>Purchased</td>
        <td>304 Stainless Steel Filter Mesh, 20 x 20 Mesh Size, 0.034" Opening Size, 1 ft x 1 ft</td>
        <td>McMaster (85385T73)</td>
        <td>15.2</td>
      </tr>
      <tr>
        <td>Outlet Funnel</td>
        <td>1</td>
        <td>Each</td>
        <td>Purchased</td>
        <td>Standard-Wall PVC Pipe 45 Degree Elbow Connector, White, 3/4 Socket, Connect Female</td>
        <td>McMaster (4880K32)</td>
        <td>1.45</td>
      </tr>
      <tr>
        <td>M3 Screws</td>
        <td>1</td>
        <td>Pack of 50 Each</td>
        <td>Purchased</td>
        <td>Phillips Rounded Head Screws for Plastic, 18-8 Stainless Steel, M3 Screw Size, 25 mm Long</td>
        <td>McMaster (99461A948)</td>
        <td>10.91</td>
      </tr>
      <tr>
        <td>Fine Mesh</td>
        <td>1x2</td>
        <td>Feet</td>
        <td>Purchased</td>
        <td>Stainless Steel, 270 x 270 mesh size, 0.0023'' Opening</td>
        <td>McMaster (85385T113)</td>
        <td>32.57</td>
      </tr>
      <tr class="total-row">
        <td>Total Prototype Price</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td>195.56</td>
      </tr>
    </tbody>
  </table>
</div>

### Additional Project Expenses

<div class="bom-scroll-wrapper">
  <table>
    <thead>
      <tr>
        <th>Part Name</th>
        <th>Quantity</th>
        <th>Source</th>
        <th>Specs</th>
        <th>Supplier/Process</th>
        <th>Cost ($)</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>Mesh Housing (Bottom) - 0</td>
        <td>1</td>
        <td>Fabricated</td>
        <td>116.744 grams, Light Gray PLA</td>
        <td>RPL (3D Print)</td>
        <td>5.84</td>
      </tr>
      <tr>
        <td>Mesh Housing (Top) - 0</td>
        <td>1</td>
        <td>Fabricated</td>
        <td>146.875 grams, Light Gray PLA</td>
        <td>RPL (3D Print)</td>
        <td>7.34</td>
      </tr>
      <tr>
        <td>Spiral - 0</td>
        <td>1</td>
        <td>Fabricated</td>
        <td>198.400 grams, Light Gray PLA</td>
        <td>RPL (3D Print)</td>
        <td>9.92</td>
      </tr>
      <tr>
        <td>Shaft - 0</td>
        <td>1</td>
        <td>Fabricated</td>
        <td>11.988 grams, Light Gray PLA</td>
        <td>RPL (3D Print)</td>
        <td>0.6</td>
      </tr>
      <tr>
        <td>Motor Housing</td>
        <td>1</td>
        <td>Fabricated</td>
        <td>275.303 grams, Light Gray PLA</td>
        <td>RPL (3D Print)</td>
        <td>13.77</td>
      </tr>
      <tr>
        <td>Spiral - 2</td>
        <td>1</td>
        <td>Fabricated</td>
        <td>241.859 grams, Light Gray PLA</td>
        <td>RPL (3D Print)</td>
        <td>12.09</td>
      </tr>
      <tr class="total-row">
        <td>Total Additonal Price</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td>49.56</td>
      </tr>
    </tbody>
  </table>
</div>

### Total Project Cost

<table class="grand-total-table">
  <thead>
    <tr>
      <th>Total Project Cost</th>
      <th>Cost ($)</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Prototype</td>
      <td>195.56</td>
    </tr>
    <tr>
      <td>Additional</td>
      <td>49.56</td>
    </tr>
    <tr class="total-row">
      <td>Grand Total</td>
      <td>245.12</td>
    </tr>
  </tbody>
</table>

---

## Project Poster


<div style="width:100%; max-width:850px; margin: 2rem auto;">
  <img src="{{ '/assets/images/ODP_Poster_Draft.png' | relative_url }}" alt="Project Poster" style="width:100%; height:auto; display:block;">
</div>
