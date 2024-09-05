# Programmable Gain Amplifier (PGA)

## Overview
This project involves designing and implementing a Programmable Gain Amplifier (PGA) using discrete components. The PGA's gain is adjustable through two TTL control inputs, allowing for multiple gain settings.

## Features
- **Adjustable Gain**: Controlled by two TTL inputs with four possible settings.
- **Components Used**: Op-Amp, NPN transistors, analog switch, resistors, and a Zener diode.
- **Gain Settings**: 
  - A = 0, B = 0: Gain = 1
  - A = 0, B = 1: Gain = 10
  - A = 1, B = 0: Gain = 50
  - A = 1, B = 1: Gain = 100

## Components Required
- Breadboard x2
- Wires
- Function Generator
- Oscilloscope
- DC Power Supply (+5 V, 0 V, -5 V)
- NPN Transistors (2N2222A) x4
- Op-Amp (UA741) x1
- Analog Switch (CD4066E) x1
- Zener Diode
- Resistors: 8.2 kΩ x2, 100 kΩ x1, 20 kΩ x1, 3.3 kΩ x1, 4.7 kΩ x1

## Circuit Design
The PGA uses a non-inverting Op-Amp configuration with feedback resistances controlled through analog switches. The switches are controlled by TTL inputs to set the desired gain.

## Level Shifter
A level shifter converts TTL logic levels to bipolar control signals required for the analog switch. It includes a 2N2222A NPN transistor and a Zener diode.

## Experimental Observations
Gain values were verified for different TTL input combinations:
- **A = 0, B = 0**: Gain = 1
- **A = 0, B = 1**: Gain = 10.08
- **A = 1, B = 0**: Gain = 51.2
- **A = 1, B = 1**: Gain = 100.2

## Conclusion
A PGA with programmable gain control was successfully designed and implemented using discrete components, demonstrating the ability to set and measure different gain levels accurately.
