The simplest defination of a process is "a program in execution", but if we want to extend it
for the sake of writing more we can write
"State of a program when executing loaded in memory"
when the code in program is loaded into memory and executed by the processor it becomes a process.
An active process also require resources to run which are managed by the OS.
For example,
- Process registers
- Program counters
- Stack pointers
- Memory pages

![[Pasted image 20230126133109.png]]

Eac Process has its own memory address space, meaning if 1 process malfunctions it does not affect any other proceses.

![[Pasted image 20230126134532.png]]
Chrome is a good example of this process isolation method, it gives each tab its own process, so when 1 tab fails other tabs are unaffected.

The info about process is stored in a data structure known as [[Process Control Block]] (PCB)