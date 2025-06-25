[Home](/README.md)

# Reference
Some of the terms will be linked to here, so as not to obscure important information in the main articles.
<hr>


## flash memory
* a type of of non-volatile computer memory (unlike RAM which loses data when power is removed) that can be erased and reprogrammed with electrical signals. This means it retains data even when the power is turned off, making it ideal for permanent or long-term storage in a wide range of devices. It typically erases data in blocks rather than individual bytes, and has a finite number of write/erase cycles until it wears out. It's solid-state, since it has no moving parts (unlike HDDs), making it more durable, quiet, and resistant to shock/vibrations. <br>
* It works by storing information in an array of memory cells, each made from a **floating-gate transistor**. These transistors can trap electrons, and the presence or absence of these trapped electrons determine whether a memory cell stores a binary "0" or "1". 
* it has faster read/write speeds compared to HDDs, leading to quicker boot times, faster application launches, and overall improved system performance.
* flash memory is ubiquitous in modern electronics in modern electronics due to above stated benefits: 
    - USB flash drives - portable storage
    - SSDs - replaces traditional HDD in computers
    - Memory Cards - digital cameras, smartphones, tablets, SD cards, etc.
    - Embedded Systems - IoT devices, routers, even BIOS chips in computers for storing firmware.
    - Gaming consoles - game data, system updates, user profiles.
* the two main types of memory are:
    - NAND Flash - optimized for high-density data storage and fast write speeds. Commonly found in SSDs, USB drives, memory cards. 
    - NOR Flash - known for direct random access capabilities. Suitable for executing code directly, such as in embedded systems for boot code and firmware. 


## boot ROM
* a critical piece of firmware embedded directly into a computer system CPU or a dedicated chip. It's the first set of instructions executed by the processor immediately after power-on or a reset. 


## Chips
aka **Integrated Circuits (ICs)**

Chips are essentially a way of modularizing circuits. That is, delegating just one segment of your full computer's circuits to accomplish a task. 

Examples of chips accomplishing different tasks are:<br>
**Microprocessor chip** performs calculations and controls.
**Memory chip** stores data.
**Amplifier chip** boosts signal strength.
**Voltage Regulator chip** provides a stable power supply. 

Each of the listed chips encapsulates a complex circuit into a single, manageable component. If an issue is diagnosed (the computer turns off unexpectedly), a technician might think to look into troubleshooting near the chip that handles that task (the Voltage Regulator chip).

Old circuits were built using discrete components (large, standalone pieces like a diode or transistor) that had to be wired together manually. The **Integrated Circuit** solved this issue in the 1950's, revolutionizing electronics. Now, circuits that perform specific tasks would not need to be made from scratch. Instead engineers were able to select pre-made circuits and connect them together, like Lego blocks, which reduced complexity and cost. This modularity also allowed for abstraction in larger systems.


## Program Counter
aka **Instruction Pointer**


## PATA
Parallel Advanced Technology Attachment (PATA) is an older interface used to connect storage devices to a computer’s motherboard. These devices included: 
* Hard Drives
* CD-ROM drives
* Floppy Disk Drives

Some of these devices might give a clue as to how outdated this interface is. It was replaced by SATA (Serial Advanced Technology Attachment) when its specifications were released in 2003. At this point, many companies began to adapt the superior interface, which became the new standard.

The reasons for this are:
* SATA offered significantly higher data rate transfer
* SATA cables are much thinner and flexible than PATA’s older ribbon cables
* the new cables provided for much more airflow and management to the computer’s hardware
* PATA was not able to hot-swap (connect or disconnect drives while the computer is powered on)

By 2008 (only 5 years later), SATA had recieved over 99% of market shares, making the older PATA obsolete.


## M.2 slot
A type of expansion slot on a motherboard that serves as a connection point for high-speed solid-state drives, but can also be used for other devices like wireless cards. It offers a compact form factor and significantly faster data transfer rates compared to older interfaces like mSATA. 
* it is designed to accomodate various devices, with SSDs being the most common. 
* it can also host wireless cards, Bluetooth modules, and other expansion cards.
* it’s a smaller, more streamlined form factor compared to previous expansion slots. This makes it ideal for laptops where space is limited.
* it can utilize the PCIe (Peripheral Component Interconnect Express) interface, which is significantly faster than the older SATA (Serial ATA) interface used by many traditional SSDs. This allows much faster data transfer speeds, leading to improved system performance.
* it can support both SATA and NVMe (Non-Volatile Memory Express) protocols for SSDs. NVMe SSDs leverage the PCIe interface and offer even higher performance than SATA M.2 SSDs.


## 