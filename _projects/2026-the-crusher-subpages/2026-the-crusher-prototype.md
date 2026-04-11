---
layout: project
title: The Crusher — Functional Prototype
description: MAE 2250 Functional Prototype Report
technologies: [CAD, 3D Printing, Rapid Prototyping]
image: /assets/images/prototype_thumbnail.jpg
subcollection: true
---

For my Introduction to Mechanical Design course (MAE 2250), our group the Vine Vanguard developed and tested a first functional prototype of The Crusher, a mechanical device designed to destroy Spotted Lanternfly egg masses after scraping.

---

# Vine Vanguard
# Functional Prototype

## Design Documentation

<table>
  <thead>
    <tr>
      <th>Part Name</th>
      <th>Quantity</th>
      <th>Source</th>
      <th>Specs</th>
      <th>Supplier/Process</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Fine Mesh</td>
      <td>1x2 Feet</td>
      <td>Purchased</td>
      <td>Stainless Steel, 270x270 mesh size, 0.0023" Opening</td>
      <td>McMaster (85385T113)</td>
    </tr>
    <tr>
      <td>Spiral</td>
      <td>1</td>
      <td>Fabricated</td>
      <td>PLA, Volume 1.984E+08 mm³</td>
      <td>3D Print (RPL)</td>
    </tr>
    <tr>
      <td>Spiral Shaft</td>
      <td>1</td>
      <td>Fabricated</td>
      <td>PLA, Volume 1.198E+07 mm³</td>
      <td>3D Print (RPL)</td>
    </tr>
    <tr>
      <td>Mesh Housing (Top)</td>
      <td>1</td>
      <td>Fabricated</td>
      <td>PLA, Volume 1.173E+08 mm³</td>
      <td>3D Print (RPL)</td>
    </tr>
    <tr>
      <td>Mesh Housing (Bottom)</td>
      <td>1</td>
      <td>Fabricated</td>
      <td>PLA, Volume 9.819E+07 mm³</td>
      <td>3D Print (RPL)</td>
    </tr>
    <tr>
      <td>Inlet Funnel</td>
      <td>1</td>
      <td>Fabricated</td>
      <td>PLA, Volume 8.050E+07 mm³</td>
      <td>3D Print (RPL)</td>
    </tr>
  </tbody>
</table>

## Illustration of Design Intent:
Prototype components (CAD) and functions:

Prototype assembly:

## Design Tests

**Test 1:**
Does the device's assembly of press-fits remain intact during use?

**How this was tested:**
Completely construct device in accordance with intended assembly, including the insertion of the grid mesh, while noting any times where excessive force was required to connect parts. Firmly shake the device for 10 seconds, in upright and inverted positions. Inspect the entire device for any loosened or detached components.

**Result:**
- Primary Construction: The press-fits for the shaft-spiral and housing-funnel connection were securely fastened without excessive force. The tolerances for the connections between the housing top and bottom were inaccurate, and the two could not be press-fit together. Extra adhesion (duct-tape) was required to secure these two components. The mesh was secured easily into the housing groove.
- Post Shake Test: No loosen pieces were found in the device. The connected shaft and spiral slid in and out of the housing bottom when inverted.

**Required Changes:**
In next prototypes, we will alter the CAD geometries for the housing components so that they securely connect via press-fit.

**Test 2:**
Does the spiral properly rotate without jamming/getting blocked in its motion?

**How this was tested:**
Rotate the device manually through multiple full crushing cycles including before, during, and after the insertion of model egg masses (hydrated Orbeez). Observe whether or not the spiral experiences any resistance, blockage or misalignment during rotation. Testing was conducted over varying loads (no Orbeez, 20-30 Orbeez, 50 Orbeez) to simulate realistic operating conditions.

**Result:**
- Rotation Without Orbeez: The spiral rotated smoothly, with minimal resistance and no visible wobbling or misalignment of the shaft within the mesh housing.
- Rotation With Orbeez (during operation): Rotation became inconsistent once Orbeez were introduced. Some Orbeez became lodged beneath the spiral rather than being carried through the crushing mechanism. This created intermittent resistance and slight jamming. Additionally, it prevented many Orbeez from being fully crushed since there was no resistance between the spiral, the Orbeez, and the mesh.
- Mesh Interaction: Due to unforeseen ordering complications, we used a temporary replacement mesh for testing in our lab section. The openings of this replacement were approximately 8mm in diameter, while our partially hydrated Orbeez were about 3mm in diameter. This meant the Orbeez could simply fall through the mesh rather than being crushed against it by the spiral. We tried to rectify this by adding multiple layers of mesh in the housing to create smaller openings, but Orbeez would still fall through. Due to this large mesh opening size, during our prototype testing, Orbeez were not properly supported during rotation, further contributing to slipping and inconsistent contact with the spiral.

**Required Changes:**
 In next prototypes, we will add a guide or mechanical restraint such as little arms attached to the inside columns of the mesh housing to keep the spiral flush against the bottom of the mesh housing. This will prevent eggs from being trapped underneath and remain uncrushed during rotation. Additionally, as we originally planned, we will replace the temporary replacement mesh with much finer mesh to prevent Orbeez from slipping through the openings.

**Test 3:**
How efficient is the juicer inspired mechanism at crushing the egg masses? What percentage of eggs come out of the device entirely crushed?

**How this was tested:**
 Insert a standardized number of Orbeez (model SLF eggs) into the device. Manually crank the spiral shaft to engage the crushing mechanism for ~30 seconds. Divide the number of eggs that come out intact by the number of eggs inserted into the device. This will give us the percentage of eggs that were not destroyed. Repeat this process for numerous trials and average the percentages.

**Result:**
 As stated in Test 2, the inaccurate sizing for the replacement mesh meant that our trials did not produce crushed Orbeez. However, the trials allowed us to examine the model eggs' motion throughout the crushing process.

- Spiral Design: We observed that the spiral's egg-like shape, which tapered out to the diameter of the housing mesh groove then tapered in, allowed Orbeez to accumulate at the housing bottom. The current design had no method to move the settled eggs outside of inverting the device.
- Mesh Stability: The interactions between the spiral and the mesh were observed. We suspect that the mesh will not be stable enough in the groove to withstand the lateral load of eggs pushed into it by the spiral at regular operation.

**Required Changes:**
 To address the accumulation of Orbeez at the housing bottom, the spiral will be redesigned to not taper in towards its base. Adjustments to the mesh will be explored to make it more secure against the eggs pressing against it. Configurations such as a 3D printed cylinder with cutouts for mesh pieces, a 3D printed cylinder with an embedded mesh design, and a solid cylindrical column with internal sandpaper lining may be tested.

## Success Criteria:
This project focuses on designing a device attachment that integrates with an existing scraping process to mechanically crush Spotted Lanternfly (SLF) egg masses immediately after removal, ensuring they do not hatch. Success will be evaluated based on effectiveness, processing speed, and appropriate sizing.

**Criteria 1: Egg Crushing Effectiveness**
- **What it assesses:** the ability of our mechanism to completely and reliably crush inserted masses
- **Metric:** ~80% eggs crushed per egg mass
- **How it will be measured:**
  - Insert a standardized number of Orbeez into the device and run the crushing mechanism for a standardized amount of time.
  - After each trial, count total Orbeez inserted and crushed Orbeez after being run through the mechanism. Calculate (crushed/total) x 100 to get the percentage of eggs crushed.
- Exhibit-Day demonstration:
  - Live crushing of Orbeez demo
  - Calculate crushing efficiency in real time for observers

**Criteria 2: Processing Rate (eggs per second)**
- **What it assesses:** speed at which device crushes a desired amount of eggs.
- **Metric:**
  - Assume it takes ~10-20 seconds to hand-scrape an SLF egg mass from an uneven surface and insert the masses into the device's inlet funnel. Since there are approximately 30-50 eggs per egg mass, we'd want to crush the eggs in the same timescale at which they're being inputted into the mechanism. So, taking the upper limit, we'd hope to crush 50 eggs in 20 seconds, translating to a processing rate of around 2-3 eggs per second.
- How it will be measured:
  - Insert 50 Orbeez into the device. Turn the crushing mechanism on for 20 seconds. Count the number of crushed eggs produced and divide by the processing time to calculate the processing rate. Repeat this process for multiple trials and average.
  - Repeat this trial for greater quantities of eggs over a standardized amount of time. Count the number of crushed eggs produced and calculate the processing rate. Compare to the desired 2-3 eggs per second metric.
- Note: This would not be tested with our manually controlled prototype, but will be tested when we integrate an electric motor into the device.

**Criteria 3: Device size and weight**
- **What it assesses:** practicality for attachment and field use
- **Metric:**
  - For our device to be easily attachable, we'd want to make it small and lightweight
  - Based off sizes of common juicers and electric grinders, as well as accounting for the size of the motor we hope to incorporate into the device, we hope to create a device whose bounding box is less than or equal to 6x6x10 inches
  - The mechanism is intended to be attached to another device's frame reasonably. Thus we will base the ideal weight on regular handheld devices such as a computer, making the maximum weight to be 4lbs
- How it will be measured:
  - After creating our next prototypes, physically measure the size of device using rulers or calipers
  - Measure the weight of the device using a scale

---

[Download the PDF]({{ '/assets/ODP 5_Functional Prototype.pdf' | relative_url }})