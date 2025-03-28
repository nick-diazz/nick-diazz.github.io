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
  - url: /assets/img/IMG_2829.jpg
    image_path: assets/img/IMG_2829.jpg
    alt: "Pliers Thickness"
---

## Introduction/Purpose
This project focused on designing needle nose pliers capable of gripping through-hole resistors using a print-in-place approach and incorporating a flexible spring component. The final design featured a 5-part assembly (2 rigid claws, 2 rigid handles, and 1 TPU spring) that requires no tools to assemble, functioning immediately after pressing the pieces together.

### What is Print-in-Place?
Print-in-place designs are multi-component models printed as a single object or pre-assembled kit, with built-in clearances that allow moving parts to function directly after printing—no screws, glue, or assembly required. These designs are commonly seen in toys, tools, and hinges, and they showcase the precision possible in 3D printing.

More complex assemblies may benefit from **multi-material prints**, where elastic materials like TPU are combined with rigid ones to simulate springs, gaskets, or soft-touch parts. This project used 95A TPU for the spring.

**Examples of print-in-place applications:**

- **Hinges and joints in 3D-printed toys**  
  Articulated toys, chains, and flexible models rely on built-in hinges and joints that print as a single unit. These moving parts are possible thanks to carefully designed tolerances that allow rotation or bending immediately after printing. Design guides recommend specific spacing and geometries to prevent fused joints and ensure smooth motion.  
  *Sources:*  
  [Endeavor 3D – Designing 3D Printed Hinges and Interlocking Components](https://endeavor3d.com/designing-3d-printed-hinges-and-interlocking-components/)  
  [All3DP – 40+ Coolest Print-in-Place 3D Models](https://all3dp.com/2/coolest-print-in-place-3d-models/)

- **Working gearboxes**  
  Gearboxes like planetary gears or differential drives can be printed in one go with correct tolerances between gear teeth and shafts. This eliminates post-assembly and is useful for prototyping mechanical systems.  
  *Source: [Instructables – Print-in-Place Spring-Loaded Box](https://www.instructables.com/Print-in-Place-Spring-Loaded-Box/)*

- **Prosthetic components with flexible interfaces**  
  In some low-cost prosthetic designs, flexible TPU joints or hinges are printed directly into the device. These components allow motion, reduce part count, and make the device more comfortable.  
  *Source: [nTop – 3D Printing in Prosthetics: A Design Guide](https://www.ntop.com/resources/blog/3d-printing-in-prosthetics-a-design-guide/)*

---

## Design Process

### Interactive CAD Model
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a42f32e15944736827?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

- CAD was developed in Fusion 360 with a fully constrained, timeline-organized model.
- Top-down modeling principles guided the component relationships.
- The handles were rigid PLA components, while the spring was printed separately in TPU.

### Spring Component
- The TPU spring geometry was iteratively tested and modeled for optimal flexibility.
- The final spring design featured a rhombus-shaped component that flexed outward under compression and reliably returned the pliers to the open state when released.
- To enhance elasticity, the **top and bottom solid layers of the spring were removed**, leaving only the internal structure exposed. This reduced material stiffness and allowed for more responsive deformation.
- A **grid infill pattern** was used, which provided multidirectional flexibility and structural consistency under repeated use.
- The infill density was reduced to approximately **25%**, striking a balance between durability and springiness.
- Multiple versions were printed with varying rhombus dimensions and infill patterns to test how geometry influenced the spring’s restoring force and overall performance.


---

## Specifications

| Feature                | Specification           |
|------------------------|-------------------------|
| Total Length           | ~300 mm                 |
| Jaw Length             | 110 mm                  |
| Jaw Capacity           | ~5–6 mm at tips         |
| Material (Handles/Jaws)| PLA                     |
| Material (Spring)      | TPU (95A)               |
| Assembly               | Tool-free, hand-pressed |

---

## Print Settings

- **Handles (PLA):**
  - Layer Height: 0.6 mm
  - Infill: 100%
  - Orientation: Flat on the surface for maximum layer adhesion and strength at stress points
- **Spring (TPU):**
  - Layer Height: 0.6 mm
  - Infill: 25% (for better elasticity), Grid Pattern, Top and Bottom infill layers removed
- Printed using a standard Voron printer with adjusted slicer settings.

---

### Discussion

**Challenges and Iterations**  
- Early prints lacked sufficient clearance between the jaws and the hinge, resulting in fused parts.
- A test piece was printed for the spring-fit to dial in tolerances.
- TPU presented some challenges during printing, particularly with occasional stringing in areas with long travel moves or retraction gaps.
- When printing the spring component, if the retaining wedges were too small, the printer tended to round them off or print them as rectangles, which compromised their ability to securely hold all five parts together.
- The final version had an optimized jaw taper for precision gripping of small resistors.

**Performance Review**  
The pliers snapped together easily and operated smoothly thanks to the TPU spring. They reliably gripped small components, returning to the open position without user input.

**Future Improvements**  
- Add ribbing or grip texture on handles for ergonomic use.
- Integrate snap-fit features to better retain the spring under tension.
- Explore printing the entire system in-place on the multi-material printer for full automation.

---

### Multimedia

{% include gallery caption="Gallery showing printed pliers and design process." %}

<!-- Imgur embed starts here -->
<blockquote class="imgur-embed-pub" lang="en" data-id="a/RFCUgJ5" data-context="false">
  <a href="//imgur.com/a/RFCUgJ5">View post on Imgur</a>
</blockquote>
<script async src="//s.imgur.com/min/embed.js" charset="utf-8"></script>
<!-- Imgur embed ends here -->

<!-- Imgur embed starts here -->
<blockquote class="imgur-embed-pub" lang="en" data-id="a/kENeOPF" data-context="false">
  <a href="https://imgur.com/a/kENeOPF">View post on Imgur</a>
</blockquote>
<script async src="https://s.imgur.com/min/embed.js" charset="utf-8"></script>
<!-- Imgur embed ends here -->

