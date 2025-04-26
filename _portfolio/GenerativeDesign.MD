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

This project focused on using Fusion 360’s generative design to create a functional and efficient filament spool holder, specifically designed to be mounted onto a 3D printer. The part was intended not just as a structural support but as an improvement to a common problem faced in many 3D printing setups, especially in shared lab environments. Traditional spool holders are often mounted on the back of the printer, making it difficult to monitor how much filament is left during a print. Users typically have to walk around the machine or use a step stool to check the filament status. My design repositions the filament spool holder to a more accessible location, aiming to improve user experience by providing a clear line of sight to the remaining filament throughout the print process.

My finalized design consists of a robust spool mounting arm that supports the filament spool above the printer, a guide tube holder that lets the filament smoothly flow into the extruder, and integrated mounting features to easily secure the assembly onto the printer’s frame. I used PA12 nylon through selective laser sintering (SLS) printer as the intended manufacturing method, as this was one of the project’s constraints. This was perfectly fine since PA12 is very durable and has the ability to handle the more complex organic geometries produced by generative design. The part needed to meet several key functional requirements: it had to withstand the full weight of a fresh filament spool (which can weigh up to 1kg), securely anchor the filament guide tube under dynamic loads (such as tension during extrusion), and resist impacts or bumps common in busy lab spaces.

The problem this part solves is specifically related to usability and reliability in 3D printing. In many lab environments, students and users initiate prints without realizing their spool is running low on filament, leading to mid-print failures that waste time, material, and machine availability. My professor identified this as a recurring issue and emphasized the need for a design solution that would make filament levels easily visible during printing. By repositioning the spool to a visible location and incorporating a stable mounting for the filament guide tube, this project directly addresses that problem. It ensures that students and users can quickly glance at the printer and immediately tell whether there is enough filament to complete their print or if they need to switch the spool. This significantly reduces failed prints and improves overall workflow.

This project was especially meaningful to me because I personally experienced this exact frustration a couple of times while working with the lab’s 3D printers. In order to check the amount of filament left, I often had to search for a step stool, climb up behind the machine, and awkwardly reach around the printer just to see what spool was installed and how much filament was left. This process not only wasted time but also introduced small risks, such as accidentally bumping neighboring 3D printers mid-print or misjudging filament availability. Designing a solution to this everyday inconvenience felt very real and practical. It was motivating to create something that could improve not just my experience but also that of many future students using the same equipment.

Moreover, working through the design process using generative design tools added an additional layer of meaning to the project. Generative design allowed me to approach the problem in a way that I would not have considered with traditional CAD modeling. Instead of manually designing supports and optimizing material placement through intuition alone, I set up real-world load cases and constraints that allowed the software to explore many possibilities. It gave me valuable insight into how computational design can create forms that are structurally efficient yet lightweight, forms that I probably would not have arrived at manually. One thing I would like to mention is how specific the software was. In some instances, you would expect the AI to develop a solution with what's already there, but even then, it would fail. It really showed me that I have to monitor the design and make sure it makes sense for the software to solve. Seeing the original structures evolve through multiple iterations made me appreciate how engineering and design are increasingly driven by computational power and how important it is to guide that process with good real-world understanding.

Finally, the project tied together both practical needs and advanced design methods, which is something I found particularly rewarding. It wasn’t just about making a visually interesting part, it was about solving a real problem with a smart, easy-to-make, and practical solution. The experience deepened my appreciation for the role of user-centered design in engineering, and even small improvements, like repositioning a spool holder, can have a significant impact on everyday workflow and equipment reliability how well the equipment works.

Overall, this project was a meaningful intersection of personal experience, lab needs, and modern design tools. It taught me that good engineering is often about focusing on small, overlooked problems and applying the right tools to create thoughtful, practical solutions.

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
