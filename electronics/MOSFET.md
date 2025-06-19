# MOSFET
aka Metal Oxide Semiconductor Field Effect Transistor<br>

**Transistor** - a semiconductor device that can amplify or switch electronic signals and electrical power.<br>
**Field Effect Transistor (FET)** - a type of transistor that, when voltage is applied to the **gate** terminal, creates an electric field that controls the current flow between the **source** and **drain** terminals.<br>
**Metal Oxide Semiconductor (MOS)** - this refers to the strucure of the MOSFET. It's comprised of a metal gate electrode, an insulating layer of silicon dioxide beneath it, and a semiconductor material (typically silicon) as a substrate. 

This *field-effect transistor (FET)* is a basic building block of most modern computer chips.
The key to its operation is its insulated gate. When a voltage is applied to the gate, it creates an electric field that changes the conductivity of a channel between the source and the drain. By varying the voltage on the gate, you can control the flow of current through this channel. This allows you to control whether the device is on/off (for our purposes, whether the bit is 0 or 1).

It typically has 3 terminals:<br>
1. **Gate:**  this is the control terminal. It's **electrically isolated** from the semiconductor material beneath it by a very thin layer of insulating material (the "Oxide"). This insulation results in high input impedance (almost no current flows through it) making it power-efficient to control.
2. **Source:**  is where the charge carriers *enter* the channel.
3. **Drain:**  is where the charge carriers *exit* the channel.
4. **Body/Bulk:**  is the main semi-conductor substrate on which the transistor is built. This terminal will almost always be connected to the source terminal, which is why I'm considering a MOSFET as a 3-terminal device.

<!-- This type of transistor is overwhelmingly the most commonly used in almost all modern digital electronic devices. The reason for its dominance comes from its key advantages:<br>
* Extremely low static power consumption:  this is the most significant advantage. In MOS circuits, when a digital gate (inverter, NAND gate, etc) is in a stable "0" or "1" state, one MOSFET 

* High input impedence:   -->

