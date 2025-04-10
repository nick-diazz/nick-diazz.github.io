---
title: "Top-Down Modeled Bike Phone Holder"
excerpt: "A modular phone mount for bikes that enables quick attachment, smooth rotation, and stable use through road vibration, built using a top-down CAD approach."
header:
  image: /assets/img/IMG_2887.jpg
  teaser: /assets/img/IMG_2887.jpg
gallery:
  - url: /assets/img/phoneholder1.jpg
    image_path: assets/img/phoneholder1.jpg
    alt: "Top view of mounted phone holder"
  - url: /assets/img/phoneholder2.jpg
    image_path: assets/img/phoneholder2.jpg
    alt: "Side view of detent mechanism"
  - url: /assets/img/phoneholder3.jpg
    image_path: assets/img/phoneholder3.jpg
    alt: "Phone holder installed on handlebars"
---

## Introduction

This project involved designing and 3D printing a functional phone holder for a bicycle using a **top-down modeling approach** in Fusion 360. The holder secures a smartphone onto handlebars, allowing the user to rotate the phone between portrait and landscape orientations using a detent-based snapping mechanism. The device was modeled around a fixed handlebar component and a CAD model of the user’s phone, allowing for seamless design integration and component alignment.

### Project Objectives
- Quick phone attachment/detachment without tools
- Smooth snap rotation between landscape and portrait
- Secure grip under road vibrations
- Clamp compatibility with 22.2 mm and 25.4 mm bike handlebars

## Design Features

### Top-Down CAD Modeling
Using a top-down approach, the handlebar served as the fixed reference component. A CAD model of my current phone was imported and positioned at a natural viewing angle, either landscape or portrait. Components such as the rotation disc, detent ring, phone clamp, and handlebar mount were designed in place using **as-built joints**. Parametric dimensions were applied to enable easy tweaking for fit and clearance.

### Detent Rotation Mechanism
The rotating mount includes a detent mechanism: a **spring-loaded ball bearing** that locks into shallow circular notches on the rotating disc. This provides tactile feedback and holds the phone in fixed orientations during use. The mechanism was prototyped separately and iteratively refined to optimize holding strength without restricting rotation.

### Structural Design
- **Clamp mount** fits both 22.2 mm and 25.4 mm bars with swappable sleeves
- **Snap-fit arms** securely grip the phone without tools
- **Rotation disc** and detent interface ensure tactile rotation
- Printed with **PLA filament** and **TPU filament** for the phone holder simply for demonstration purposes

---

## Instructions

### Interactive CAD Model
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a4dc1395df3c21536d?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true" frameborder="0"></iframe>

### Assembly Overview
1. Print the individual components: base clamp, rotating disc, phone clamp, detent ring.
2. Insert M3 fasteners and heat-set inserts where applicable.
3. Install the spring and ball bearing into the detent chamber.
4. Assemble the rotating disc and snap the phone clamp onto the phone.
5. Attach the clamp mount to the handlebars using M5 bolts or Allen keys.
6. Rotate the phone to the desired orientation until it snaps into place.

### Printing Tips
- Use **0.6 mm layer height** and **40-50% infill** for strength.
- Print detent parts vertically to resist shear.
- Optional: Use powder printing for smoother surface finish and stronger parts if available.

---

## Discussion

### Modeling Strategy
Top-down modeling enabled a highly integrated design where every component fit together without later adjustments. Starting from a fixed handlebar model and a CAD phone ensured the mount was optimized for real-world use and sightlines. As-built joints were crucial for defining component relationships without over-constraining the model.

### Functional Results
- The holder successfully rotated between orientations with a satisfying "click".
- The phone stayed secure during vibration testing.
- Swapping between phones of similar size only required parameter adjustment.

### Limitations & Improvements
- Detent ball housing could be tighter for a higher holding force.
- Introducing rubber pads or TPU inserts could improve grip and vibration damping.
- Adding a tool-free tightening knob for the clamp may improve field usability.

### Potential Extensions
- Modular arm attachments for GoPros or lights
- Quick-release tab for single-hand removal
- Embedded NFC tag or phone charger integration

---

## Multimedia

{% include gallery caption="Gallery of bike phone holder and detent mechanism in use." %}

<iframe width="560" height="315" src="https://www.youtube.com/embed/EEker-w1FwE" title="YouTube video player" frameborder="0" allowfullscreen></iframe>

---

### References
- [Top-Down CAD Overview](https://www.youtube.com/watch?v=QnqAtSeqRPo)
- [Bike Handlebar Standards](https://a.co/d/iuKd8nz)
- [Detent Mechanism Components](https://a.co/d/6SNhmxb)
