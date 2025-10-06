---
concept: circuits
topic: basic-electricity
difficulty: intermediate
tags:
  - ohms-law
  - power
  - resistor
  - voltage
  - circuit
  - resistance
  - resistivity
  - voltage
  - lab
---
### 1. Resistivity (ρ - "Rho")

**The Simple Idea:** Resistivity is a material's **innate ability to resist the flow of electric current**. It's like the "friction" inside the material itself.

*   **Good Conductors** (like Copper, Silver): Have **very low resistivity**. It's like a smooth, wide-open pipe. Electrons flow easily.
*   **Good Insulators** (like Rubber, Glass): Have **very high resistivity**. It's like a pipe clogged with sponges. Electrons cannot flow.
*   **Resistors** (like Carbon): Have a medium, controlled resistivity. We use them to manage current flow in circuits.

**The Formula:**
Resistivity (ρ) is a fundamental property of the material. We use it to *calculate* resistance.

### 2. Resistance (R)

**The Simple Idea:** Resistance is the **actual, measurable opposition to current flow in a specific object**. It depends on two things:
1.  The material it's made from (its **Resistivity**).
2.  Its physical shape and size.

Let's go back to the water pipe analogy:
*   **Longer Pipe = Harder for water to flow = Higher Resistance.**
*   **Sker Pipe = Easier for water to flow = Lower Resistance.**

**The Formula:**
The resistance `R` of a uniform object is given by:

$$R = \rho \frac{L}{A}$$

Where:
*   `R` = Resistance (in Ohms, Ω)
*   `ρ` (rho) = Resistivity of the material (in Ω⋅m)
*   `L` = Length of the object (in meters, m)
*   `A` = Cross-sectional Area of the object (in square meters, m²)

**Example:** A long, thin copper wire has more resistance than a short, thick copper wire, even though they are both made of the same material (same ρ).

---

### 3. Ohm's Law: The Relationship Between Voltage, Current, and Resistance

This is the most important law in basic circuit theory.

**The Simple Idea:**
*   **Voltage (V):** The "electrical pressure" that pushes the electrons. (Like water pressure in a pipe).
*   **Current (I):** The "flow rate" of the electrons. (Like the flow of water in gallons per minute).
*   **Resistance (R):** The "restriction" that opposes the flow.

Ohm's Law states: **The current through a conductor between two points is directly proportional to the voltage across the two points and inversely proportional to the resistance between them.**

**The Formula:**

$$V = I R$$

Or, rearranged:

$$I = \frac{V}{R}$$

$$R = \frac{V}{I}$$

Where:
*   `V` = Voltage (in Volts, V)
*   `I` = Current (in Amperes, A)
*   `R` = Resistance (in Ohms, Ω)

**Example:** If you increase the voltage (pressure) across a resistor, the current (flow) will increase. If you increase the resistance (make it harder to flow), the current will decrease for the same voltage.

---

### 4. Electrical Power (P)

**The Simple Idea:** Power is the **rate at which electrical energy is used, delivered, or converted** into another form (like heat, light, or motion). It's measured in **Watts (W)**.

Think of a light bulb:
*   A 100W bulb converts electrical energy into light and heat **faster** than a 60W bulb. It's "using up" the energy more quickly.

**The Formulas:**
The most fundamental power formula is:

$$P = V I$$

(Power = Voltage × Current)

By combining this with Ohm's Law (`V = IR`), we get two other very useful formulas:

$$P = I^2 R$$

$$P = \frac{V^2}{R}$$

Where:
*   `P` = Power (in Watts, W)
*   `V` = Voltage (in Volts, V)
*   `I` = Current (in Amperes, A)
*   `R` = Resistance (in Ohms, Ω)

**Example:** Why do resistors get hot? When current `I` flows through a resistance `R`, power is dissipated as heat according to `P = I²R`. This is why high-power circuits need larger resistors or heatsinks.

---

### 5. Conductivity (σ - "Sigma")

**The Simple Idea:** Conductivity is simply the **opposite of Resistivity**. It's a measure of how *easily* a material conducts electric current.

**The Formula:**

$$\sigma = \frac{1}{\rho}$$

Where:
*   `σ` (sigma) = Conductivity (in Siemens per meter, S/m)
*   `ρ` (rho) = Resistivity (in Ω⋅m)

### Summary & Practical Application

Let's connect it all with a real-world scenario: **Choosing a wire for a circuit.**

1.  **Material Choice (Resistivity ρ):** You choose **copper** because it has a low ρ (it's a good conductor). You wouldn't choose rubber (high ρ).
2.  **Wire Sizing (Resistance R):** You calculate the needed Resistance `R` for your circuit. For a long wire run, you might need a thicker wire (larger area `A`) to keep the resistance `R = ρL/A` low and prevent power loss.
3.  **Circuit Design (Ohm's Law):** You use `V = IR` to figure out how much current `I` will flow through your wire and components for a given voltage `V`.
4.  **Component Rating (Power P):** You check that your resistor can handle the power using `P = I²R`. A 1/4W resistor would burn up in a circuit where `P = 1W`.

You now have the basic toolkit! These concepts of Voltage, Current, Resistance, Resistivity, and Power are the foundation upon which all of electronics is built.

