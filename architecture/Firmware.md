# Firmware
Generally written in low-level languages that allow direct interaction with hardware.
The most common languages for firmware development are C, C++, and Assembly.


## Is firmware written for SoCs, or core kernel?
OEM flashes the firmware for various hardware device components. 

This includes
• SoC firmware
• Component-specific firmware
• Bootloader firmware

NOR flash - 
- suitable for code that needs to be read directly by the processor because of it's parallel nature. This is because of direct access to memory
- primarily interact with C because it gives low-level access to memory addresses and hardware registers that are important for flash
- BIOS / UEFI firmware
- faster reading
- byte-level random access

NAND flash - 
- HHD, USB cards, memory cards
- higher density, lower bit cost
not used for Firmware cuz it'd require a Bootloader
