---
concept: beam-bending
topic: materials
difficulty: intermediate
tags:
  - inertia
  - theoretical-deflection
  - youngs-modulus
  - stress
  - strain
  - lab
status: learning
week: 4
---
By analyzing and collecting data, we can determine how solid materials exhibit an elastic, spring-like response when force is applied. 

## Stress ($\sigma$)
---
**Stress** is how much force is being applied over an **area**. For example you need to add more force to a thick, wide rubber band but less force to a needle on a balloon to pop it.

Stress = How "concentrated" the force is.

$$\sigma = \frac{F}{A}$$
**Where:**
- $\sigma$ = Stress (Pa)
- $F$ = Applied Force (N)
- $A$ = Cross-sectional Area (m²)

## Strain ($\epsilon$)
---
**Strain** is the measurement of how much a material **deforms**, stretches or bends. For example, if you pull a rubber band from its initial length of 10 cm to 12 cm, the strain was 2 cm.

Strain = How much it "gives" or deforms.

$$\epsilon = \frac{\Delta L}{L_0}$$
**Where:**
- $\epsilon$ = Strain (unitless)
- $\Delta L$ = Change in Length (m)
- $L_0$ = Original Length (m)

## Young's Modulus ($E$)
---
Young's Modulus is a material's **resistance to being stressed**, showing how still or flexible it is. For example, a steel rod has a high Young's Modulus compared to rubber band.
$$E = \frac{\sigma}{\epsilon} = \frac{FL_0}{A\Delta L}$$
**Where:**
- $E$ = Young's Modulus (Pa)
- $\sigma$ = Stress (Pa)
- $\epsilon$ = Strain (unitless)

| Material       | Young's Modulus (GPa) | Young's Modulus (psi) |
| -------------- | --------------------- | --------------------- |
| Polystyrene    | 3                     | 435,000               |
| Basswood       | 35                    | 5,000,000             |
| Aluminum       | 70                    | 10,000,000            |
| Carbon Fiber   | 70                    | 10,000,000            |
| Titanium       | 105                   | 15,000,000            |
| Copper         | 130                   | 18,900,000            |
| Steel (carbon) | 210                   | 30,000,000            |
| Diamond        | 1050                  | 150,000,000           |

In many cases, engineers design structures so that the maximum stress in buildings or airplanes will never exceed the Proportional Limit (Point 2), even under the most adverse conditions.

![[Pasted image 20251004150710.png]]

## Moment of Inertia (I)
---
Moment of Inertia measures the shape's effectiveness at resisting bending, for example bending a rectangle is more difficult if you bend it on its side. For example, the orientation changes its resistance to bending. 

$$I = \frac{w \cdot t^3}{12}$$
**Where:**
- $I$ = Moment of Inertia (m⁴ or in⁴)
- $w$ = Width of the beam
- $t$ = Thickness/height of the beam

#### 1. Thickness is Cubed ($t^3$)
- Thickness has a **massive effect** on stiffness
- Doubling the thickness makes the beam **8 times** stiffer (since $2^3 = 8$)
- This explains why putting material far from the center (like in I-beams) is so effective

#### 2. Pure Geometry Factor
- Notice the formula only uses dimensions ($w$ and $t$)
- A steel beam and wooden beam with same $w$ and $t$ have the **same $I$**
- Material differences are handled by **Young's Modulus ($E$)**
## Summary
---
**Putting It All Together:**
- **Stress** is how hard you push them.
- **Strain** is how far they stumble.
- **Young's Modulus** is their inherent "stability."

Pulling on a rubber band (low Young's Modulus) causes a lot of deformation and stretching (strain), even with a small pulling (stress).
