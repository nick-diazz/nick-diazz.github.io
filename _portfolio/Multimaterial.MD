---
title: "Multi-Material Spring-Loaded Pliers"
excerpt: "Flexible, print-in-place needle nose pliers designed for precision gripping using rigid and elastic components."
header:
  image: /assets/img/PLiers 1.jpg
  teaser: /assets/img/PLiers 1.jpg
gallery:
  - url: /assets/img/PLiers 1.jpg
    image_path: assets/img/PLiers 1.jpg
    alt: "Fully assembled pliers with TPU spring"
  - url: /assets/img/IMG_2832.jpg
    image_path: assets/img/IMG_2832.jpg
    alt: "Top view of open jaws"
  - url: /<blockquote class="imgur-embed-pub" lang="en" data-id="a/RFCUgJ5" data-context="false" ><a href="//imgur.com/a/RFCUgJ5"></a></blockquote><script async src="//s.imgur.com/min/embed.js" charset="utf-8"></script>
    image_path: <blockquote class="imgur-embed-pub" lang="en" data-id="a/RFCUgJ5" data-context="false" ><a href="//imgur.com/a/RFCUgJ5"></a></blockquote><script async src="//s.imgur.com/min/embed.js" charset="utf-8"></script>
    alt: "Iteration testing flexible spring"
---

## Introduction/Purpose
This project focused on designing needle nose pliers capable of gripping through-hole resistors using a print-in-place approach and incorporating a flexible spring component. The final design featured a 3-part assembly (2 rigid arms and 1 TPU spring) that requires no tools to assemble, functioning immediately after pressing the pieces together.

### What is Print-in-Place?
Print-in-place designs are multi-component models printed as a single object or pre-assembled kit, with built-in clearances that allow moving parts to function directly after printing—no screws, glue, or assembly required. These designs are commonly seen in toys, tools, and hinges, and they showcase the precision possible in 3D printing.

More complex assemblies may benefit from **multi-material prints**, where elastic materials like TPU are combined with rigid ones to simulate springs, gaskets, or soft-touch parts. This project used 95A TPU for the spring.

**Example of print-in-place applications:**  
- Hinges and joints in 3D-printed toys  
- Working gearboxes  
- Prosthetic components with flexible interfaces ([All3DP article](https://all3dp.com/3d-printed-flexible-pliers/))

---

## Design Process

### Interactive CAD Model
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SHxyz...example" width="640" height="480" allowfullscreen frameborder="0"></iframe>

- CAD was developed in Fusion 360 with a fully constrained, timeline-organized model.
- Top-down modeling principles guided the component relationships.
- The handles were rigid PLA components, while the spring was printed separately in TPU.

### Spring Component
- The TPU spring geometry was iteratively tested and modeled for optimal flexibility.
- A U-shaped arch flexed outward under compression and returned the jaws to the open state.
- Multiple spring thicknesses were tested for durability and opening capacity.

---

## Specifications

| Feature              | Specification                  |
|----------------------|--------------------------------|
| Total Length         | ~100 mm                        |
| Jaw Length           | 35 mm                          |
| Jaw Capacity         | ~5–6 mm at tips                |
| Material (Handles)   | PLA                            |
| Material (Spring)    | TPU (95A)                      |
| Assembly             | Tool-free, hand-pressed        |

---

## Print Settings

- **Handles (PLA):**
  - Layer Height: 0.2 mm
  - Infill: 30%
  - Orientation: Vertical for jaw strength
- **Spring (TPU):**
  - Layer Height: 0.2 mm
  - Walls: 3
  - Infill: 100% (for better elasticity)
- Printed using standard Voron printer with separate passes for each material.

---

### Discussion

**Challenges and Iterations**  
- Early prints lacked sufficient clearance between jaws and hinge, resulting in fused parts.
- A test piece was printed for the spring-fit to dial in tolerances.
- TPU proved difficult to print without stringing; printing speed and retraction were adjusted.
- Final version had an optimized jaw taper for precision gripping of small resistors.

**Performance Review**  
The pliers snapped together easily and operated smoothly thanks to the TPU spring. They reliably gripped small components, returning to the open position without user input.

**Future Improvements**  
- Add ribbing or grip texture on handles for ergonomic use.
- Integrate snap-fit features to better retain the spring under tension.
- Explore printing the entire system in-place on the multi-material printer for full automation.

---

### Multimedia

{% include gallery caption="Gallery showing printed pliers and design process." %}

<iframe width="560" height="315" src="https://www.youtube.com/embed/YOUR_VIDEO_ID" title="Pliers Function Demo" frameborder="0" allowfullscreen></iframe>
