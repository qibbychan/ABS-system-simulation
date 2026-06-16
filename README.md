
<img width="1287" height="492" alt="image" src="https://github.com/user-attachments/assets/4d10eb57-a9b3-4ce0-b6cf-b93d1065510f" />

# Anti-lock Braking System (ABS) Simulation using MATLAB/Simulink
---

## 🛠️ Project Overview (5W 1H Analysis)
* **What:** A MATLAB/Simulink simulation model analyzing the dynamics of an Anti-lock Braking System (ABS).
* **Why:** To prevent wheel lock-up during emergency braking, ensuring vehicle stability and maintaining maximum tire-road friction.
* **Who:** Developed as a computer/electronic engineering control system project.
* **When:** Analyzed over a critical braking duration of **10.0 seconds**.
* **Where:** Built and tested digitally in the MATLAB/Simulink environment using a quarter-car mathematical model.
* **How:** Utilizes a **1-D Lookup Table** based on a custom Mu-Slip curve to monitor wheel slip. A bang-bang controller cycles the brake pressure automatically to maintain slip at the optimal target of **0.2**.

---

## Key Findings & Scope Results
Upon running the simulation, the system successfully demonstrated standard ABS behavior across four critical parameters:
1. **Wheel Slip:** Safely oscillated around the optimal **0.2** zone, validating that the bang-bang controller effectively prevents total lock-up.
2. **Wheel Speed:** Exhibited a steady, cyclic "wavy" decline rather than a sudden drop to zero, proving active brake pressure modulation.
3. **Vehicle Angular Speed:** Decreased smoothly from 35 to 15 rad/s, showing stable chassis deceleration despite rapid wheel braking cycles.
4. **Stopping Distance:** Plotted a clean progress curve, demonstrating controlled forward motion without losing lateral stability.

---

## Conclusion
The simulation successfully demonstrates that a bang-bang control algorithm can effectively govern tire slip dynamics. By keeping the wheel slip locked near the peak friction window (~0.2), the system actively maximizes deceleration force, minimizes stopping distances, and successfully keeps the vehicle steerable during hard braking.

---

## 🎥 References & Credits
* **Tutorial Reference:** This simulation model and its physical parameters are built based on the guidance from the video tutorial *"Anti-lock Braking System (ABS) Simulation using MATLAB / Simulink"* by **Stephen Kingston**.
