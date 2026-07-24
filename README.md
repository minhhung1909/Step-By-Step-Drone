### 🚀 Day 1: Power Management Architecture & Schematic Design
* **Fixed & Verified Output Rails**: Finalized the power tree architecture for the 4-in-1 FOC ESC[cite: 1].
* **Buck Converter Stage (MP2359)**: Configured the step-down regulator to efficiently drop the main battery voltage down to a stable 5V rail.
* **LDO Linear Regulator Stage (MIC5219-3.3)**: Integrated the ultra-low noise LDO to convert 5V to 3.3V, ensuring a clean analog supply (`VDDA`) for the STM32G431 MCU and preventing FOC current-sensing noise.
* **Schematic Captures**: 
  * Configured proper bootstrapping components and decoupling/filtering capacitors.
  * Set up component attributes (such as DNP for optional feed-forward configurations) to keep the BOM clean for manufacturing.