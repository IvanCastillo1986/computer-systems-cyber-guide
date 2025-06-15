# Path of data

## Initial Power Up
1. User presses power button. Electrical circuit closes
2. PSU receives electrical signal and begins POST (power on self-test). After passing test, power provided to rest of circuit
3. Motherboard receives signal after test. Chipset/embedded controllers receive power (ie. platform Controller Hub aka PCH)
4. Baseboard Management Controller (BMC) in servers signal CPU to leave reset state
5.user presses power btn -> electrical signal closes -> 
6. CPU executes boot ROM. First tiny amount of code is read (small, unchangeable ROM). It's just enough to begin CPU functions towards motherboard's BIOS/EU (Basic Input/Output System, Unified Extensive Firmware Interface)
7. CPU uses signal to run BIOS or UEFI firmware, which in turn runs POST

User presses power button -> 
electrical circuit closes -> 
PSU receives electrical signal and begins POST (power on self-test) -> 
motherboard passes POST -> 
motherboard receives power signal -> 
Chipset/embedded controllers receive power (ie. PCH) -> 
Baseboard Management Controller (BMC) in servers signal CPU to leave reset state -> 
CPU executes boot ROM -> 
first tiny amount of code is read (small, unchangeable ROM). It's just enough to begin CPU functions towards motherboard's BIOS/EUFI (Basic Input/Output System, Unified Extensive Firmware Interface) -> 
CPU uses signal to run BIOS or UEFI firmware -> 
BIOS/UEFI runs POST -> 

## OS Boot and Driver Load
1. OS Load - after POST, BIOS/UEFI passes on to OS.
2. OS recognizes CPU - The OS looks for hardware. OS finds video card CPU.
3. Graphics Driver Loading - crucial step. OS loads specific graphics driver (NVIDIA GeForce, AMD Radeon driver) for video card. Video driver is bridge between OS and GPU communication

## Data Flow for Graphics Rendering
