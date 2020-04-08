# virtual_memory
The following project makes use of two pieces of software, namely Weensy OS and hardware emulator QEMU. 

When you run Weensy OS, it displays a visual representation of both physical and virtual memory. Highlighted memory addresses indicate the pages accessible by each process upon execution. Below are two labeled memory diagrams, showing what the characters mean and how memory is arranged:

Initial state of memory shows no isolation, address space abstraction and processes cannot implement fork nor exit.


Implemented isolation using virtual memory, so that a process cannot modify kernel or other processes’ code/data + abstract address space for each process + fork and exit system calls on Weensy OS such that upon calling specific allocator programs on the machine, we can get desired behavior of memory usage and allocation.

Normal allocator:

Forking allocator:

Fork-exit allocator (runs indefinitely):
