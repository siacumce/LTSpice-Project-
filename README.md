# Analog Electronics Amplifier Design

## Project Description
This repository contains LTspice simulations for a multi-stage analog electronics project. The design parameters (such as frequency, input impedance, and gain) are dynamically scaled based on a group number variable (`N_Gr`). 

The project is structured into three main phases:
* **Common Emitter (CE) Amplifier:** Design and simulation of a single-BJT CE amplifier. Includes DC operating point analysis, AC waveform generation, and voltage gain evaluation under both no-load and loaded conditions.
* **Two-Stage Amplifier (CE + CC):** Addition of a Common Collector (CC) output buffer stage to the initial circuit. Involves recalculating operating points and comparing loaded gain performance with the single-stage design.
* **Op-Amp Audio Amplifier:** An audio processing circuit using a non-inverting operational amplifier, preceded by a 1st-order High-Pass Filter (HPF). It processes a `.wav` file input, strictly adhering to variable constraints for RMS voltage, maximum amplitude, and specified gain targets.

## Prerequisites
* **LTspice:** [Download and install LTspice](https://www.analog.com/en/design-center/design-tools-and-calculators/ltspice-simulator.html).
* A compatible `.wav` audio file for the Op-Amp simulation phase.

## How to Run
1. Clone this repository to your local machine:
   `git clone [your-repository-url]`
2. Open **LTspice**.
3. Go to `File > Open` and select the `.asc` schematic files from the cloned folder.
4. Click the **Run** button (the running figure icon) to execute the simulation.
5. Probe the nodes in the schematic to view the AC/DC waveforms and verify the gains.

## Notes
Simulation data files (`.raw`, `.log`) are intentionally ignored via `.gitignore` to keep the repository lightweight. Run the simulations locally to generate the waveform data.