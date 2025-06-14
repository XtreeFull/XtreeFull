# Bachelor Thesis: Novel High-Torque Locking Ball Joint

For my bachelor's thesis, I single-handedly designed, prototyped, and validated a novel, high-performance locking ball joint for robotics. The project addressed a critical weakness in modern robotics: the inability of most robotic joints to withstand high torques, which limits their use in demanding applications.

<div align="center">
  <img src="../images/ball-joint-cad-vs-reality.png" alt="CAD model and physical prototype of the locking ball joint" width="70%">
</div>

> *Image Description: The final CAD design alongside the functional, 3D-printed prototype.*

---

### The Challenge

Most locking ball joints used in research for applications like wearable or walking robots are surprisingly weak, often failing at torques below 1 Nm. This severely limits their real-world utility. The challenge was to engineer a new, compact, and efficient locking ball joint from the ground up that could dramatically outperform these existing solutions.

The primary design goals were:
* **High Holding Torque:** Withstand over 10 Nm for a plastic prototype and project to over 250 Nm for a steel version.
* **Fast & Efficient Actuation:** Lock and unlock quickly with minimal power consumption.
* **Compactness & Simplicity:** Ensure the design was small, lightweight, and easy to maintain.

---

### My Design Process & Solution

After analyzing existing concepts, I chose a mechanical, gear-based locking mechanism as the most promising path for high torque resistance. My design process was highly iterative:

1.  **Systematic Actuation Testing:** I prototyped and evaluated four different actuation mechanisms (Solenoid/Spring, Servo/Lead Screw, Pneumatic, DC Motor) before selecting a **non-captive pancake stepper motor**. This choice provided the best combination of compact size, high precision, and crucial safety features.

2.  **Mechanical Refinement & Analysis:** I solved critical design challenges like the "drawer effect" (self-wedging) in the brake guides by refining the component geometry. I performed force calculations using the **Lewis Form Factor** to ensure the gear teeth could withstand extreme loads.

3.  **Final Design:** The final design uses two brakes that press onto a central gear ball. The non-captive stepper motors drive M5 lead screws, providing precise and strong clamping force. A key feature is that the mechanism is **not back-drivable**, meaning it remains securely locked even with zero power, ensuring safety and energy efficiency.

<div align="center">
  <img src="../images/ball-joint-performance-comparison.png" alt="Graph comparing the performance of my ball joint to other designs" width="80%">
</div>

> *Image Description: Performance graph showing my design (top yellow line) is significantly stiffer and stronger than other state-of-the-art locking mechanisms (lower blue and red lines).*

---

### Key Achievements

* **Engineered a prototype that achieved ~20 Nm of holding torque**—over **40 times stronger** than comparable academic designs which were limited to less than 0.5 Nm.
* **Designed for extreme efficiency**, requiring **200 times less actuation torque** (10 Nmm vs. 4 Nm) to engage than an equivalent commercial steel joint.
* **Validated industrial-grade performance with FEA**, projecting a maximum holding torque of **over 700 Nm** for a CNC-machined steel version of the design.
* **Conducted a rigorous, iterative design process**, systematically prototyping and testing multiple actuation systems and tooth geometries to find the optimal configuration.
* **Authored a comprehensive 40-page thesis** detailing the entire research, design, and validation process.

<div align="center">
  <img src="../images/ball-joint-fea-analysis.png" alt="FEA analysis of the ball joint components" width="90%">
</div>

> *Image Description: Finite Element Analysis (FEA) performed in Fusion 360, used to validate the structural integrity of the components under load and project the performance of industrial-grade materials.*

---

### Core Technologies & Skills

* **Mechanical Design:** 3D CAD (Fusion 360), Geometric Dimensioning & Tolerancing (GD&T), Design for Manufacturability (DFM).
* **Mechanical Analysis:** Finite Element Analysis (FEA), Classical Mechanics (Lewis Form Factor, Frictional Force Calculations).
* **Prototyping:** FDM 3D Printing (PLA), System Integration (Arduino, Stepper Motors & Drivers).
* **Experimental Validation:** Designing and executing physical test procedures using a Zwick universal testing machine.

* [Back to Main Page](../README.md)
