# 16S1P-Passive-cell-Balancing-then-Discharging-or-Charging-for-Li-ion-battery-pack-used-in-EVs
This repository contains the simulation and control implementation of passive cell balancing followed by discharging or charging, based on the Minimum State of Charge (Min SoC) strategy, for a 16S1P lithium-ion battery pack commonly used in electric vehicles (EVs).It focuses on enhancing battery safety, lifespan, and efficiency by addressing the issue of cell voltage or state-of-charge (SoC) imbalance in a series-connected battery configuration.


📌 Project Objective
The goal of this project is to:

Ensure all cells in the series configuration reach a balanced state before the main charging or discharging process begins.

Use Min SoC-based logic to prevent over-discharge of weaker cells during pack operation.

Simulate safe, efficient, and reliable battery operation using passive balancing techniques.

⚙️ System Configuration
Battery Type: Li-ion

Pack Configuration: 16S1P (16 cells in series, 1 parallel)

Balancing Type: Passive (resistive discharge method)

Balancing Trigger: Before pack discharge/charge

Balancing Strategy: Higher SoC cells are discharged down to the SoC of the weakest cell (Min SoC)

Simulation Tool: MATLAB/Simulink



🧠 Methodology
Initial Condition:

All 16 cells have different initial SoC levels (non-uniform).

Passive Cell Balancing:

Cells with SoC higher than the minimum SoC are discharged using resistors until all cells are at or near the same SoC level.

Post-Balancing Operation:

Once balanced, the pack undergoes either:

Discharging (e.g., during EV operation), or

Charging (e.g., regenerative braking or plug-in charging)

Monitoring:

Includes basic protection against under-voltage and over-voltage.



📊 Simulation Results
Before Balancing: SoC values across cells are scattered.

After Balancing: All cells are nearly equal to the minimum SoC.

Post-Balancing Operation: Smooth and safe discharge/charge with reduced risk of cell mismatch or damage.



💡 Applications
EV Battery Management System (BMS) development

Cell balancing algorithm testing and optimization

Academic projects on battery modeling and control

Research in EV safety and battery longevity




✅ Key Advantages
Improves safety by preventing over-discharge

Enhances battery pack lifespan through uniform SoC control

Provides a scalable method for larger battery systems (e.g., 16S, 32S)

Helps in understanding real-world battery dynamics through simulation




🛠 Requirements
MATLAB 

Simulink and Simscape (Electrical)

Basic understanding of BMS and battery modeling



🏭 Industrial Visit: Palis Eco Vehicle Pvt. Ltd.
As part of this project, an industrial visit was conducted at Palis Eco Vehicle Pvt. Ltd., a Bengaluru-based company specializing in the manufacturing of electric buggies and lightweight EVs.

During the visit, we observed the practical implementation of 16S1P lithium-ion battery packs in their electric vehicles. These battery packs are designed with a focus on modularity, safety, and cost-effectiveness, aligning well with the objectives of our simulation.

This visit provided valuable real-world insights into:

Battery integration and packaging techniques in EVs

Thermal and electrical safety considerations in live systems

Balancing strategy requirements for effective BMS performance

The importance of SoC uniformity for vehicle efficiency and battery longevity

The experience bridged the gap between simulation and industry practice, reinforcing the importance of robust battery management strategies like the one developed in this project.
