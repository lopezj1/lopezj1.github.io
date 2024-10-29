---
title: "Remixing the Pikie Lure - Part 1: The Design Phase"
date: 2024-10-28 00:00:00 -04:00
tags: [3D Printing, CNC Machining, Shapeoko, Ender3, Fusion360]
description: "Reimagining a Classic Lure with Desktop Maker Tools"
math: true
---

## Intro
As an avid saltwater fisherman, I'm always searching for ways to improve my game, both on and off the water. Owning both a 3D printer and a CNC router, I decided to take on a new challenge: designing a modern remix of a classic striped bass lure—the Pikie.

A bit of history: The Pikie lure, originally designed by the Creek Chub Bait Company in the early 1900s for freshwater fishing, became a favorite among striped bass anglers along the U.S. East Coast by the mid-20th century. Its lifelike baitfish profile, durable construction, and versatile wobbling action made it particularly effective at mimicking prey like bunker and herring, turning it into a go-to lure for surfcasters targeting big stripers.

![Pikie Lure Prototype](assets/img/pikie-lure/Original-pikie-striper.jpg)
*Striped Bass that fell for irresistable wobble of the Pikie - Image from [On The Water](https://onthewater.com/choose-the-right-striper-plug)*

Traditionally, the Pikie was made from buoyant wood like basswood and shaped on a lathe. For my version, I'll be using 3D printing for prototyping and a CNC router for final production. Since these manufacturing methods differ from the original, I’ll need to design the lure body in two halves and join them during post-processing. This approach offers advantages: it allows me to experiment with internal cavities for creating air pockets to boost buoyancy or adding weights to fine-tune the lure’s action.

In this post, I'll outline my design requirements and the considerations I’ve made with Design for Manufacturing (DFM) in mind. I'll walk you through my design process, share the lessons learned along the way, and discuss the next steps as I move toward prototyping my remix of this iconic lure.

## Design Requirements
1. Thru-Wire Construction
   - Ensures that a hooked fish stays on even if the lure body breaks, providing durability and reliability.
2. Target Weight: 1-3 oz
   - This weight range is optimal for my preferred surf fishing setup, offering a balance between casting distance and control.
3. Buoyant in Saltwater
   - Designed to float, allowing for surface action with the flexibility to tune for subsurface performance when needed.
4. Parametric 3D Model
   - A fully parametric design for easy adjustments to the lure’s shape and profile, streamlining iterations and experimentation.
5. 3D Printable
   - Optimized for rapid prototyping and testing, allowing for efficient tweaks and on-the-fly improvements.
6. CNC Machinable
   - Tailored for transitioning proven prototypes to a CNC workflow, making it production-ready for higher-volume or more refined builds

## Design Process
#### Material Selection
I will be using PLA filament for 3D printing the prototype of this Pikie remix for a few reasons:
- Easy to Print (minimal quality issues)
- Faster to Print (this material can run near the upper limits of my printer)
- Non-critical mechnical properties 
  - I will be coating this in epoxy resin to make it water tight and more durable for testing

There is one important caveat; however, **PLA is more dense than wood**

A little bit of physics and math is needed to ensure my design will float in saltwater like a traditional pikie made out of basswood.

The density equation is:

$$
\rho = \frac{m}{V}
$$

where:
- $ \rho $ is the density,
- $ m $ is the mass,
- $ V $ is the volume.

Here are the densities that will need be evaluated:

| Material | Density          |
| -------- | ---------------- |
| PLA      | 1.240 $ g/cm^3 $ |
| Basswood | 0.320 $ g/cm^3 $ |
| Salwater | 1.025 $ g/cm^3 $ |

At first glance, it appears PLA will sink in saltwater and basswood will float, but there are two levers that can be tweaked to target a specific density -- mass and volume. The volume in this case will remain constant because the same lure shape/profile will be used for both materials.  On the other hand, the mass can be adjusted on the PLA version to ensure it will float in saltwater. 

To explain how this can be done, I will need to walk through the CAD modeling of the design and highlight some of the nuances in additive manufacturing that can help solve this problem.

#### CAD Modeling
## Learnings
#### Challenges
#### New Skills
## Ready for Prototyping
<!-- Final Design -->
<!-- Next Post Tease -->
## Conclusion
<!-- encourage comments for feedback/questions
invite engagement - ask if anyone has remixed this or similar -->

## References
1. [Plug Building 2023: The Anti-Pike](https://www.thefisherman.com/article/plug-building-2023-the-anti-pike/)
2. [How to Build a Danny style Plug](https://www.stripers247.com/media/categories/how-to-build-a-danny-style-plug.7/)
3. [Tips for 3D Printing Press-Fit Parts](https://makezine.com/article/digital-fabrication/3d-printing-workshop/tips-3d-printing-press-fit-parts/)
4. [Complete 3D Printed Fishing Lure Design Course - Designing the Lure Body](https://youtu.be/7JGIUfx0y8I?si=sHJDN0qpQfNqf2Qc)
