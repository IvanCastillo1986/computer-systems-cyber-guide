# Generic Kernel Image

**GKI**  -  hardware-agnostic core kernel. aka General Kernel Image
**System-on-Chip (SOC)**  -  hardware-specific modules.
**ACK**  -  


GKI initiative was created by Google.
Solves issues with kernel fragmentation because each System-on-Chip vendor and device manufacturer had its own modifications for ACK (Android Common Kernel), which slowed down production and performance.

It unifies the core kernel library (GKI).
This kernel is **hardware-agnostic**. Because it's used by so many different Android devices, it isn't tailored for any device's specific hardware, hence "agnostic".

System-on-Chips (SoCs) are **hardware-specific** modules, specific to the manufacturer device's hardware. This is board-specific support. This means that code and drivers are for specific computer components with specific circuit boards (WiFi card, speaker board, micrphone board, etc).

## Before GKI
The whole kernel (including hardware-specific modules) used to be compiled into one big monolithic image. Updating a driver for one component would mean recompiling and flashing a new image. For developers, this is similar to not having modules from libraries.

## After GKI
You now have a "framework" and "interfaces" with hardware-specific logic that controls hardware. The logic for specific components (custom image signal processor, particular touchscreen controller, etc) reside in the separate, loadable vendor modules. When the GKI boots, it loads the vendor modules. These modules allow it to interact with specific hardware on that device.

This modularity allows for faster updates and reduced fragmentation, since they allow for one core to be used between different companies. The separate components can contain their own logic (instead of rewriting one entire monolithic image). 
