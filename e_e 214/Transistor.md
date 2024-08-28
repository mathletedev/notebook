---
tags:
  - e_e_214
created: 2024-08-28
---

## Layout

![[Transistor 2024-08-28 09.14.28.excalidraw]]

## Silicon

Silicon is an abundant material on Earth. UV light is shone through a **photomask**. The light only goes through the apertures, changing the properties of the silicon directly under.
The silicon is then **doped** to create concentrated wells of negative charge.

## Transistor

![[Transistor 2024-08-28 09.27.10.excalidraw]]

When the switch goes to `Vdd`, negative charges are attracted to the insulator. This creates a **negative channel** that allows current to flow.
When the switch goes to `GND`, positive charges are attracted to the insulator. This creates a **positive channel** that prevents current from flowing.

**Transistor** (transform resistor): An electronic switch that can be turned on or off (or even somewhere in between!).

**Field Effect Transistor**:
**nFET**: Uses negative channels (e.g. doped with phosphorus). Turns on with a `1`, conducts `0` well.
**pFET**: Uses positive channels (e.g. doped with boron). Turns on with a `0`, conducts `1` well.

### Shorthand Symbols

![[Transistor 2024-08-28 09.42.42.excalidraw]]

You shouldn't connect an nFET source to `Vdd`, since you're trying to move positive charges through a negative channel. Vice versa for pFET. Therefore,
- Always connect pFET source to `Vdd`.
- Always connect nFET source to `GND`.
- Only use as many FETs as needed.

> *Rule*
> Always drive output to `0` or `1`.
> Never drive output to `0` and `1` simultaneously. This creates a short circuit.