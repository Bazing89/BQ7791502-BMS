# BQ7791502 BMS-
Overview
  This project is a compact Battery Management System design using the BQ7791502 IC from Texas Instruments. It is specifically tailored for space-constrained builds like one-wheel and electric skateboards. The BMS features active cell balancing, overcharge protection, and temperature monitoring, ensuring efficient and safe battery management.

![Screenshot 2023-08-12 231647](https://github.com/Bazing89/Onewheel-PEV-Open-source-BMS-/assets/46078524/67177b8c-d4ab-4fdb-a063-5eb55b8456b0)

Features
	•	20s Battery Compatibility: (Each IC handles 5 cells and can be stacked)
	•	Active Cell Balancing:
	•	Redistributes excess charge from overcharged cells to undercharged ones.
	•	Highly efficient with minimal heat generation.
	•	Overheating Protection:
	•	Automatically stops charging at temperatures between 55°C and 60°C.
	•	Charge-Only Design:
	•	Optimized for charging with no discharging circuitry.
	•	Regenerative Braking Protection:
	•	Configured to charge to 98-99% to prevent overcharging during regenerative braking.
	•	Balancing Logic:
	•	Starts balancing at 4.15v per cell State of Charge (SOC) and continues until 99%.
	•	Automatically resumes charging after dropping to 97% SOC.
	•	Compact Form Factor:
	•	Dimensions: 25mm x 100mm.
	•	Fits seamlessly in small spaces for one-wheel builds.
	•	Charging Capabilities:
	•	Recommended charging current: 10A (supports up to 20A).


Specifications

Feature	Details
Supported Cells	20S
Balancing Type	Active Cell Balancing
Balancing Start SOC	~ 4.15v cell
Balancing End SOC	~• Balancing continues until the voltage differences between cells are reduced to within a specified range, ensuring all cells are evenly charged.
Charge Limit Cutoff	98-99%
Overheat Protection	Stops charging at 55°C-60°C
Charging Current	10A (recommended), 20A (max)
Dimensions	25mm x 100mm

Advantages
	•	Efficient Charging:
	•	Generates minimal heat compared to passive balancing systems.
	•	Eliminates the need for large heat sinks.
	•	Safety Features:
	•	Protects against overcharging and overheating.
	•	Compatible with regenerative braking systems.
	•	No coding required; preconfigured IC from the factory.

Limitations
	•	Preconfigured IC:
	•	Balancing parameters cannot be customized as the BQ7791502 IC is factory-set.
	•	Charge-Only Design:
	•	No discharge protection, requiring a separate discharge circuit for safety.


Usage Notes
	•	Leave Plugged In:
	•	The BMS will automatically resume charging if the charge drops to 97%, allowing the board to remain plugged in for long durations.
	•	Although active balancing generates minimal heat, small heatsinks can be used on the MOSFETs for higher charging speeds.

Sources
BQ7791502 Datasheet.

If there are any issues with my schematic or routing please feel free to give me feedback by opening a ticket.




