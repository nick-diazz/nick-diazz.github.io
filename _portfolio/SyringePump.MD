---
title: "3D-Printed Syringe Pump"
excerpt: "The syringe pump enables precise and controlled delivery of fluids at adjustable flow rates for experimental applications."
header:
  image: /assets/img/Syringe Pump.png
  teaser: /assets/img/Syringe Pump.png
gallery:
  - url: /assets/img/Cyber-Scooter-1.jpg
    image_path: assets/img/Cyber-Scooter-1.jpg
    alt: "placeholder image 1"
  - url: /assets/img/Cyber-Scooter-2.jpg
    image_path: assets/img/Cyber-Scooter-2.jpg
    alt: "placeholder image 2"
  - url: /assets/img/Cyber-Scooter-3.jpg
    image_path: assets/img/Cyber-Scooter-3.jpg
    alt: "placeholder image 3"
---

### Purpose and Features
The syringe pump project aims to deliver fluids at controlled flow rates for applications such as healthcare, microfluidics, and industrial use. It offers a cost-effective, customizable alternative to traditional syringe pumps by utilizing 3D printing and Arduino programming. Key features include:
- Adjustable flow rates (1–10 mL/min) using a potentiometer.
- Compatibility with syringes of varying diameters (10 mL to 20 mL).
- LED indicators for operation states (running, paused, or empty).
- Manual adjustments using momentary buttons for precision control.

---

### Final Design
![Rendered Syringe Pump Design](assets/img/Syringe Pump.png) 
*A rendering of the syringe pump.*

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
[View Code](link_to_github_repository)

---

### Interactive 3D Model
An interactive Fusion 360 model of the syringe pump assembly is available for exploration.  
[View 3D Model](link_to_model)

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
