---
subject: Electrical Engineering
course: ENGR 1181 - Fundamentals of Engineering
exam_type: midterm
date: 2025-10-06
total: 100
your_score:
topics_covered:
tags:
  - exam
  - midterm
---
# Electrical Engineering Fundamentals Exam

## Progressive Learning Assessment

**Time Allowed: 90 minutes**  
**Total Points: 100**

**Instructions:** Select the best answer for each question. Each question is worth 4 points unless otherwise noted. Questions are arranged from basic to advanced within each category to build your understanding progressively.

**Note:** Circuit diagrams are provided using CircuiTikZ notation rendered with TikZJax.

---

## Category 1: Ohm's Law and Basic Power (20 points)

### Question 1

A resistor has 10 V across it and 2 A flowing through it. What is the resistance?

```tikz
\usepackage{circuitikz}
\begin{document}
\begin{circuitikz}
\draw (0,0) to [R, l=$R$, v=10V, i=2A] (3,0);
\node at (4.5,0) {$R = ?$};
\end{circuitikz}
\end{document}
```

A) 5 Ω  
B) 12 Ω  
C) 20 Ω  
D) 8 Ω

### Question 2

Using Ohm's Law, if $R = 50$ Ω and $I = 0.5$ A, what is the voltage?

A) 100 V  
B) 25 V  
C) 50 V  
D) 10 V

### Question 3

A device operates at 120 V and draws 5 A. What power does it consume?

```tikz
\usepackage{circuitikz}
\begin{document}
\begin{circuitikz}
\draw (0,0) to[V, v=120V] (0,3)
      to[generic, l=Device, i=$5A$] (4,3)
      to[short] (4,0)
      to[short] (0,0);
\node at (5,1.5) {$P = ?$};
\end{circuitikz}
\end{document}
```

A) 24 W  
B) 600 W  
C) 125 W  
D) 300 W

### Question 4

If a resistor dissipates 100 W when 5 A flows through it, what is its resistance?

A) 20 Ω  
B) 4 Ω  
C) 500 Ω  
D) 0.05 Ω

### Question 5

A 1500 W heater operates on 120 V. If electricity costs $0.12 per kWh, how much does it cost to run for 5 hours?

A) $0.60  
B) $0.90  
C) $1.20  
D) $1.50

---

## Category 2: DC Circuits - Resistance Combinations (20 points)

### Question 6

Two resistors, 10 Ω and 20 Ω, are connected in series. What is the total resistance?

```tikz
\usepackage{circuitikz}
\begin{document}
\begin{circuitikz}
\draw (0,0) to[R, l=$10\Omega$] (2,0) 
      to[R, l=$20\Omega$] (4,0);
\end{circuitikz}
\end{document}
```

A) 15 Ω  
B) 30 Ω  
C) 6.67 Ω  
D) 200 Ω

### Question 7

Two identical 10 Ω resistors are connected in parallel. What is the equivalent resistance?

```tikz
\usepackage{circuitikz}
\begin{document}
\begin{circuitikz}
\draw (0,0) to[short, *-] (0,0)
      (0,0) -- (0,1) to[R, l=$10\Omega$] (2,1) -- (2,0)
      (0,0) -- (0,-1) to[R, l=$10\Omega$] (2,-1) -- (2,0)
      (2,0) to[short, -*] (2,0);
\end{circuitikz}
\end{document}
```

A) 20 Ω  
B) 10 Ω  
C) 5 Ω  
D) 2.5 Ω

### Question 8

Three resistors (6 Ω, 12 Ω, and 4 Ω) are connected in parallel. What is the total resistance?

```tikz
\usepackage{circuitikz}
\begin{document}
\begin{circuitikz}
\draw (0,0) to[short, *-] (0,0)
      (0,0) -- (0,1.5) to[R, l=$6\Omega$] (3,1.5) -- (3,0)
      (0,0) -- (0,0) to[R, l=$12\Omega$] (3,0)
      (0,0) -- (0,-1.5) to[R, l=$4\Omega$] (3,-1.5) -- (3,0)
      (3,0) to[short, -*] (3,0);
\end{circuitikz}
\end{document}
```

A) 22 Ω  
B) 2 Ω  
C) 8 Ω  
D) 3 Ω

### Question 9

A circuit has two parallel branches. Branch 1 is 20 Ω, Branch 2 is 30 Ω. If the total current is 10 A, what current flows through the 20 Ω resistor?

```tikz
\usepackage{circuitikz}
\begin{document}
\begin{circuitikz}
\draw (0,0) node[left]{$I_{total}=10A$} to[short, i=$I_{total}$] (1,0)
      (1,0) -- (1,1.5) to[R, l=$R_1=20\Omega$, i>^=$I_1$] (4,1.5) -- (4,0)
      (1,0) -- (1,-1.5) to[R, l=$R_2=30\Omega$, i>^=$I_2$] (4,-1.5) -- (4,0)
      (4,0) to[short] (5,0);
\end{circuitikz}
\end{document}
```

A) 4 A  
B) 6 A  
C) 5 A  
D) 3.33 A

### Question 10

In a voltage divider with $V_{in} = 36$ V, $R_1 = 18$ kΩ, and $R_2 = 6$ kΩ (series connection, output across $R_2$), what is $V_{out}$?

```tikz
\usepackage{circuitikz}
\begin{document}
\begin{circuitikz}
\draw (0,0) to[V, v=$V_{in}=36V$] (0,3)
      to[R, l=$R_1=18k\Omega$] (0,5)
      to[short] (2,5)
      (2,5) to[R, l=$R_2=6k\Omega$, v^=$V_{out}$] (2,3)
      to[short] (0,3)
      (2,3) to[short] (2,0)
      to[short] (0,0);
\draw[-latex] (3,3) -- (3,5) node[midway, right]{$V_{out}$};
\end{circuitikz}
\end{document}
```

A) 12 V  
B) 9 V  
C) 27 V  
D) 18 V

---

## Category 3: AC Fundamentals and Impedance (20 points)

### Question 11 

What is the angular frequency (ω) of a 60 Hz AC signal?

A) 60 rad/s  
B) 120π rad/s  
C) 377 rad/s  
D) 188.5 rad/s

### Question 12

An AC voltage has a peak value of 339 V. What is its RMS value?

A) 170 V  
B) 240 V  
C) 339 V  
D) 480 V

### Question 13

What is the impedance magnitude of a 100 mH inductor at 50 Hz?

```tikz
\usepackage{circuitikz}
\begin{document}
\begin{circuitikz}
\draw (0,0) to[sV, v=$V_{AC}$] (0,2.5)
      to[L, l=$L=100mH$, i=$I$] (3,2.5)
      to[short] (3,0)
      to[short] (0,0);
\node at (4.5,1.25) {$Z_L = ?$};
\end{circuitikz}
\end{document}
```

A) 5 Ω  
B) 15.7 Ω  
C) 31.4 Ω  
D) 50 Ω

### Question 14 

What is the impedance magnitude of a 100 μF capacitor at 60 Hz?

```tikz
\usepackage{circuitikz}
\begin{document}
\begin{circuitikz}
\draw (0,0) to[sV, v=$V_{AC}$] (0,2.5)
      to[C, l=$C=100\mu F$, i=$I$] (3,2.5)
      to[short] (3,0)
      to[short] (0,0);
\node at (4.5,1.25) {$Z_C = ?$};
\end{circuitikz}
\end{document}
```

A) 26.5 Ω  
B) 37.7 Ω  
C) 16.7 Ω  
D) 60 Ω

### Question 15

An AC circuit has $V_{rms} = 120$ V, $I_{rms} = 10$ A, and power factor = 0.6. What is the real power consumed?

A) 1200 W  
B) 720 W  
C) 600 W  
D) 960 W

---

## Category 4: Energy Storage Elements (16 points)

### Question 16

Three capacitors (10 μF, 20 μF, 30 μF) are connected in parallel. What is the total capacitance?

```tikz
\usepackage{circuitikz}
\begin{document}
\begin{circuitikz}
\draw (0,0) to[short, *-] (0,0)
      (0,0) -- (0,1.5) to[C, l=$10\mu F$] (3,1.5) -- (3,0)
      (0,0) -- (0,0) to[C, l=$20\mu F$] (3,0)
      (0,0) -- (0,-1.5) to[C, l=$30\mu F$] (3,-1.5) -- (3,0)
      (3,0) to[short, -*] (3,0);
\end{circuitikz}
\end{document}
```

A) 5.45 μF  
B) 20 μF  
C) 60 μF  
D) 6000 μF

### Question 17

Three capacitors (10 μF, 20 μF, 30 μF) are connected in series. What is the total capacitance?

```tikz
\usepackage{circuitikz}
\begin{document}
\begin{circuitikz}
\draw (0,0) to[C, l=$10\mu F$] (2,0)
      to[C, l=$20\mu F$] (4,0)
      to[C, l=$30\mu F$] (6,0);
\end{circuitikz}
\end{document}
```

A) 60 μF  
B) 20 μF  
C) 5.45 μF  
D) 6.67 μF

### Question 18

How much energy is stored in a 100 μF capacitor charged to 200 V?

A) 0.02 J  
B) 2 J  
C) 20 J  
D) 4 J

### Question 19

A 200 mH inductor carries 5 A. How much energy is stored in its magnetic field?

A) 0.5 J  
B) 2.5 J  
C) 5 J  
D) 1 J

---

## Category 5: Three-Phase Systems (16 points)

### Question 20

In a balanced Y-connected system, if the phase voltage is 120 V, what is the line voltage?

```tikz
\usepackage{circuitikz}
\begin{document}
\begin{circuitikz}
\draw (0,0) node[ground]{N} 
      (0,0) to[R, l=$Z_a$] (0,2) node[above]{A}
      (0,0) to[R, l=$Z_b$] (-1.73,-1) node[left]{B}
      (0,0) to[R, l=$Z_c$] (1.73,-1) node[right]{C};
\draw[-latex] (-0.3,0.5) -- (-0.3,1.5) node[midway, left]{$V_{phase}=120V$};
\draw[dashed, red] (-1.73,-1) -- (0,2) node[midway, above left]{$V_{line}=?$};
\end{circuitikz}
\end{document}
```

A) 120 V  
B) 208 V  
C) 240 V  
D) 69.3 V

### Question 21

In a balanced Δ-connected system, if the line voltage is 480 V, what is the phase voltage?

```tikz
\usepackage{circuitikz}
\begin{document}
\begin{circuitikz}
\draw (0,0) node[above left]{A} 
      to[R, l=$Z_{ab}$] (3,0) node[above right]{B}
      to[R, l=$Z_{bc}$] (1.5,-2.6) node[below]{C}
      to[R, l=$Z_{ca}$] (0,0);
\draw[-latex] (0.3,0) -- (2.7,0) node[midway, above]{$V_{line}=480V$};
\draw[-latex, blue] (1.2,-0.3) -- (2.3,-0.3) node[midway, below]{$V_{phase}=?$};
\end{circuitikz}
\end{document}
```

A) 277 V  
B) 480 V  
C) 831 V  
D) 240 V

### Question 22

In a Y-connected system, if the line current is 15 A, what is the phase current?

A) 26 A  
B) 15 A  
C) 8.66 A  
D) 7.5 A

### Question 23

A balanced three-phase system has $V_L = 400$ V, $I_L = 20$ A, and power factor = 0.9. What is the total real power?

A) 8 kW  
B) 12.47 kW  
C) 7.2 kW  
D) 13.86 kW

---

## Category 6: Integrated Concepts (8 points)

### Question 24

A wire with resistivity $\rho = 1.68 \times 10^{-8}$ Ω·m, length 100 m, and diameter 2 mm carries 10 A. What is the power loss in the wire?

A) 5.35 W  
B) 53.5 W  
C) 535 W  
D) 10.7 W

### Question 25

In an RLC series circuit at resonance, which statement is TRUE?

```tikz
\usepackage{circuitikz}
\begin{document}
\begin{circuitikz}
\draw (0,0) to[sV, v=$V_{AC}$] (0,3)
      to[R, l=$R$] (2,3)
      to[L, l=$L$] (4,3)
      to[C, l=$C$] (6,3)
      to[short] (6,0)
      to[short] (0,0);
\end{circuitikz}
\end{document}
```

A) Total impedance is maximum  
B) Inductive and capacitive reactances cancel, leaving only resistance  
C) Current is minimum  
D) Power factor is zero

---

# Answer Key with Progressive Explanations

## Category 1: Ohm's Law and Basic Power

### Question 1: **Answer: A) 5 Ω**

**Foundation Concept:** This is the most fundamental application of Ohm's Law: $V = I \times R$

**Solution:** $$R = \frac{V}{I} = \frac{10 \text{ V}}{2 \text{ A}} = 5 \text{ Ω}$$

**Key Insight:** Resistance is the ratio of voltage to current. Higher resistance means more voltage is needed to push the same current through.

---

### Question 2: **Answer: B) 25 V**

**Building on Q1:** Now you're finding voltage instead of resistance using the same formula.

**Solution:** $$V = I \times R = 0.5 \text{ A} \times 50 \text{ Ω} = 25 \text{ V}$$

**Key Insight:** You can rearrange Ohm's Law to find any variable if you know the other two: $V = IR$, $I = V/R$, $R = V/I$

---

### Question 3: **Answer: B) 600 W**

**New Concept Introduction:** Power is the rate of energy consumption. The basic formula is $P = V \times I$

**Solution:** $$P = V \times I = 120 \text{ V} \times 5 \text{ A} = 600 \text{ W}$$

**Key Insight:** Power (in watts) tells you how much energy is used per second. A 600 W device uses 600 joules every second.

**Real-world Connection:** This is like a typical household appliance - maybe a coffee maker or small space heater.

---

### Question 4: **Answer: B) 4 Ω**

**Combining Concepts:** Now you need to use both power and Ohm's Law concepts together.

**Solution:** Use $P = I^2 \times R$ $$R = \frac{P}{I^2} = \frac{100 \text{ W}}{(5 \text{ A})^2} = \frac{100}{25} = 4 \text{ Ω}$$

**Alternative Approach:**

- First find voltage: $V = P/I = 100/5 = 20$ V
- Then find resistance: $R = V/I = 20/5 = 4$ Ω

**Key Insight:** There are often multiple valid paths to the answer. Choose the most direct one!

---

### Question 5: **Answer: B) $0.90**

**Practical Application:** This combines everything you've learned into a real-world cost calculation.

**Solution:**

1. Energy consumed: $E = P \times t = 1.5 \text{ kW} \times 5 \text{ h} = 7.5 \text{ kWh}$
2. Cost: $\text{Cost} = 7.5 \text{ kWh} \times $0.12/\text{kWh} = $0.90$

**Key Insight:** Power is instantaneous (watts), but energy is power over time (watt-hours or kilowatt-hours). Your electric bill charges for energy, not power.

**Why This Matters:** Understanding this helps you estimate costs of running appliances and make energy-efficient decisions.

---

## Category 2: DC Circuits - Resistance Combinations

### Question 6: **Answer: B) 30 Ω**

**Foundation Concept:** In series, current has only one path, so resistances simply add.

**Solution:** $$R_{total} = R_1 + R_2 = 10 \text{ Ω} + 20 \text{ Ω} = 30 \text{ Ω}$$

**Key Insight:** Series means "one after another." Think of obstacles in a single pipe - each one adds resistance.

**Intuition Builder:** Total resistance is always greater than the largest individual resistor.

---

### Question 7: **Answer: C) 5 Ω**

**Conceptual Shift:** Parallel circuits divide current among multiple paths.

**Solution:** $$R_{total} = \frac{R_1 \times R_2}{R_1 + R_2} = \frac{10 \times 10}{10 + 10} = \frac{100}{20} = 5 \text{ Ω}$$

Or using the reciprocal formula: $$\frac{1}{R_{total}} = \frac{1}{10} + \frac{1}{10} = \frac{2}{10} \Rightarrow R_{total} = 5 \text{ Ω}$$

**Key Insight:** For identical resistors in parallel, divide by the number of resistors: $R_{total} = R/n = 10/2 = 5$ Ω

**Intuition Builder:** Adding parallel paths DECREASES total resistance (more ways for current to flow).

---

### Question 8: **Answer: B) 2 Ω**

**Complexity Increase:** Now applying parallel formula to three different resistors.

**Solution:** $$\frac{1}{R_{total}} = \frac{1}{6} + \frac{1}{12} + \frac{1}{4} = \frac{2 + 1 + 3}{12} = \frac{6}{12} = \frac{1}{2}$$ $$R_{total} = 2 \text{ Ω}$$

**Step-by-step Tip:** Find common denominator (12), then add fractions.

**Key Insight:** The total parallel resistance is always less than the smallest resistor (here, less than 4 Ω).

---

### Question 9: **Answer: B) 6 A**

**New Tool: Current Divider:** This teaches you how current splits in parallel branches.

**Solution:** First, find total resistance: $$R_{total} = \frac{20 \times 30}{20 + 30} = \frac{600}{50} = 12 \text{ Ω}$$

Current divider rule: Current goes inversely with resistance! $$I_1 = I_{total} \times \frac{R_2}{R_1 + R_2} = 10 \times \frac{30}{50} = 10 \times 0.6 = 6 \text{ A}$$

**Key Insight:** The SMALLER resistor gets MORE current. Current takes the path of least resistance!

**Verification:** $I_2 = 10 \times (20/50) = 4$ A, and $6 + 4 = 10$ A ✓

---

### Question 10: **Answer: B) 9 V**

**New Tool: Voltage Divider:** Essential for understanding how voltage drops across series resistors.

**Solution:** $$V_{out} = V_{in} \times \frac{R_2}{R_1 + R_2} = 36 \times \frac{6}{18 + 6} = 36 \times \frac{6}{24} = 36 \times 0.25 = 9 \text{ V}$$

**Pattern Recognition:** Output voltage is proportional to the fraction of total resistance.

**Key Insight:** Voltage divider is like splitting money proportionally: if $R_2$ is 1/4 of the total resistance, it gets 1/4 of the voltage.

**Practical Application:** Voltage dividers are used everywhere - sensor circuits, volume controls, biasing circuits.

---

## Category 3: AC Fundamentals and Impedance

### Question 11: **Answer: C) 377 rad/s**

**Foundation Concept:** AC analysis uses angular frequency (radians per second) instead of cycles per second.

**Solution:** $$\omega = 2\pi f = 2\pi \times 60 = 377 \text{ rad/s}$$

**Why This Matters:** In AC circuit equations, we use ω because it relates directly to the phase of sine waves.

**Key Insight:** For 60 Hz (US standard), remember ω ≈ 377 rad/s. For 50 Hz (Europe/Asia), ω ≈ 314 rad/s.

---

### Question 12: **Answer: B) 240 V**

**Critical Concept:** RMS (Root Mean Square) values represent AC equivalents to DC for power calculations.

**Solution:** $$V_{rms} = \frac{V_{peak}}{\sqrt{2}} = \frac{339}{\sqrt{2}} = \frac{339}{1.414} = 240 \text{ V}$$

**Real-world Connection:** When we say "240 V AC," we mean RMS. The actual peak is 339 V!

**Key Insight:** RMS value represents the DC voltage that would deliver the same power. This is why household "120V" outlets actually swing from -170V to +170V.

**Memory Aid:** $\sqrt{2} \approx 1.414$, so RMS ≈ 0.707 × Peak

---

### Question 13: **Answer: C) 31.4 Ω**

**New Concept: Inductive Reactance** - How inductors resist AC current.

**Solution:** $$X_L = \omega L = 2\pi f L = 2\pi \times 50 \times 0.1 = 31.4 \text{ Ω}$$

**Key Insight:** Inductors oppose changes in current. The faster the change (higher frequency), the more they resist.

**Frequency Dependence:** If frequency doubles, inductive reactance doubles. At DC (f=0), $X_L = 0$ (inductor is just a wire).

**Phase Note:** In an inductor, current lags voltage by 90°.

---

### Question 14: **Answer: A) 26.5 Ω**

**New Concept: Capacitive Reactance** - How capacitors resist AC current.

**Solution:** $$X_C = \frac{1}{\omega C} = \frac{1}{2\pi f C} = \frac{1}{2\pi \times 60 \times 100 \times 10^{-6}} = \frac{1}{0.0377} = 26.5 \text{ Ω}$$

**Key Insight:** Capacitors resist slowly changing voltages. Higher frequency means easier current flow (lower reactance).

**Contrast with Inductors:**

- Inductors: Higher f → Higher $X_L$ (more resistance to AC)
- Capacitors: Higher f → Lower $X_C$ (less resistance to AC)

**Phase Note:** In a capacitor, current leads voltage by 90°.

---

### Question 15: **Answer: B) 720 W**

**Advanced Concept: Power Factor** - The "efficiency" of power delivery in AC circuits.

**Solution:** $$P = V_{rms} \times I_{rms} \times \cos(\theta) = 120 \times 10 \times 0.6 = 720 \text{ W}$$

**Breaking It Down:**

- Apparent Power: $S = 120 \times 10 = 1200$ VA (total power flow)
- Real Power: $P = 1200 \times 0.6 = 720$ W (useful power)
- The "missing" 480 VA is reactive power (oscillates back and forth)

**Key Insight:** Power factor of 0.6 means only 60% of the apparent power does useful work. The rest is "wasted" in reactive components.

**Real-world Impact:** Industrial facilities pay penalties for poor power factor because it requires more current for the same useful power.

---

## Category 4: Energy Storage Elements

### Question 16: **Answer: C) 60 μF**

**Pattern Recognition:** Capacitors in parallel combine like resistors in series!

**Solution:** $$C_{total} = C_1 + C_2 + C_3 = 10 + 20 + 30 = 60 \text{ μF}$$

**Physical Intuition:** Parallel capacitors effectively increase the plate area, so total capacitance increases.

**Key Insight:** More capacitance means more charge storage at the same voltage.

---

### Question 17: **Answer: C) 5.45 μF**

**Pattern Recognition:** Capacitors in series combine like resistors in parallel!

**Solution:** $$\frac{1}{C_{total}} = \frac{1}{10} + \frac{1}{20} + \frac{1}{30} = \frac{6 + 3 + 2}{60} = \frac{11}{60}$$ $$C_{total} = \frac{60}{11} = 5.45 \text{ μF}$$

**Physical Intuition:** Series capacitors effectively increase the distance between plates, so total capacitance decreases.

**Memory Aid:** Capacitors are "opposite" of resistors:

- Series: Capacitors use reciprocal formula (like resistors in parallel)
- Parallel: Capacitors add directly (like resistors in series)

---

### Question 18: **Answer: B) 2 J**

**Energy Storage Concept:** Capacitors store energy in electric fields between plates.

**Solution:** $$E = \frac{1}{2}CV^2 = \frac{1}{2} \times 100 \times 10^{-6} \times (200)^2 = 0.5 \times 10^{-4} \times 40000 = 2 \text{ J}$$

**Key Insight:** Energy depends on SQUARE of voltage. Doubling voltage quadruples stored energy!

**Practical Application:** This is why camera flashes use capacitors - they charge slowly, then release energy quickly for the bright flash.

---

### Question 19: **Answer: B) 2.5 J**

**Energy Storage Concept:** Inductors store energy in magnetic fields around coils.

**Solution:** $$E = \frac{1}{2}LI^2 = \frac{1}{2} \times 200 \times 10^{-3} \times (5)^2 = 0.5 \times 0.2 \times 25 = 2.5 \text{ J}$$

**Key Insight:** Energy depends on SQUARE of current. Doubling current quadruples stored energy!

**Comparison:** Both formulas have the $\frac{1}{2}$ factor:

- Capacitor: $E = \frac{1}{2}CV^2$ (voltage squared)
- Inductor: $E = \frac{1}{2}LI^2$ (current squared)

**Practical Application:** Inductors in switching power supplies store energy during one part of the cycle, then release it during another.

---

## Category 5: Three-Phase Systems

### Question 20: **Answer: B) 208 V**

**Foundation Concept:** In Y-connection, line voltage is $\sqrt{3}$ times phase voltage.

**Solution:** $$V_{line} = \sqrt{3} \times V_{phase} = 1.732 \times 120 = 208 \text{ V}$$

**Why $\sqrt{3}$?** The 120° phase shift between phases creates this geometric relationship.

**Real-world Connection:** In North America, 120V phase-to-neutral becomes 208V phase-to-phase in a Y system.

**Key Insight:** Line voltage is always measured between two phases, while phase voltage is measured from one phase to neutral.

---

### Question 21: **Answer: B) 480 V**

**Y vs Δ Distinction:** In a Delta connection, line voltage EQUALS phase voltage.

**Solution:** $$V_{phase} = V_{line} = 480 \text{ V}$$

**Key Insight:** There's no neutral point in a delta connection. Each winding connects directly between two line conductors.

**Memory Aid for Delta:** "V is the same" (line = phase for voltage)

---

### Question 22: **Answer: B) 15 A**

**Y-Connection Current Rule:** Line current equals phase current in a Y-connection.

**Solution:** $$I_{phase} = I_{line} = 15 \text{ A}$$

**Physical Explanation:** In Y-connection, each line wire connects to exactly one winding, so the same current flows through both.

**Memory Aid for Y:** "I is the same" (line = phase for current)

**Complete Y-Connection Summary:**

- $V_{line} = \sqrt{3} \times V_{phase}$ (voltage increases)
- $I_{line} = I_{phase}$ (current stays same)

---

### Question 23: **Answer: B) 12.47 kW**

**Three-Phase Power Formula:** Combines everything you've learned about three-phase systems.

**Solution:** $$P_{total} = \sqrt{3} \times V_L \times I_L \times pf = 1.732 \times 400 \times 20 \times 0.9 = 12,470 \text{ W} = 12.47 \text{ kW}$$

**Breaking Down the Formula:**

- $\sqrt{3}$ accounts for the three phases (1.732 ≈ 1.73)
- $V_L \times I_L$ gives apparent power per phase (scaled)
- $pf$ (power factor) gives real vs. apparent power ratio

**Key Insight:** Three-phase systems deliver MORE power than three times single-phase because the phases are staggered, maintaining more constant power delivery.

**Real-world Application:** Industrial motors and large facilities use three-phase because it's more efficient for high-power applications.

---

## Category 6: Integrated Concepts

### Question 24: **Answer: B) 53.5 W**

**Multi-Step Problem:** Combines resistivity, geometry, Ohm's Law, and power concepts.

**Solution:**

**Step 1:** Find cross-sectional area  
Diameter = 2 mm, so radius = 1 mm = 0.001 m $$A = \pi r^2 = \pi \times (0.001)^2 = 3.14159 \times 10^{-6} \text{ m}^2$$

**Step 2:** Find resistance $$R = \frac{\rho L}{A} = \frac{1.68 \times 10^{-8} \times 100}{3.14159 \times 10^{-6}} = \frac{1.68 \times 10^{-6}}{3.14159 \times 10^{-6}} = 0.535 \text{ Ω}$$

**Step 3:** Find power loss $$P = I^2 R = (10)^2 \times 0.535 = 100 \times 0.535 = 53.5 \text{ W}$$

**Key Insight:** Power loss in transmission lines is proportional to $I^2$. This is why high-voltage transmission is used (lower current for same power).

**Real-world Application:** This 53.5 W loss over 100m might seem small, but over thousands of kilometers in power lines, losses add up significantly. This is why utilities use very high voltages (hundreds of kV) to minimize current and thus minimize $I^2R$ losses.

---

### Question 25: **Answer: B) Inductive and capacitive reactances cancel, leaving only resistance**

**Fundamental Concept:** Resonance is a critical phenomenon in AC circuits.

**Explanation:**

At resonance in a series RLC circuit:

- $X_L = X_C$ (inductive reactance equals capacitive reactance)
- They cancel because they're 180° out of phase
- Total impedance: $Z = R + j(X_L - X_C) = R + j(0) = R$
- Impedance is at MINIMUM (only resistance remains)
- Current is at MAXIMUM (Ohm's Law: max I when Z is minimum)
- Power factor = 1 (purely resistive, voltage and current in phase)

**Why Other Answers Are Wrong:**

- A) Impedance is minimum, not maximum
- C) Current is maximum, not minimum
- D) Power factor is 1 (unity), not zero

**Real-world Application:** Resonance is used in:

- Radio tuning (select specific frequency)
- Filters (pass or block certain frequencies)
- Wireless power transfer
- Musical instruments

**Key Insight:** Resonance occurs when $\omega_0 = 1/\sqrt{LC}$. At this frequency, the circuit "rings" naturally.

---

**End of Exam - Congratulations!**

By progressing through this exam, you've built understanding from simple Ohm's Law to complex three-phase power systems. Each question was designed to prepare you for the next, building confidence and competence systematically.

**Study Tips for Next Time:**

1. Master the fundamentals first (Category 1-2)
2. Understand the physical meaning, not just formulas
3. Practice identifying which formula to use
4. Check your units - they reveal calculation errors
5. Draw circuit diagrams when confused