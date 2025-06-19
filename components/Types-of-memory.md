[Home](/README.md)

# Types of Memory

# Primary Memory
This is the computer's short-term workspace, and the CPU can directly access it for immediate operations.
As soon as power is removed, RAM loses all memory, as opposed to a HDD which persists data even after powering off.

## Random Access Memory (RAM)
"Random Access" means that the CPU can access any location in memory. 
<!-- ToDo: continue here -->

* volatile - loses data when power off
* read/write - CPU can both read from and write data to any location in RAM
* temporarily stores data/programs that CPU actively uses, enabling quick access for processes and multi-tasking
* types of RAM:  
    * Dynamic RAM (DRAM)  -  DRAM is the most common type for main system memory. Each cell consists of a transistor and a capacitor. Capacitors require periodic refreshing to maintain their charge (and thus data). 
        * Synchronous DRAM  -  synchronizes memory speed with CPU clock speed.
        * Double Data Rate SDRAM (DDR SDRAM) - faster version of SDRAM which transfers data on both the rising and falling edges of clock signal. DDR, DDR2, DDR3, DDR4, DDR5 are successive generations. Each of them offer higher speed and bandwidth.
    * Static RAM (SRAM)  -  more expensive/faster than DRAM. Each cell uses multiple transistors. Usually uses 6 transistors. 


## Read-Only Memory (ROM)
* non-volatile  -  ROM retains its data even when the power is off.
* read-only (primarily)  -  data in ROM is permanent and cannot be easily erased.
* stores critical firmware and instructions (BIOS/UEFI) needed to boot the computer and initialize hardware components.
* Types of ROM:
    * Mask ROM (MROM)  -  can’t be changed because it’s programmed during manufacturing.
    * Programmable ROM (PROM)  -  can be programmed once by user.
    * Electrically Erasable PROM (EEPROM)  -  can be erased and reprogrammed electrically, without removing it from the device.
    * Flash Memory  -  a type of EEPROM that can be erased amd reprogrammed in blocks. It’s suitable for solid-state drives (SSDs), USB drives, and memory cards. It has faster read speeds than traditional HDDs and is non-volatile.

## Cache Memory
* volatile  -  loses memory when power off (like RAM)
* much faster than RAM
* small, high-speed memory unit lcated very close to or within CPU. Stores frequently used data and instructions from main memory to reduce time that CPU waits for data, improving system and performance.
* organized in levels (L1, L2, L3 cache)
    * L1 is fastest/smallest
    * L3 is slowest/largest

## Virtual Memory
* not distinct hardware component
* it’s a memory management technique that uses portion of secondary storage (HDD, SDD) as temporary extension of RAM when physical RAM is full and not available.
* it prevents crashes (like a last resort backup) from insufficient memory. If this weren’t available, it would task the system into crashing. 


# Secondary Memory
aka External memory or Auxiliary storage
non-volatile and provides persistent long term storage for large amounts of data. 
Its typically slower than primary memory, and not directly accessible by the CPU.
Data must be loaded into primary memory first.

## Hard Disk Drive (HDD)
* non-volatile  -  retains data without power
* stores data magnetically on spinning platters
* because it’s slower and more prone to mechanical failure than SSD, it’s inexpensive in comparison

## Solid State Drives (SSD)
* non-volatile
* uses NAND flash memory to store data on integrated circuits
* is more expensive than HDD because it’s faster, more durable, and consumes less power

## Optical Discs
* non-volatile
* used for data archiving, software distribution, and media playback
* CDs, DVDs, Blu-ray Discs, etc.

## Magnetic Tape
* non-volatile
* large capacity
* access is sequential and slow, thus its low cost per GB
* good for large-scale data backup and archiving

