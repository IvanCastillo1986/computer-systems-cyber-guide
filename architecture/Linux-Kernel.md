# Linux Kernel
[Home](../README.md)

# Linux Kernel Basics

## What is a Kernel?
It's the core of any operating system.
This layer acts like a bridge between the computer's hardware and software applications.
It's the first program loaded after the bootloader, and it manages the system's resources and provides services to user-space applications. It's like the device's nervous system or control unit.


## Hardware
The kernel is responsible for managing and interacting directly with your computer's hardware components, including the CPU (Processor), memory (RAM), and input/output (I/O) devices like hard drives, keyboards, and printers. It translates requests from software into commands the hardware can understand. 


## Monolithic vs Microkernel
Why Linux is monolithic.

## Kernel Space vs User Space
### Kernel Space
It's a privileged memory area where the kernel code resides and executes.
It has direct access to all hardware and memory.
If a program in kernel space crashes, it typically brings down the entire system.

### User Space
It's the space where the applications that the user has access to run.
These applications have limited access to hardware and memory, and they must request services from the kernel through system calls.
If a user space application crashes, it usually doesn't affect the rest of the system.


## System Calls
These are the primary interface between user-space applications and the kernel.


## Processes and Threads


## Memory Management
Virtual memory, paging, memory allocation.


## File Systems
VFS (Virtual File System) and common Linux file systems (ext4, procfs, sysfs).


## Device Drivers
How hardware interacts with the kernel.


## Interrupts and Interrupt Handlers


