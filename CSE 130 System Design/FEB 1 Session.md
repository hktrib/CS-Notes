## Interupts

#### **Two types of Interrupts
* Computer-Wide: 
	* Hardware such as a disk or network card
* Thead-specific:
	* Address error, illegal instruction, math error, trap



###### Computer-Wide





###### Thread-Specific


## Virtual Memory
* All threads share the same physical memory pool
	* only one location for any given address
	* programs must be able to run anywhere in memory
* Abstraction each thread gets its own memory pool
	* Address range from 0-2^n - 1
	* Myltple phyiscal location (one per thread) with virtual address 0x1000
	* Thread + virtual memory = process
* Result 
	* Programmer always sees the same addresses regardless of where in physical memory the program is located





#### Thread Communication link: Bounded Buffer
* Op



