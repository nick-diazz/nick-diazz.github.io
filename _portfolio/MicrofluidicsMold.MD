---
title: "Resin-Printed Microfluidics Mold"
excerpt: "A resin-printed mold that enhances precision in microfluidic pinch-flow sorting."
header:
  image: /assets/img/Screenshot 2025-03-16 184559.png
  teaser: /assets/img/Screenshot 2025-03-16 184559.png
gallery:
  - url: /assets/img/IMG_2804 (1).jpg
    image_path: assets/img/IMG_2804 (1).jpg
    alt: "placeholder image 1"
  - url: /assets/img/IMG_2805 (1).jpg
    image_path: assets/img/IMG_2805 (1).jpg
    alt: "placeholder image 2"
  - url: /assets/img/IMG_2802 (2).jpg
    image_path: assets/img/IMG_2802 (2).jpg
    alt: "placeholder image 3"
---

## Introduction/Purpose 
This project utilizes resin-printed molds for precise particle sorting in microfluidic pinch-flow fractionation, offering an efficient, customizable method for micro-scale fluid analysis. Key features include:
- High-resolution molds printed using SLA technology.
- Symmetrical channel design for balanced flow distribution.
- Outlet optimization for easy fraction collection.
- Parylene-coated surfaces for smooth, reliable PDMS casting.

### Microfluidic Devices
Microfluidic devices manipulate tiny fluid volumes, typically on the microliter or smaller scale, to perform precise     operations such as particle sorting, fluid mixing, and chemical reactions. These compact systems exploit the physics of fluid flow at microscale to precisely control fluid behavior, making them valuable tools in analytical chemistry, biological analysis, and medical diagnostics.

### Pinch Flow Fractionation
Pinch Flow Fractionation (PFF) is a microfluidic technique used to separate particles based on size. In PFF, particles are initially focused into a narrow stream within a microchannel, creating a "pinch" region. When the channel expands downstream, smaller particles migrate toward the walls faster than larger particles due to differences in their positions in the laminar velocity profile. This leads to particle separation into distinct outlet streams according to size.

### Application
One specific application of particle sorting through PFF is the isolation of circulating tumor cells (CTCs) from blood samples. Effective sorting of these cells can greatly enhance cancer diagnosis and monitoring. A study demonstrated that PFF could reliably separate rare cancer cells from blood components, significantly improving early detection and therapeutic outcomes ([Lu & Xuan, 2015](https://link.springer.com/article/10.1007/s10404-013-1291-9)).

#### References
- [Density and Specific Gravity of Water and Other Liquids](https://www.cospheric.com/density_specific_gravity_of_water_and_other_liquids.htm)
- [Lu & Xuan, 2015. Particle separation and sorting in microfluidic devices: A Review](https://link.springer.com/article/10.1007/s10404-013-1291-9)

---

## Instructions

### Interactive 3D Model
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a4dc1395df3c21536d?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>
- Design your microfluidic mold using Fusion 360, ensuring all sketches and features are fully constrained and clearly labeled.
- Maintain minimum dimensions based on printer specifications (XY resolution: 25 μm, Z resolution: 25 μm).
- Use 1.5 mm extrusions for inlet and outlet connections.

### Print and Cure Mold
- Print the mold using the Form 3+/4 SLA printers, selecting appropriate layer thickness (typically 0.05 mm or 0.025 mm).
- Ensure the bottom face of the mold (which contacts the glass slide) remains perfectly flat to prevent layer lines.
- Wash the printed mold for 5 minutes in FormWash, followed by an additional 5-minute wash in fresh IPA. Dry thoroughly for 30 minutes and cure the mold surface for 60 seconds at room temperature.

### Parylene Device
- Coat your resin-printed mold with parylene to ensure a smooth, reliable casting surface for PDMS and to avoid curing inhibition issues caused by uncured resin residues.

### Cast PDMS
- Cast polydimethylsiloxane (PDMS) onto the parylene-coated mold.
- Cure the PDMS according to recommended heat cure times (24 hours at 23°C, 4 hours at 65°C, or 15 minutes at 150°C).

### Plasma Bond Glass Slide
- Bond your PDMS device to a glass slide using plasma treatment to form a secure, leak-free microfluidic device.
- Ensure proper alignment and consistent bonding to maintain structural integrity and functional efficiency.

#### References
- [Density and Specific Gravity of Water and Other Liquids](https://www.cospheric.com/density_specific_gravity_of_water_and_other_liquids.htm)
- [Lu & Xuan, 2015. Particle separation and sorting in microfluidic devices: A Review](https://link.springer.com/article/10.1007/s10404-013-1291-9)
- [Rapid prototyping of cell culture microdevices using parylene-coated 3D prints](https://pubs.rsc.org/en/content/articlelanding/2021/lc/d1lc00744k)

---

### Discussion

**Parylene Coating and Applications**  
Resin-printed molds are coated with parylene to prevent PDMS curing inhibition and achieve a smooth surface suitable for effective bonding with glass substrates. Parylene coating significantly reduces surface roughness and facilitates easy removal of PDMS from molds, thus enhancing device reliability. Hypothetical applications of this microfluidic sorter include biomedical diagnostics (such as blood cell sorting), environmental monitoring (e.g., separating microplastics), and pharmaceutical quality control.

**Sorting Geometry**  
The design geometry supports pinch-flow fractionation by precisely controlling fluid dynamics. The critical pinch width is sized at approximately 1.2–1.5 times the diameter of the largest target particle (425–500 µm) to avoid clogging and ensure effective single-layer particle separation. Outlet channels are symmetrically designed, with matched lengths and widths to maintain equal flow rates and avoid recombination of particle streams. Inlet and outlet ports are strategically positioned at least 11 mm apart, ensuring barb compatibility and preventing interference. Channels are positioned at least 3 mm from device edges to enable strong bonding to a glass slide and prevent leakage.

**Ensuring Consistent Flow Rates**  
To ensure each outlet had the same flow rate and the particles stayed separated, I designed the outlet layout so that the bottom half of the outlet section mirrors that of the top half. While it was challenging to make all outlet paths exactly the same length due to the size limitations of the microfluidic device, the mirrored layout helped balance the pressure across each channel and supported consistent flow. With this setup, the smallest particles naturally went through the top outlet, and the slightly bigger ones went through the second one below it. The equal layout made the flow smooth and predictable, which helped the sorting work properly.

**Potential Improvements**  
After fabricating and testing the microfluidic device, it performed successfully. Particles were sorted correctly, with smaller particles consistently flowing through the top channel, and larger particles being directed to the channel immediately below it. The bottom two channels functioned effectively to expel excess water. One improvement that can be made to the device includes figuring out a way to where all outlet lengths are equivalent so that the risk of backpressure and mixing is further minimized. Future improvements to the testing setup could involve refining the leveling of the testing setup for enhanced ease of setup and achieving better test results.

**Bonus Opportunity**  
Although the bonus opportunity was not attempted, one possible solution would be to design and 3D print a simple manifold device with symmetrical tubing pathways and integrated leveling adjustments to ensure equal backpressure and uniform flow rates across all microfluidic device outlets. This approach would minimize variations caused by tubing length, diameter, and positioning.  

---

### Multimedia

{% include gallery caption="This is a sample gallery to go along with this case study." %}

<iframe width="560" height="315" src="https://www.youtube.com/embed/EEker-w1FwE" title="YouTube video player" frameborder="0" allowfullscreen></iframe>

