---
title: "Creating a Spool Holder using Generative Design"
excerpt: "A generatively optimized filament spool holder designed to reduce material use while maintaining strength, featuring multiple preserve/obstacle geometries and realistic mechanical load cases."
header:
  image: /assets/img/IMG_3055.jpg
  teaser: /assets/img/IMG_3055.jpg
gallery:
  - url: /assets/img/IMG_3055.jpg
    image_path: assets/img/IMG_3055.jpg
    alt: "Front view of printed spool holder"
  - url: /assets/img/IMG_3056.jpg
    image_path: assets/img/IMG_3056.jpg
    alt: "Side view of mounting interface"
  - url: /assets/img/IMG_3059.jpg
    image_path: assets/img/IMG_3059.jpg
    alt: "Spool holder installed on 3D printer frame"
---

## Introduction

This project was all about using Fusion 360's generative design tools to create a functional and efficient spool holder that would be mounted on a 3D printer. One of the issues with the current spool holder is how it is mounted on the back, and users cannot see how much filament is left on the spool. The goal was to solve this issue and be able to generate an organic, structurally sound component using selective laser sintering (SLS) with PA12 nylon. The design had to be able to withstand the weight of a full spool of filament, hold the guide tube that leads the filament to the extruder, and survive clumsy lab environments.

### Project Objectives
- Reduce mass while preserving structural strength
- Properly support a full filament spool and prevent twisting or tangling
- Avoid material in critical operating zones (obstacle geometry)
- Enable secure retention/holding of the filament guide tube
- Design for SLS manufacturing and a bounding box of 100mm x 100mm x 100mm

## Design Features / Rationale

### Preserve & Obstacle Geometry

- **Preserve Geometries (GREEN):**
  - Mounting holes and baseplate for attachment to the printer
  - Spool support axle
  - Filament guide tube holder (added to meet project requirements (have at least 3 preserve and 3 obstacle geometries))

- **Obstacle Geometries (RED):**
  - Volume occupied by the filament spool
  - Path of the filament between spool and extruder
  - Clearance zones for mounting and assembly

![Preserve and Obstacle Geometry Diagram](/assets/img/Screenshot 2025-04-25 152758.png)

### Loading Conditions

| Load Name                | Description                                   | Magnitude | Direction       |
|---------------------------|-----------------------------------------------|-----------|-----------------|
| Vertical Tube Force       | Weight of filament guide tube                | 3.5 N     | Downward        |
| Spool Mounting Load        | Force from spool weight when mounted         | Varies    | Vertical        |
| Tension Force in Filament  | Pulling force from extruder motor            | ~1-5 N    | Toward Extruder |

### Additional Forces

| Load Name                        | Description                                             | Magnitude | Direction            |
|-----------------------------------|---------------------------------------------------------|-----------|----------------------|
| Spool Push Force (Loading)        | User pushing spool onto the mount                       | 10 N      | Horizontal (axial)   |
| Guide Tube Weight                 | Weight of filament guide tube (duplicated for clarity)  | 3.5 N     | Vertical (downward)  |
| Top Guide Tube Holder Force       | Force during loading/unloading guide tube               | 5 N       | Various (user applied) |
| Impact Load on Guide Tube Holder  | Accidental bump during clumsy handling                  | 30 N      | Left/Right (lateral)  |

### Structural Constraints

The main structural constraints applied to this model only really include the mounting part of the spool holder, which was fully fixed. All loads were only applied to the preserved geometry. Setting the bottom of the mounting plate to fully fixed limits the AI in what to change/generate when having to connect all the pieces. 

### Manufacturing Constraints

Manufacturing constraints were set to “unrestricted” for the best outcomes. Although the holder was intended to fit within 100 x 100 x 100 mm build volume, it was built more towards 130 × 105 × 285 mm. 

### How forces were determined

I determined the magnitude, direction, and location of each load by using ChatGPT to estimate reasonable forces based on typical user interactions and component weights. For example, loads from the filament spool and guide tube were based on expected handling forces and gravity. To refine these loads on a real-world prototype, you can use tools like a spring scale to measure actual forces during use. Observing where stresses and deformations occur can help update the load cases for future design iterations. 

---

## Instructions

### Interactive CAD Model
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a4c536b47565c88ffa?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

### Assembly Instructions
1. Insert the guide tube into the holder; it should press-fit snugly. If need be, use a drill to make the hole a little wider
2. Mount the spool holder to the printer using screws or bolts.
3. Load the filament onto the cylindrical part of the spool holder and feed the filament into the guide tube.
4. Perform test spins to ensure smooth rotation and secure guidance.

---

## Testing | Functional Results | Critiques

- The final printed part survived repeated spool swaps and moderate bumps and shakes.
- Filament pulled through the guide tube without slipping.
- There was no warping or any type of fractures observed in areas of stress.

### Suggested Improvements
- Add TPU grip interface for quieter guide tube fit
- Embed textured grip under base for more secure surface contact
- Make preserve geometries in Fusion a little bigger to help the AI have better creativity and produce better outcomes overall

### Critiques of Generative Design

I feel as if Generative Design in 3D modeling is a very useful tool, but very specific when trying to produce something. You need to ensure that you have all of your preserve and obstacle geometries labeled correctly, all the forces with the right magnitudes, and all manufacturing/structural constraints set in place. There is also some software bias where the software will prioritize certain goals in the design over others, so make sure to review the results and adjust the design and constraints as needed. It took me a while to be able to produce a working design, but once you get the hang of it, it's pretty straightforward from there. 

Overall, I feel like generative design is most useful in industries like aerospace, automotive, and medical devices, where lightweighting and performance optimization are critical. The software does well when having to create efficient structures that would be difficult to design manually. One way generative design falls short is in applactions that require simple, low-cost, or generic parts. This would be due to the complex geometries that can be hard to manufacture with traditional methods.

---

## Gallery

{% include gallery caption="Gallery of the spool holder in design and mounted on printer." %}
