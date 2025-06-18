[Home](/README.md)

# Android boot-up
The boot-up process of a Android smartphone is a sequence of steps that takes the device from powered-up state to fully functional OS. Several layers of software and hardware interact in a precise order.

1. Boot ROM (Power on and System Startup)
* User presses power button: the device's System-on-Chip (SoC) is powered on.
* Very first code executes in **Boot ROM** which is a small, immutable piece of code hardwired into the chip's read-only-memory (ROM). 
* Its primary job is to perform basic hardware initialization (like checking memory)
* It then locates and loads the next stage of the boot process **the Bootloader** into RAM. 
* It verifies the authenticity of the Bootloader for security.

user presses power button -> SoC chip powers on -> Boot ROM code executes from chip's ROM -> 

2. Bootloader




# Vulnerabilities
Vulnerabilities boot-up. Malware can inject itself before the OS even loads. This means that the boot process is an attack vector. 