---
title: "Resin-Printed Microfluidics Mold"
excerpt: "A resin-printed mold that enhances precision in microfluidic pinch-flow sorting."
header:
  image: /assets/img/Screenshot 2025-03-16 184559.png
  teaser: /assets/img/Screenshot 2025-03-16 184559.png
gallery:
  - url: /assets/img/unnamed.png
    image_path: assets/img/unnamed.png
    alt: "placeholder image 1"
  - url: /assets/img/Syringe Pump.png
    image_path: assets/img/Syringe Pump.png
    alt: "placeholder image 2"
  - url: /assets/img/circuit-Syringe.png
    image_path: assets/img/circuit-Syringe.png
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

### References
- [Density and Specific Gravity of Water and Other Liquids](https://www.cospheric.com/density_specific_gravity_of_water_and_other_liquids.htm)
- [Lu & Xuan, 2015. Particle separation and sorting in microfluidic devices: A Review](https://link.springer.com/article/10.1007/s10404-013-1291-9)
- [Rapid prototyping of cell culture microdevices using parylene-coated 3D prints](https://pubs.rsc.org/en/content/articlelanding/2021/lc/d1lc00744k)
---

### Operating Instructions
1. **Assembly**: Mount the stepper motor, lead screw, and syringe holder. Secure all components.
2. **Install the Syringe**: Fill the syringe with the desired fluid, remove air bubbles, and insert it into the holder.
3. **Connect to Power**: Connect the system to a 12V power supply.
4. **Upload Code**: Use the Arduino IDE to upload the control code to the microcontroller.
5. **Start Operation**: Adjust the flow rate using the potentiometer and press the start button.
6. **Monitor Operation**: Observe LED indicators to track the state (green for running, yellow for paused, red for empty).
7. **Shutdown**: Turn off the power supply and clean the syringe after use.

---

### Additional Notes
- The project emphasizes modularity and precision for research or niche applications.
- Customizable design for different syringe sizes ensures broad usability.

---
{% include gallery caption="This is a sample gallery to go along with this case study." %}

