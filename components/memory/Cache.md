# Cache`

This is a small, fast memory store with less space availability. It’s purpose is not to hold all of the data that a CPU will eventually need; the purpose is to easily access the most frequently used data. The closer the memory store is to the CPU, the faster it will be retrieved. Thus, the cache is usually found closer to the processing unit. It is magnitudes faster and smaller than [DRAM](./DRAM.md), and also provides less latency. Speaking of, the CPU’s caches are built using SRAM. This differs from DRAM, in that it’s much faster, and non-volatile. They do not need to be periodically refreshed like DRAM, making this form of memory more reliable.

Caches are designed with a principle called **locality of reference**. This is the tendency of a processor to access the same set of memory locations repetitively, over a short period of time. There are two types of reference locality:
* Temporal  -  if a piece of data is accessed, it’s likely to be accessed again soon.
* Spatial  -  if a piece of data is accessed, data located nearby in memory is likely to be accessed soon.

Modern CPUs commonly have three levels of cache: L1, L2, and L3. It begins with L1 being the closest and fastest cache to the processing unit, and L3 being the furthest away and slowest. Because L1 is right next to the processor, there is less distance for the signal to travel to and from the processor, making it the fastest cache to attempt to retrieve data from. One might think that each cache is comprised of SRAM, so shouldn’t they all have the same latency? Having more memory stores would mean taking longer to check each store until the data is found before moving on to the next cache, thereby making the smallest cache the fastest and the biggest cache the slowest. But that’s not the only determinant to speed, because they all have their individual latencies, with L1 having the smallest latency. The latencies are affected by a set of reasons:
* Physical proximity to the CPU cores
* Size and complexity of the search logic (tag lookup)
* Transistor cell design
* Associativity

The cache heirarchy is a multi-level system which is designed to utilize the pros and cons of each cache level. This theoretically provides the system with the ability to use each register level for different use cases. 