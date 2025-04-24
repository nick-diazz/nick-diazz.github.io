---
title: "Creating a Spool Holder using Generative Design"
excerpt: "A generatively optimized filament spool holder designed to reduce material use while maintaining strength, featuring multiple preserve/obstacle geometries and realistic mechanical load cases."
header:
  image: /assets/img/IMG_2887.jpg
  teaser: /assets/img/IMG_2887.jpg
gallery:
  - url: /assets/img/IMG_2890.jpg
    image_path: assets/img/IMG_2890.jpg
    alt: "Front view of printed spool holder"
  - url: /assets/img/IMG_2889.jpg
    image_path: assets/img/IMG_2889.jpg
    alt: "Side view of mounting interface"
  - url: /assets/img/IMG_5653.JPEG
    image_path: assets/img/IMG_5653.JPEG
    alt: "Spool holder installed on 3D printer frame"
---

## Introduction

This project involved using Fusion 360's generative design tools to create a functional and efficient spool holder for a 3D printer. The goal was to generate an organic, structurally sound component using selective laser sintering (SLS) with PA12 nylon. The design had to accommodate the load of a 1kg spool of filament, prevent slippage of the guide tube, and survive clumsy lab environments.

### Project Objectives
- Reduce mass while preserving structural strength
- Properly support a full filament spool and prevent twisting
- Avoid material in critical operating zones (obstacle geometry)
- Enable secure retention of the filament guide tube
- Design for SLS manufacturing and a bounding box of 100mm x 100mm x 100mm

## Design Features / Rationale

### Preserve & Obstacle Geometry

- **Preserve Geometries:**
  - Mounting holes and baseplate for attachment to the printer
  - Spool support axle
  - Filament guide tube holder (added to meet project requirements)

- **Obstacle Geometries:**
  - Volume occupied by the filament spool
  - Path of the filament between spool and extruder
  - Clearance zones for mounting and assembly

### Load Conditions

| Name                      | Type       | Magnitude       | Location                          | Rationale                                                   |
|---------------------------|------------|------------------|-----------------------------------|-------------------------------------------------------------|
| Spool Weight             | Force      | 12 N            | Vertical, on top of axle          | Simulates the downward force of a full spool                |
| Filament Pull            | Force      | 5 N             | Side of axle or guide tube holder| Lateral tension as filament is pulled into extruder         |
| Spool Torque             | Moment     | 880 N·mm        | Around Z-axis of axle             | Simulates rotational torque as filament unspools            |
| Guide Tube Retention     | Pressure   | 0.1 MPa         | Inside surface of guide holder    | Ensures press-fit retention of 4 mm plastic tube            |
| Vertical Tube Force      | Force      | 2 N             | Downward on guide tube holder     | Simulates misalignment or gravitational force               |
| Impact Load (Clumsy Hit) | Force      | 15 N            | Horizontal on side of vertical arm| Adds robustness for accidental side bumps                   |
| Spool Swap Pull          | Force      | 10 N            | Axial on end of spool support     | Models manual loading/unloading force on spool post         |

### Structural Constraints

- Fully fixed constraints applied to mounting holes and baseplate
- All loads applied only to preserve geometry
- No constraints applied to the spool or guide tube preserve to allow full generative optimization

### Manufacturing Constraints

- SLS constraints set to “unrestricted” for organic forms
- Designed to fit within 100 x 100 x 100 mm build volume
- Functional iteration done in PLA before final SLS print

---

## Instructions

### Interactive CAD Model
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a494c339b681f3f63d?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

### Assembly Instructions
1. Insert the guide tube into the holder; it should press-fit snugly.
2. Mount the spool holder to the printer using screws or bolts.
3. Load the filament onto the support axle and feed into the guide tube.
4. Perform test spins to ensure smooth rotation and secure guidance.

---

## Testing & Functional Results

- The final printed part survived repeated spool swaps and moderate bumps.
- Filament pulled through the guide tube without slipping.
- No warping or fracture observed in stress areas.
- Compared to earlier PLA prototype, the SLS print was 35% lighter and more organic.

### Suggested Improvements
- Add TPU grip interface for quieter guide tube fit
- Embed textured grip under base for more secure surface contact

---

## Gallery

{% include gallery caption="Gallery of the spool holder in design and mounted on printer." %}
