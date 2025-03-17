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

# Introduction/Purpose 
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

### Off-the-Shelf Parts

| **Part Name**        | **Quantity** | **Description**                           |
|-----------------------|--------------|-------------------------------------------|
| Stepper Motor         | 1            | Provides precise rotational motion.       |
| Lead Screw            | 1            | Converts rotational motion to linear movement. |
| Arduino Uno           | 1            | Microcontroller for system control.       |
| Power Supply          | 1            | Provides required voltage for the system. |
| Push Buttons          | 3            | Latching and momentary buttons for user input. |
| Potentiometer         | 1            | Adjusts the fluid flow rate.              |

---

### 3D-Printed Parts

| **Part Name**         | **Quantity** | **Material** | **Purpose**                  |
|-----------------------|--------------|--------------|------------------------------|
| Syringe Holder        | 1            | PLA          | Holds the syringe securely.  |
| Motor Bracket         | 1            | PLA          | Mounts the stepper motor.    |
| Enclosure             | 1            | PLA          | Protects electronics.        |

---

### Arduino Code
The Arduino code controlling the syringe pump is available in the project repository.  
[View Code](https://github.com/nick-diazz/Syringe_PUMP-Arduino_Code)

---

### Interactive 3D Model
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a4dc1395df3c21536d?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

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

