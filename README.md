# Pulse Induction (PI) Metal Detector Board

2-layer mixed-signal PCB for a pulse induction metal detector: an STM32 microcontroller, a high-power MOSFET coil driver and an op-amp analog front end.


## How a PI detector works

A pulse induction detector drives its coil with short, strong current pulses and then looks at the signal that decays after each pulse. A metal target changes that decay, and the change is very small, so the receiving circuit has to amplify and condition it carefully before the microcontroller can use it.

## Hardware

| Block | Implementation |
|---|---|
| MCU | STM32F103C8T6 |
| Coil driver | High-power MOSFET switching stage with flyback diode protection for the inductive coil |
| Analog front end | Op-amp stages that amplify and condition the weak target reflection signal |
| Power | Linear regulation with capacitive noise filtering |
| Indicators | Audio and visual indicators |
| PCB | 2 layers, designed in [Altium Designer / KiCad] |



Schematic: [`docs/schematic.pdf`](docs/schematic.pdf) · PCB views: `docs/pcb_top.png`, `docs/pcb_bottom.png`




