### Thyristor Circuit Simulation with DC Supply and Resistive Load

#### Overview
This repository demonstrates the simulation of a Thyristor-based circuit using a DC supply with a purely resistive (R) load. The primary focus is on understanding the operation of the Thyristor and analyzing the output waveform generated by this setup.

#### Simulation Components
1. **DC Voltage Source**: Provides the necessary input voltage for the circuit.
2. **Thyristor**: A semiconductor device used as a switch to control the flow of current through the resistive load.
3. **Resistive Load (R)**: The load in this simulation is purely resistive, ensuring that the voltage and current are in phase.
4. **Pulse Generator**: Generates the gate pulses required to trigger the Thyristor.
5. **Ramp Block**: Used to modulate the gate pulse for controlling the firing angle of the Thyristor. The slope of the ramp is set to one, ensuring a linear increase in the reference signal.
6. **Scope**: Used to visualize the output voltage and current waveforms across the resistive load.

#### Working Principle
- **Thyristor Operation**: The Thyristor remains in the off state until a gate pulse is applied. Once triggered, it allows current to flow through the resistive load, provided the input voltage is positive.
- **Firing Angle Control**: The firing angle of the Thyristor is controlled by the pulse generator, which modulates when the gate pulse is applied. This allows for the control of the output voltage across the resistive load.
- **Output Waveform**: When the Thyristor is triggered, the output voltage across the resistive load increases according to the input voltage until the Thyristor turns off. The current through the load follows a similar pattern, as it is directly proportional to the voltage in a resistive circuit.
- 
![simulation_screenshot](https://github.com/user-attachments/assets/291b7790-b5d4-4a07-93c6-4d0fa249024f)

*Figure: Thyristor Circuit Simulation in Simulink*

#### Results and Analysis
- **Voltage and Current Waveforms**: The output voltage and current waveforms are in phase, typical for a purely resistive load. The waveforms demonstrate how the Thyristor controls the load voltage by varying the firing angle, directly affecting the load current.
- **Effect of Ramp Block**: The ramp block with a slope of one ensures that the gate pulse gradually increases, allowing a smooth transition in the Thyristor's firing angle, which results in a controlled output voltage rise across the resistive load.

![aaa](https://github.com/user-attachments/assets/27dd3d53-27b5-4284-9822-46e9d9f522de)
*Figure: Thyristor Circuit Simulation Results in Simulink*
#### Conclusion
This simulation provides a fundamental understanding of Thyristor operation in a DC circuit with a resistive load. By adjusting the firing angle via the pulse generator and ramp block, the output voltage and current can be effectively controlled. This setup is crucial for applications requiring precise voltage and current regulation.
