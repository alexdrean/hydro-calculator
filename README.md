# Small Hydro Calculator

[Use live](//alexdrean.github.io/hydro-calculator)

This **Small Hydro Calculator** is a simple, client-side HTML/JavaScript tool designed to help you estimate the electrical power and current output from a small hydro power setup. By entering the following parameters, the calculator dynamically computes:

* **Pressure (PSI)**: The static pressure driving the flow through an orifice.
* **Nozzle Size (inches)**: The diameter of the nozzle (from 1/8" to 7/16").
* **Voltage (V)**: The system voltage at which the generated power is delivered.
* **Coefficient of Discharge (Cd %)**: The efficiency factor that accounts for losses through the orifice.
* **Efficiency (%)**: Overall system efficiency (turbine + generator + mechanical).

## How It Works

1. **Flow Calculation**: Uses the orifice flow equation:

   $Q = C_d \times A \times \sqrt{\frac{2 \Delta P}{\rho}}$

   where $Q$ is volumetric flow (m³/s), $C_d$ is the coefficient of discharge (decimal), $A$ is the orifice area (m²), $\Delta P$ is pressure (Pa), and $\rho$ is water density (assumed 1000 kg/m³).
2. **Power Calculation**: Computes hydraulic power as

   $P_{hydraulic} = Q \times \Delta P$

   and multiplies by system efficiency to get the electrical output power:

   $P_{output} = P_{hydraulic} \times \text{efficiency}$

##
