# Analog Prototyping System
## What?
A modular prototyping platform for precision and high-speed analog circuits.
## Why?
Some circuits can be prototyped on a solderless breadboard, and some circuits can be made on perfboard. But both these prototyping methods lack a low-impedance ground plane, which can affect performance. The base board of this system consists of uninterrupted ground planes on both sides, and inner power planes broken out through pin headers. 
## Layout?
- Base board (in Eurocard form factor) with exposed ground planes on both sides and four internal planes (split over two layers) broken out using pin headers placed in a grid across the plane.
- IC boards including: SOIC-8 breakout with single-sided pads to solder wires to and component footprints on and across all pins with appropriate decoupling footprints to fit most standard op-amp/comparator/IC pinouts. 
- Passive boards including: 4- and 8- component breakouts for parts 1206 or smaller.
- SOT-32 breakouts for multiple SOT-32 transistors/regulators.
- Each board has castellated "anchor" pads that can be connected to base board ground plane.
## Really, why?
This project was inspired by [Mark's](https://github.com/macaba) (unreleased) prototyping system for analog circuits. Modifications include not segmenting the main planes and a different form factor.
## And?
Connections between components are meant to be made using enamelled copper wire soldered directly to breakout pads or the ground plane for low-inductance, low-capacitance wiring. Since this is basically a Manhattan prototyping, limitations apply.
## Details?
Boards so far:
- Base board (100mm x 75mm)
- SOIC-8 Breakout with passives
- 8-component breakout
- SOT-32 breakout
