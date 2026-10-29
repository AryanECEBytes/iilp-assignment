# iilp-assignment
# Door Status Indicator Module

Name: Aryan Raj
Course: EPDRE (Electronic Product Design and Reverse Engineering)

This is my assignment for the Door Status Indicator Module. I designed the schematic and PCB in KiCad.

## What it does

The circuit runs on 5V. A reed switch is used as the door sensor.

- Door closed: the magnet keeps the reed switch closed, so the green LED glows.
- Door open: the reed switch opens, the green LED goes off, and the red LED and buzzer turn on.

The red LED and buzzer are switched by a 2N7000 MOSFET (Q1). R2 is a pull-up resistor and R3 sits at the gate of Q1.

## Components used

- J1: 2 pin connector for 5V input
- SW1: reed switch
- D1: green LED
- D2: red LED
- BZ1: 5V buzzer
- R1, R4: 330 ohm
- R2: 10k
- R3: 1k
- Q1: 2N7000

## Files in this repo

- `Aryan_iilp.pdf`: has the schematic, routed PCB screenshot, 2D view, 3D view and BOM
- `Door_Status_Indicator-Edge_Cuts.zip`: Gerber and drill files

## Steps I followed

1. Made the schematic in KiCad
2. Assigned footprints to all the parts
3. Placed the components and routed the PCB
4. Ran ERC and DRC and fixed the errors
5. Generated the BOM and Gerber files
