# SATA
The Serial Advanced Technology Attachment (SATA) interface is a widely used computer bus interface for connecting storage devices to a computer's motherboard.
These devices can be:
* Hard Disk Drives
* Solid State Drives
* Optical Drives

This standard replaces the older [Parallel Advanced Technology Attachment (PATA)](../reference.md#pata) interface, which provided slower transfer speeds and outdated features (such as bigger cables). PATA used wide ribbon cables and a parallel data transfer method, which was more susceptible to interference. It also limited the cable length. 

SATA instead uses a serial communication method. Through this manner, you only have one data line transferring 1 bit at a time. It might seem counter-intuitive, but this allows for higher transfer rates. 


## Why would SATA be more efficient than PATA?
Serial communication became the standard for a few reasons:
* It's difficult to synchronize data bits that are sent at the same time, when working with too many of the ribbon wires used in PATA systems. This lack of synchronization is known as **Clock Skew**. And it was susceptible to even the tiniest manufacturing flaw.
* The information that a user sees on a monitor (like the letter "a") is the result of the computer reading *many data bits* and displaying it. The reciever in a PATA system had to wait for the last data bit to arrive at the end of the line, before it was ready to finish processing and displaying it. As signal frequencies increase, the reciever of the data bits would have to wait, causing a bottleneck. This slowed down the total transfer of bits.
* In SATA systems the reciever only has to synchronize one stream of data. This eliminates the need for the reciever to have to synchronize multiple parallel data streams efficiently, which greatly provides high individual signal frequencies.
* The electro-magnetic fields of one wire in a parallel ribbon cable can interfere with adjacent wires. The noise from the interference can corrupt data on adjacent lines, requiring error detection and retransmission. This interference is known as **Crosstalk**.
* SATA is cheaper. PATA cables were wide, bulky ribbons consisting of 40-80 wires, which meant more cost to manufacture.
* The wide ribbons from PATA cables impeded air flow within a computer, making it more vulnerablne to overheating.
* PATA ribbon cables were limited to short distances, since *Clock Skew* and *Crosstalk* became amplified over longer distances.


## What is SATA?
<!-- TODO: Deep dive into SATA here -->
