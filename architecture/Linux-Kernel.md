# Linux Kernel
[Home](../README.md)

# Linux Kernel Basics

## What is a Kernel?
It's the core of any operating system.
This layer acts like a bridge between the computer's hardware and software applications.
It's the first program loaded after the bootloader, and it manages the system's resources and provides services to user-space applications. It's like the device's nervous system or control unit.

* Hardware Interaction:  the kernel is responsible for managing and interacting directly with your computer's hardware components, including the CPU, memory, and I/O devices.
* Resource Management:  the kernel is one of the first programs loaded into memory when the computer boots up, and remains there until the system is shut down. This includes:
    - Process Management:  the kernel controls execution of programs (processes), and decides how long each process uses the CPU. This allows for multitasking, giving the illusion that multiple programs are running simultaneously.
    - Memory Management:  the kernel allocates memory space to programs and manages virtual memory, allowing programs to use more memory than physically available by temporarily storing data on the hard drive (swap space). It also ensures that one program's memory doesn't interfere with another program's memory.
    - Device Management:  it communicates with and controls all connected devices through specialized software called `device drivers`.
* System Calls:  this is how the kernel performs tasks like reading a file, writing data to a disk, accessing the network, etc. These are all services that the kernel provides, and "system calls" is how applications ask the kernel to perform them.


## Monolithic vs Microkernel
Why Linux is monolithic.

## Kernel Space vs User Space
Android OS (and many other operating systems) divide the memory into 2 areas in order to maintain system stability and security.

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


## Android's Kernel
Android uses the Linux kernel.
It's based on an upstream Linux Long Term Supported (LTS) kernel, which Google then combines with Android-specific patches. This creates what are known as Android Common Kernels (ACKs).

Newer ACKs (versions 5.4 and above) are also referred to as Generic Kernel Image (GKI) kernels, designed to separate the hardware-agnostic core kernel code from hardware-specific vendor modules.