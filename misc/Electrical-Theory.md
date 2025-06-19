# Electrical Theory
This page is a short and basic primer to electrical theory. I included it with the expectation that some readers might benefit from knowledge of a lower level of abstraction before they learn about chips, PCBs, etc.<br>

An atom is the basic building block of matter. It's comprised of a nucleus containing **protons** (positive charge) and **neutrons** (neutrally charged), with **electrons** (negatively charged) orbiting around it in layers known as shells.<br>

A **charge** is the fundamental property of matter that experiences a force when placed in an electromagnetic field. Like charges repel, and opposite charges attract.<br>

Most matter has the electrons tightly bound to the nucleus. However, certain materials called **conductors** have electrons in the outermost shell loosely bound, so they can move freely from one atom to another. These electrons are known as **free electrons**.

## Current
By convention, current is said to flow from positive to negative.<br>

current - rate of flow of electric charge.<br>
coloumb - unit that represents the amount of charge transferred by a current of one amp in one second.<br>
amperes - unit of measurement for current. One amp equals one coulomb of charge passing a point per second (1A = 1C/s).

## Voltage
aka Potential Difference<br>
It's the energy per unit charge.<br>

voltage - the force/pressure that pushes electrons around a circuit.<br>
joule - standard unit of measurement for energy or work. Corresponds to one kilogram-metre squared per second squared.<br>
volt - one volt is equal to one joule of energy per coloumb of charge (1V = 1J/C).

## Resistance
All materials have some resistance. Conductors have low resistance, insulators have high resistence. Longer wires have more resistance. Thicker wires have less resistance. For most conductors, resistance increases with temperature.<br>

resistance - the opposition to the flow of electric current.<br>
Ohms - unit of measurement for resistance. 

## Ohm's Law
This describes the relationship between voltage, current, and resistance.<br>

voltage = current * resistance<br>
V = I * R<br>
I = V / R<br>
R = V / I

## Power
power - the rate at which the electrical energy is converted to another form of energy (light, heat, mechanical, etc).<br>
watts - unit of measurement for electrical power.<br>

P = V * I

Can also be expressed using **Ohm's Law**:<br>
P = I² * R<br>
P = V² / R<br>

Example:<br>
12V circuit drawing 2A of current consumes 36W of power<br>
12V * 2A = 24W

## Circuits
A complete path for electric current to flow.<br>

Power Source - provides the voltage (i.e. battery)<br>
Conductor - wire that carries the current.<br>
Load - the component that uses the electrical energy (i.e. light bulb, motor, resistor).<br>
Switch - opens or closes the circuit, controlling current flow.<br>

There are two fundamental types of circuits: **Series** and **Parallel**.

### Series Circuit
Series circuits are comprised of components which are connected end-to-end, forming a single path for current. <br>
* Current is the same through every component. 
* Voltage is divided among components.
* Resistance is the total sum of individual resistances 
    * R total = R1 + R2 + R3 ... etc

### Parallel Circuit
Parallel circuits are comprised of components which are connected across the same two points, providing multiple paths for current.
* Current is divided among all branches in the circuit.
* Voltage is the same across every component.
* the reciprocal of total Resistance is the sum of the reciprocals of individual resistances 
    * 1 / R total = 1/R1 + 1/R2 + 1/R3 ... etc

